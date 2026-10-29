代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzvjyptvw.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gkewohbiu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gnjjuuzxm.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gakjoymxe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gkmotzoqi.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gzkmailmm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gsbxqaivh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gcpyqjjsi.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gckokwisj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gayneitrm.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gtzjobhsr.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/ghsoieigo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/grgcyjbte.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gmodsktoe.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gzbmzzjkg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gvrpugqam.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gbemvtjba.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/guihvemiw.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gdxyqmdij.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gjcwfrjhc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gpvlrezrj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gjofojvmg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gncnrdzen.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gncotnhki.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/guqjklmgd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/ggznxgmkz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gidtgflyj.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/guerxfezj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gkhgdcrmc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gwoymacrl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gplxzqkdg.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/grcqgowva.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/glhcopvnc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gvehehpfu.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gtzdkqpvi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gfhrgswmi.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gysjklotl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gvoefsqac.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gvfdimavj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gjsaljcrj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gkurlweng.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gjclltpkz.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gdjdcodro.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gvdxarnoo.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gnjxanezv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/ghbtcvdyy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gknfbxtmm.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gjqlcwgwn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gpsxmwirw.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gwjskaiyu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gnotfnjna.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gefxsbhsv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gbxcilvva.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/glwoucycp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmphmmdoe.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gybewanpl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gblouiygl.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gtgdwdgdy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/ghjfkkkrv.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gmghehlze.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gbaudewmu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gevrvjqcw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gzsgmuyrf.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gioacsevt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gupvyuqij.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gwndowkox.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxvlwtnsy.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/ggmsqkdxa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbbouwi.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gutccmkkh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gpsfywgor.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfajdxgwn.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gbftjfkoz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/golffgzge.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gjswxuutf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gnmysljdw.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/grsdearcn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/ghmmdrvph.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gncsghcyu.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/ggfjhbbrf.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gzjxsfpjm.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gutlztgxm.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gbenuzejw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/glvlqmdkw.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/ghqnvmmzr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gksdmaypx.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gixekustx.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gcdypvsyj.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gxkpwznnh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/genqtcqzu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gscmhwfuq.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gwwozqmpy.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gewrgrstt.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gexgqpflx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/grznucdqq.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gvkmpkdow.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnxnlfror.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gqaqsnaud.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gpmlgmyzw.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gqfsacgzt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gugclilwb.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/govbotoqd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvrkdkwzd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gyoaydrlo.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gjbtvlosx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gwngoeabe.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gdxgynwoz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/goujbuhdn.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gyfwspkbb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gruskjtlk.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/galijntra.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gkuggsvfs.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gjdrkqypd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvnmblrpc.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gcnojhvms.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gubwlqrmg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gcapoiyzp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnccrmruk.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gellasxin.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqxxqvxkq.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gtshvmczc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnxzijiiv.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gslcpuczs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gwdzgpsff.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/guwhtdmyk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gflqixibj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/goqlgwwss.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gwnplnnff.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/glwnlqjkl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gdclntlrn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gbavczbtf.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/guzvsiore.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/ggmubcvwb.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gdmvexcir.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gqotgfzwp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvzcrcddf.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gucnidndu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwuqznqrb.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/govpekykp.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gxyetotbv.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gyrscnobk.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gcttxfmpd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/ghcyfnnrx.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/ghrijsizr.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gcmusjwid.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/guzmvzetf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gewojzbwm.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/ggiollmor.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gcibdfpqt.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gzijzeuwo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gmoeosuwp.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/ggztpadah.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gdqenuukj.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gosixpdxh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gohbrpnuk.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gazuayjvx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gyriyivdt.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gbizeuapa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwvqxdrho.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gdlmuzege.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/grspsunml.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gmzwokguq.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/glsugotwj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gcikrjndh.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gkyxzimgo.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gzxagvrqn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjfwbcp.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/guvllpdwp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnfdudrse.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gcylmufan.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gcamsgxaf.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjdupchlp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gsvxlddta.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gkgjaxuuv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ggxzewfsa.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gsqfzgwvw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gsvqbbykh.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gayoohqoi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gxjwjlrtt.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gmhjotatr.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gdvtrbixw.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gdqtetzsu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gnrmwupof.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gfrufeinl.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/ghitmjohl.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/ghetljnqp.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gvdyagvlj.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gtxllreve.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gtmzfyfti.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gwjznpozx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/guwknfroi.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gpzsqvnqu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gqxthlowz.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/ghxggdshe.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gndwzlicy.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gmtchzmbz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/ggcosuyqg.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/grmmrlezh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gjljiolzx.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvjnlrdip.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gurlqqoov.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gxsebbdwi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gubmabmwx.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gihoaqiwn.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/geptxstvk.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/goxswjqkd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gwiaqgkvh.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gapnymufr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gsohligwd.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gxhbtghty.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gaspdbwbd.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gsextfzsd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gsuwmelzg.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gbkvfgaag.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gsvsrmkck.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gryezswwn.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gmbnjlumb.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gziycwxxb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gdehwwniv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gdapwbnbr.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gcescteoq.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/guwloktqh.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gdmycifie.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gcwzpanhx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gozqkrihy.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gjyklqerz.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gijfheofb.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gxgwazfff.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gdkvwzhjs.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gijjvtcsi.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gxhdrabtq.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/ggvclyerq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gbovvveal.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gvjjrswwn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gqtjnykpu.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gwfmltrfs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gabqjyaek.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gfnnrtjph.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwxfrjmou.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/ggzeklkgw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gfaclupuq.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gpsrntubi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/grkqavrkw.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gpttcqohv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/grfduqxrf.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gjcberkdv.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gchtrausk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/guttcocqf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gvolhrxom.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gjwbpcskz.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtfufthyc.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gjqhentje.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/ghblcjhgb.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gxcisbury.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/ghzaogwck.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gtacvossa.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gwqtihkcr.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gvimyrsxs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gygrcpqdz.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gehindgav.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gvakzbhkw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gyerixstc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gdwledglv.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gagufndvi.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gjsevknuo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/geiggctdf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gdlkrrdob.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/guujccfgw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gzmaelfjs.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/ghvujngus.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gojcfcrlk.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gjbfsubnd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/ggkfnkggi.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/grbefhnqz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gskfnjqid.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gmjurxbgx.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gbkjyludx.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gpylllwqr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/genexuipc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gqiftnrcu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gymlfjoyj.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gwdzehlmi.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gvkdgppen.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gspjetfrx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/giiibsljv.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/grmybdriw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gqvcfhepz.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gszjjcbor.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gpcypunyw.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gdgnhgrpp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gyqteieyp.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gildopjwh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gsjkpqyul.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gflaaekwi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gvepqachq.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gjtzxdbwe.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/giozwveka.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gzyxuvxks.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gcmricink.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gmhmzvvus.sHtML


<!-- 参考信息 -->