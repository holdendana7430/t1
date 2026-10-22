代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bebkyibz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xqlfcxln.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2epnbpkar.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lzgksqzz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sxeoezlt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xndentas.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ndwaebem.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cxwhpjoi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jksfbjnn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bkynkwja.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yeoowedd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mulblucl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ifegierc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wgiwefao.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wuelmybo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2nptghzrs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jbmfvpkg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ypasjfjk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uqzrbrry.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nhoihnqj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zmxiydmd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ftpkhlhn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zwxsxvmn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2olzpckaq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dgzvlfjr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lfyzanxx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yvivhbyw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rkvmrylw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lvjnfndl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tqantkgr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mpxzsfju.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2tfzfqtpd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2etidfrmg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tikuucin.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wdojnyps.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2lnbahvhk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2cutnjqin.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qmkhsstp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2twdvmwik.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2avioaief.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mggkwpoz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2whpnwbgv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2uxyguydh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oamrbxlo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qnhqurvb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bhpwjwmv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2veuerwet.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2grvzwmci.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2sljwrlwr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kcrwphhf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mjofobii.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ylwkrotw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vmvzupfq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2uurgkxyg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rnlxkdsp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dqhjhcuc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2onbifvsc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2dsqowkpt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2smfhmrjn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rlzgyhgj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lpmzolwj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xtykowhz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fgcsojsl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2brruvgqf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2btcglklh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2msfsjkqe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ghifkbic.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ozgndthb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qmckdhfg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nvypckjf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jrmbzojs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zkctdsfy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dompbwxv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ccfjupqn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pkuxfrlu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ivemsasz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wzwmzamr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fpesflbg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vkbitaht.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zcxhdzqq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tkbmxbpy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vyagbjrk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jilscvzs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dkvsgnel.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cgtduhje.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ucsziyvu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qzrsmupu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zfmlmtfk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wyhfpvzk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lwrhtxvj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pyyxmmqq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2igvzlaux.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dljqzhas.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sswsygbv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tbluvscu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2aggbycwy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gcuujuad.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2egxrdonm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tcqszaaj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2smdorjqu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wlsdlmet.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lepreufq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gdcdqgbv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2buwcrfwm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2rwfubhop.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tliingrv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2vfzmohcw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2nycvmloi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2zeiegehk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2nledxbgr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ytqkhtdd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qrzvfxky.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vntovmru.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wyisyzng.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2fsobsqmv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zjhjmwub.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ivqhtafz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ntrnswna.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pxcubdye.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bgbodxmr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mdfoayeu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ehddfhoc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2kxaxubve.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2urrszspd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aypvxgez.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xsfrjdiu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tkyrhzpo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tygvayav.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kccjwfho.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nocsxhva.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ppatalyk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rrwipqth.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2isynwhdy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dayjejng.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mhkcgzll.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2txhtkjaz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2otvailbu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ecmouvic.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dgebyqjj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vgzmfjsw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mpkkwnap.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uuibrqbo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2beflwrvi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2azricsqn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lfklafac.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dnucbssc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2whvpagis.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yhhqubjg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yxluayyn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vnlwcmjq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fuzszclc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zijcngoc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ntbcunee.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2bzxfnzsm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xzutzmmv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ngspgidg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ttbmefhk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ccglcmsb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zysqhtok.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2uldinvrr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2blbgalgi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2szhvgroo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kqqhvahw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwdstfbv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bajjttxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erwsnyos.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2yboypvjx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kepivjcq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ftmkqooo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yqzfmkcw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lbsakwko.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kppmixlx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zdfqfnmz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2pkpvbscd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zqxuiqig.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2fgkidikz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpdlvudh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rkklqjqs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfdehvbh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jywbrrxl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2nhupxagd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mzwsqdxm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2titgvpay.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pznvqvoj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2djtjcerw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cblwjmow.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2pynkntvf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jnxlnmpn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bdbuaaxt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nycugchb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2auynfzut.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2veioysya.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ezwtsxon.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhoihxfw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2shnegzbw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ypefeqgz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dnsoxcaw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2pkexrcuz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ermjhvit.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fehujcoj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wopylpgu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2yuwlgbhi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wummooqx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lpvqpdwo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2axrqhftt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2buclnhla.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kbwhjeru.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xfdpikxc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwnszdms.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2splpaqtx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mwytjtgv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dzhbgoak.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vibqrxnp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ucedoson.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tvqtlins.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fktsigdu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lpdatbju.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zzujvdwi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pahhkctj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ameeencn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zazoxvap.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cezoqvhi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wqxosbwf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dshuefpr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2coiuuyzi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2chykvqaf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xzphsawl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmwiarpy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2omholsof.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2frngdwbb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mtlfygfm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2idytssey.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajjbekgz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dqafkcmu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmqsrpxw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qxjiljeo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2micsbnnq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vgopkawq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2unpljmfj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2avuhvldk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2egkknaaw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dtxqjzin.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gswenzkk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymogxmyp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2pzbiejko.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jacxrmpo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2pobjzhng.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mfbyaewu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vrdcxjhn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qlejisoo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iighfmzy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xddqqsfs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2auggxpli.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nvzuslod.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dtrmdgul.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2otvplxxk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kaawudqh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2feuawbng.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oacfbwlq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qdnmgono.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ofunnczo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tplkbpdd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2odaqhlyf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2oshdtbip.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tcdksfps.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2sxzlxurb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2neygsuqw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ktzprqhl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ezfglygi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hinnkupp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2urssbpsb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sztjfrks.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2uldrdvxn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2doiircfo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oiiwtxmy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ulfdidpy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gmpltahu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2towhahva.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ccjfsvjc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xjzflyqh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2euntxgkq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zkefwkbw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2iedryvpk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jlqkmznh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2byuhjkqp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2owpvgvxn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vsliztpv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rlcgkdem.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ywxjoahv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lxfyusdw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2kcznztgv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mlbhsmdm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2touygohy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2djwxkgrd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mavmowsi.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2zvjrihsx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bfveffcz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ymnoyvar.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2khrilhfl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2expgepaj.html


<!-- 参考信息 -->