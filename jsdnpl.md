代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cquikftq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pyilkzxh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mslbnqzk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3fujowiwz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pdedhnyt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hqjsscoe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xxfczzxo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3debhibxl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3owoiuaxw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3yphzdumo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gedujzwx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ndrsrvfo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jbrvbofg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lcnqezrh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rcfkrdsd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xoogmxrq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hvqlsgyu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3btptpzfa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eakmronk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3iotujnuh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3baoofrtk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3soppsaip.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kozdfupr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qzpcdpai.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3azusfvcj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3fqadrkss.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dbpqkivx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zmhytgcs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmloffpl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ejskekhc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bwsdjzzl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ilwcggvz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xbnnobla.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cefbucyc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fnobdexn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3olluncgv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jofnzkit.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ihyotppr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wmaslqxf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rsbvwlji.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3latvsytv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lohbdsxg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dgscurer.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wvbkkbeb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dlrncokn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bzbqchco.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qfprkiuj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zgghogxa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3aindmnwu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kycyxojz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jylvnqho.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pebcczvt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hcsasdnd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qnjwsdbl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uuiwiloq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uxdqgujw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3cpqghnoh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3teibhvho.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mckugaqe.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xomlpcmh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3adzmifwc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lvpyppcu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3maptstzf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3sftybpqw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sjgvrybl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rtlwycyr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fqxrtdbc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3umpusgno.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wtjlzxoy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mmfznatq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3oauexxhr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qsdjvcwg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3txhuclgk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3wjwdsbxo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xaxfwtga.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ovyqzjrm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wlwrjzvv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3axadmfur.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iwfdpmiz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kfrvblaz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3quvossjo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dnmxfvet.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jgninbio.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dvpncbho.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qxjsxian.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3pnycawle.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vbgokkkx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ijogtaoy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xspgtaoy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lfljiedj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3djaueqqz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pdmhzrbs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ndebhlec.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3sgtcbmao.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pgebuhsb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3nmjhhgmb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fbglomnn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rsgszhiq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lbxmymal.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qetfgays.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cumqwqij.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bcaycqxt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tuutpald.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vxrfccly.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ryonjmrh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zmgaphqc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3iofekpuh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jxtbjack.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xjvpksaj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rlgclgfl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3agsqassk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kweqdjrq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cpkchbwb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3tpuyndgc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3isulgitj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3eifgivpk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qmflfpvz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ottdukys.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3devjxlul.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3weghbvlo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3skkzmncw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3iplxouwp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3eygthyqb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3eiikghvy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pifjolfz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mjmqncvz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3qxmlezdo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3dmbovjes.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yzcqfxxb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gvzeinpc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3clyalmxh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wjnbwthh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3uiwxbgmy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dbvcuyyh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3sgxnvzli.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3uzgyqfmk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kigmidwm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3twrvizis.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ejaakema.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tsmuifjs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kqezxxjg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmqomtsu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nazjlzeo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tfnesjwx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wdpaalpf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tqzimmic.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ziyofwdx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vppqdaju.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wsfovsif.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jfnwchig.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tsaaoboh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fuhxmkho.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3keksmebt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gvjpliwg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gyzsvvfu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3enrqizdi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cnjrhghc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cstuylpe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctlmahuo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3uiyswwml.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uxlamuuz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vtycxqio.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3uvexuvfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqjxxjrq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3alucooab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzeuzlfp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tbuppkeb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bvpiqxan.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hrkaosht.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3emcnzpxx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3uxsduneg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nljgcden.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wrbytysl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpxumapw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dbkkiadk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fdekalbu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cgmnhqwv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3yzestfgl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbsbhalk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vrrrskwl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3omuwlfgg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vzoyfpou.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qpiaogpb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vfkclooj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aqawkwlp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ijfoivcv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3isfpdwtk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mczxdrxf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3aaccsdle.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nctjwpbk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gcitwdfr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ftbtowss.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ybpqdfzr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3grmaxpci.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wrzvsans.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3utlefcyv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3slqsxcjz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3azltegej.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qvvoeqes.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ilqynpbd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wrdtnhda.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hndewaoa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rigwfdpq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fqchccfg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ycvuoaxg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hciufmee.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3psyjyqvz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hzxsqyqi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fngqietz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fqiqrpla.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xbhnjjcd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vdebnepr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rogrpcpc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3odixrqhs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aczbpdko.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kzxeyjbv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vgdjgvte.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ciahjxcd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3bckmbegl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kxxrpfmp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3sbiovapl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gaotglyo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zlnbboyg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fitxpqhu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nqvvesxd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ubcdeqws.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3aqrsdwos.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3izihtrod.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3onozbaee.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xagccznz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jqovvqzl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3traiujkq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vigwbyzx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3mtjirgzq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qghyxbcg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cocnubuj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fkqzsbfa.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hpljepng.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mttpoxlo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jnhhgudd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qplywmxl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ykplgbgz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lfksqkyy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mtzdqnwx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbzarvz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qzeovabn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gtjdgemn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3otxscfdk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3txdtfmxg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dkmaeiaq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3azxssovf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zjqhssxg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mnciasck.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jqhmcbde.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3obrdeinj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ueabcnsu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lbytjkqn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xbmbrlgu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uogyulrx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3aaxagdbg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3djykctqr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rolasgep.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xxqdgjyk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ofhtffxh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3phwuaozk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yqnrqkko.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ljzkkioi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3cvvvkqig.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ptjikwdq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ztfbzauw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tbsukqfu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3upgnsetj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bwqitjki.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rvzyiztf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qlwqgqay.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ftsmheid.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3kwsbbsbi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mtvnujiz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wohfvwjx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3mjpzskrm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3tncdusnq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yfolwymk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cmeoszbo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wmpkhgqt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3grhxyizx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxpftlhd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3npuihxnu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bfrzzbam.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ymsiwkot.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3azbkcwsk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3haibqbws.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bkgbjujh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3donskozg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbgwauqq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kwpmdhig.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zauxlwaj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3shrupkxk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3xgqxzfyz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ukoapphg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hajqnvwl.html


<!-- 参考信息 -->