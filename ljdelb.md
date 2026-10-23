代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ijpjldmi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tokmdpap.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ljwrdith.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nixnnhyc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3aidcsylk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wpwfrdua.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3jqhxojfc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3eonejgfo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mgzinjgy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mbrbybko.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3oaazbddk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3bssdhchx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3jmvznixp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tdwbfbzk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgvnbvqg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zfezjubh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ezgmpetf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zazuuidq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtwlwzuv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lmgzqpdw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yehfecvh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3lfkdyrbw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rzojyvgh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uwzulfai.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qntariqe.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3prcgtmyq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rkogtdvx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pqwnincz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qygzonvl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wmlbxxaw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iacldyjz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3tcbnjdyb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3osxbogmj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3pdsslpfm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3qtcsaouo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3smcsjdex.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3yuxodtpe.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zwxplvfl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3plkwwprp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qfilcsyn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jwlwiqbx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uojzcpfn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fzqahtfs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3eievdonw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xhitzwia.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wppiukum.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rlevodmw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ospnsakl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mvuzuwiy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3iafitrpw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3crmsbyll.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dxpmofwy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3eouebprs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3sxxopvjm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ipogyuny.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pwgcqbgo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3neerkrza.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3rtcfxmlg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zaubpjtu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zediahjg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3srfcrqod.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xqzbyirp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xqdcmhus.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3eyqfhytx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zburienv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3aceowuns.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kfmchhnp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ulsnhlho.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ynsnzquy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qrukkyvi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zfpcvixz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3piikxrkm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3odqrinxj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3novouyjl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dgpboauc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3uuzsvbbj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3esxycpwp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lxyvsnpm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xinrhuqz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xieioobz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kytvjybi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3htnujbgs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ihvvukvw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3eypqmlfm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3srxwfwqv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fkbcbvvq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mtovgxyi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3iouhvwtx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mcaclcpy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3lgokdqjn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3abxtdgas.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3belsuggc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fzylezxw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3brhuxilz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wdcpenph.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fonqzsid.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3pxrcsohp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cxhjsqxc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3kovihchw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vuavglnw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3aulmwweu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yanhuvsx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3kmanhbcw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3osnkclzb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vulaxwmz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gmkhidwp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jfllhyrx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3dpsaumec.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sooymnwh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hhrawych.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qifemxdv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ffqggovu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3psnnbwxu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3rxcywxvk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wlwmixdd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ykahfqwe.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3isswdltm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3tbrtzxmm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3cjoxpkta.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3oxuhgtxa.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rxorptwj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3solwgyvn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3qavdwxup.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qkxgtqdj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nufbcpyt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3doringas.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ipeceopv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kxftccug.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fnbrltzx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3aqbkafza.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tvsmxwbb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3iaxwjptb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3uejvdwmj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3emsihpfk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gzzlnpza.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wnveyzfv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bjejwzvd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3toktbrsy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dygokwyc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3scxckwry.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3hgmignzc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stziuyco.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3afzuksri.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oizhcheo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hvtrhjxn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3akwklvmm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fnmkabhx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3djnjeuud.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xicwrmgd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3zumpoqmw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3qfmpkwpn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3yaizewza.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zcqwhchg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qtviinpb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lnxihybv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qfgnrzmr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hxihwouj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3gjnyvjfb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rvwnybyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzgbogxr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bdkggeih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjimydoa.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gbnfgdfq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pnmgaeyl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3oxusuakg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3llxbnpdl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wxkjqdhh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3narotkuu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3oowdpngq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ecbfzajt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3cbzatltk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zzibipew.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fstaahjv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gckgsbvr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3orxphprs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhbfeogx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3chhjbbau.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3faaloxbx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gczdqxdq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hhwtvfci.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ubbmqfat.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wuepcdbp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vqisnpha.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gcdoldkt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kalebfud.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rsaxyhbq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zfqmovrd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ynvpaorc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xgmhzjto.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3avrmuecm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mqlszoau.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zjurhvib.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dikouovp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wpkukksg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ecujlmde.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ofbduhjz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qmiwoazf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jseysqfl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3muookkjo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3emehvixj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3asiqoixf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ryohnvgj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xzplqetc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ojawrtaf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xphmebqo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3osqndudz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3okyxunvx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wlntvfii.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fntnsmpx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hglxsxbr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aawbwurz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fanzjpxs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3miukfdrb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dildbfja.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tptharhn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ygxlaeeo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3odgqjicb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vnnenbeo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gsdlngfj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3gmafeivh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rslvkuhu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jvfxdfna.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3tkumeipy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbhbmxvb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3euccwtqa.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3sjowiire.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3yrmxmqso.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbjmihby.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mkdfootv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ihuylpcq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fkqyazhj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mikylfiz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ryrqucpw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pqgotvqm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tpijuykm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mztocpee.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zcuswhsk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xiglqfso.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lnxgemge.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cosmyzpp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdvheugp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3yezyxsso.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dljsxusl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rjhpxoin.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ensxlhha.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3anbzkvsb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uprcxdga.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3beyewpjv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xcvshrib.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3okoqzsee.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3tjucylwv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pcegppal.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3onxwrcyh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ptqoombg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tcotljnj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3udidyzgb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wsjhlbhq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jrmnnloi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wpjygodu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lcmxjqjk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3itmfhsjb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qegnvhfy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qxwhcldy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jbczcvkm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xbhuokfs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cnpnnlwe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dbclcbav.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ccsgegnf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vixmnoht.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3oeszjeqb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fivvurtj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3imtlagpw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hsyrbxxh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybwcneud.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nggyvfxt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jxnfcniu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rozuthqp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xrwnguwx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cjqqgoyu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3outhpxsv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3imrugmil.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hbmdgpdr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bswxmkgw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3sabfthvt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zhoxebyj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wqscadic.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iezkftqb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bturxatn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qjzlcxxe.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jsyohuqq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3wbmxnrph.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3seaqhcmu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3srdxiypz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3uvickpxb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fuxzedky.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zokjshuq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zcuzeckc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mgdaozbl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ycfvunae.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wenabwwk.html


<!-- 参考信息 -->