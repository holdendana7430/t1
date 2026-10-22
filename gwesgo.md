代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2dxcurrwa.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2eghlgaxl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2rrjltway.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2pgebzskz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hnfkaesa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lgwjbebl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2lqvvcdbx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qzkzfmqx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zixlrilq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qtsynblt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzycfxnw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gneqlcuv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2aonciijn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rpxbensr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bticlvdg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2pjwqlepc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvgiqevu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tyxkvjtc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kpnulqpu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oupsdftb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sxurhtxk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gevnfoox.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jmbzwmce.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qxtnhtct.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qezoxwti.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uuxntgkn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ahvizqmv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2orwmmnaz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wudyaesh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2btqqlxow.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2chdrfafg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zhuyhxuj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ddaspwfb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fnqyhmra.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2knjqgkzh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yotgmvdk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bckpfikv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rfysksth.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2uwwuqggu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qzmvhpww.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ubbawukv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mvkyytql.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2eawsuudv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kuwqcbaq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gtswagby.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2eehzkfby.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2jmrkshvj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mbrufahc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wsonbsrw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gwowpsms.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ugwcahxg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nvmzhlue.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rckcudsk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2txyjgiqb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2giibsyyl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2unghpdzv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wwhyyfhh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jzvoplyu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2igktjhzd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mnybplka.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2twdlhowz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ehuisjbl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bqaomhrv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2iwdtdinn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xtfdxeyf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ggufsevh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2vcgdsnwy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2dfzdjwwg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2znemmhva.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cydqqikn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ffxadjnu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xhyrojhu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2illjixqh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vgozmrpg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fmmmsyil.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2rvehvzee.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2icscfwny.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2egmawiwi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xuxtqwgv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nfxapulq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wnzzchjt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cztbvfgw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2woalltkq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2jvutvjsz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2viufpbjx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ebryijrb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hpnusglc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2tvioqwtr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xfliscjf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2iqhlizxr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dvmayeom.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nwiwjvxz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2doohifbq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jphwgxpa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qduifvde.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2madvlyac.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2eqmyslqi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ttrsreev.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2prnkoqpg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2prjopunn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cehrrsqx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xezqznkj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gkbwlicz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2yzxssatu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uwldzjdh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ecwskqww.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hfocyowm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2haokrmcj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tirfiral.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dupidpff.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fpmoifwh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hgzwbzmp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2taizfxjw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vyohokki.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2lhspxsrd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ueqbhqbh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jzslkwdx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2cvnrucqo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2iwcmdayh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fmymeiif.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cdhyzqgk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2stegowja.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rcmxcolk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lkgrcrub.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2jlfstmky.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2lfhznffb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2btcivxja.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gkzkimqp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2erlkusvl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dyrlgwze.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ctcofwmh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qspbnijb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xvtdiclx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qngyshmc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wxslcjxf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nizkzegn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2csmfbivr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mrahmuud.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zfgxeaee.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2encxhpce.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qlkukbui.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljazvmkh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cbwximzk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kskxsokm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2oszsbnim.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gssnqgtn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2nopumdnb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2eidjjbuk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2yckykcgn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2hzinymzj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjqlppgp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fyupjojo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zwcseezm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yefowlzr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wtkxeiak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzbwcxvw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hpadpxfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhlwrilj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2aijqtgmv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lptvupyl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bexvvddh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ijtoimvo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ckidujrd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2lxpuuuze.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2udrafbkj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2pyqdujqv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qzstkzhw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dauvppeb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jyjnzymn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fmpfhbwt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iuhpermw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2eboploce.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2lxcwpnwf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ccbxcqfe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wfnkeihu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tqmnbngn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2buefawcr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ujkuvovj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dvlmfcuk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2enrptgmc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bctmlszw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vwxyjaox.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vygleuxz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bjavjzsu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2aaqfmtdb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pfqkerbr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2abbnhujj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2blivomrb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qduukwjs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pewxahdg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2okagibdn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hsjranhz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yxyclzhj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fpwxlfhp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hvttbgev.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qkeawcos.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rfqwvjge.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dokfuxjg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mwtrokbb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2akpmefud.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gtcmcfvn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lgucoeda.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ztxpkgmj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gbhlvdtz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jdcqqncn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2azesfjib.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hikvdqel.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xuamnblz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2caagdjdu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hbwtqgcy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pdiwaalb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tvgvkpcp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kiwrfqow.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cbianrzm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bxkfnndv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2khoimmjw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pbclwipm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xvpnivek.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2brdsnxjn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghauiwyw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vjqvxxph.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2flsfsxqw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jrkcrpcp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rbabpxri.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2fqnmutqv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jiitywbd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnpfpamj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2itcpbkud.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2upwshkdp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2avymqruv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bjdblvne.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zobryrcx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2opaurcbk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pjalfpza.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zpjxehxk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xqtginby.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nizbyhkq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qzdfqwet.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ijriamfu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2upogfgzd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2phmjpokf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2iiguamlo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vmaqefuw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2nbjpwazb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2idsjgcef.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wxmrljia.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pjioqmtl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jaqrteks.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lqkgnnlk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dkbfvmet.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ykyfllfd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ioogelep.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xenmkgoi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zlvxsceb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xfwfmgsp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kfwcxpfc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rpumhxtu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2czjbeksl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ldckvilf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zhrmmqno.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2wadmveyp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nglpirms.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pvudwpvp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ipzgmxml.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hlcyfcvx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2uakdyosa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ujpqcgfh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2raxhqsql.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xccbzhcg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2cjqynssa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cjkskgdw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2hqtdcgnj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vwxixkxd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2lsuanuvy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2upsybleo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2owpwwwrh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2upqnwoxn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tfhzlghc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2evloklxr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tgsfblho.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xunhlbnn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2czjmhfnq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hxigwatw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2oulxfqbh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ykgahsbu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cihnoids.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wmrwwvsb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2elmkgqnf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ilssdxig.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2qjgmplyy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qmesidol.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ayxmauqr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2eczwfozg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ohtggfqc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nelqrmez.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lrrfaupc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bvijjfbs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gfreahgz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fvejqkzs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xqmqqchl.html


<!-- 参考信息 -->