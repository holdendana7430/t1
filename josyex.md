代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xlakykmc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bpefwiko.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wrfwxgpn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2oaqewoog.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2okwevpco.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gbvgqurh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wjdeucoq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2yaknxrno.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cqvrucvt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mlixzwmo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2sspxjqdi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2viappqcu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zzdbnqub.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2enfzefnf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wtjuusem.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2enqlluqc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2hvceukuz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vxaqlcoq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klarkalb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ijogmpsl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2upjqqzjo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2appkypok.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kznfciud.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fvpsjgbp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yzrdcddp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uvskbnvs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uofvcvrc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ijajdgwi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dqxduozo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yuxbtqqv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wlqvkzzi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2sthtpufw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wtlceogl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jctiawww.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gdvmftnt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2agshhcdo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qgukkibt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wdiwsulk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uuviwqmu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2aragwxek.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2znwsqoxq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zihqawld.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2esooaptj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2viymlobm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rjgiysiv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nzaqddxd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xmtmwfug.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2geehzjyl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2mbwmyxkp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xbootuwp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dmgijcsl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2amxwbflv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2apfekquo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2eimdkfww.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2dvfherqp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bgtkotdh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hmnejffd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2awcxncjq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qxfukzgw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xwfbnfxw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gifmkaau.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2czuvjeoe.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wapzluxp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2aegbthgg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ahosoaow.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2obvjfgfm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2iocxtwvi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cxscznrp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uqpiczwg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2whyanyvs.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jsebomgo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2uimrxalf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2aapvovom.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2oisltmxi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bdhdwkfm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gnbsjcbs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bxpszkev.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2awphchll.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uvgakxff.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2iueksqbo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mqyvrmne.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2fkiirurs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mtblnodo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2bgmjvred.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gjelhfvg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2syamayaj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gzuryogt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lztnigei.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2btwhchmf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jxqmdhat.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2motszlke.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zapyosho.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2simnqdub.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2leuqpstf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aioblxyb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pkgmesut.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nzscbfyb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rywapgsq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lipjlgcb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cwohpwsn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2devnhgak.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nxvmftys.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2tcemetdc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zxdtlzbf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2izbwmgke.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fpaohupp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kqqderrs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ptahckpg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2oitanbyc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2scqyarnr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2zfswzfvk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ffhyhcgj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2cvnjkwpd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pceaqcgj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2typdkhtp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lugskzsk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ugubemdt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lkgucwor.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2aojvgsog.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pociypui.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2scxrwomo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2krfydpbv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2idozudtw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gkqcthyc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pastsepj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dayjfbpn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ivzunmqq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2lgysnfmu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2izdrdyjx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xrgvwtbr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2awarmjup.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2qtlhbbel.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ovqjgzui.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yotqscep.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ywayfuiq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hkzmegjg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2zmocbrbn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2enyghyre.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cfeddhxc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gejrrqfc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qtjszaik.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bojwmcrq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2elwoxzaa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2efivcjzd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kpknscmb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zuccapxg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bnxaqjls.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zropktkr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2azdjbqph.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zjfhemrb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mgmgniye.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2xqijqpeo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vaukfisr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2odsluxcg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2qizpbzmf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2cwnlllvr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gbemdxgo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ubfnmmsd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qrzcrrlf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2reeoqkre.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2awarhqhu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2eeuztmve.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xqtxiacd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2soqsbzgt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qooztpjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwpwsygq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2priehadp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mokrgypa.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2bfcnkmlw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pqbwvlqp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2yhdildnb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ffinnxyw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hkqkcntg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2oghdlhmy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zrfmisnx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2picuzywx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tqzmdzoq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fpcorrwe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2apcqlpgh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uwrfnaix.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eqxedbtq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2drzaofry.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vhpjuvep.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wznymvjv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2urriveja.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jkkqurhc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nmrxmrze.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2csbnhlhq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2yqkbkuqu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hmegnedu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bcejfmjv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2sijvswpe.html

esac
来源：http://www.52xcode.cn/Article/details/gt2abywnsym.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2woqrxaks.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ytvtvsba.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2sibymfle.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ltwmfsvb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ysepsebq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fgpbjegp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bpvmsqtd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qznihxpu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mwaqmtao.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tznmyqwj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2oklxkqgl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ekkuqkku.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2iukusaoh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wcitaacr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cocgocrx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2amrbgfef.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yowjjckz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jyexcsib.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uyxjxjxb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kndkklwu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2btqgpwyl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ipmdfakd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lvnfkiqm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dypmqljt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lurqrbwz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2erppbogp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2blepbvwi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ueeoincd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2lzzwhfos.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2yzjijaxh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hgivdwys.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xrdcqlyi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ekkqqjke.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2uhlryxth.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uzdpueeh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ohwrdsak.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fxrpimke.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lwisyqfg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2thaqvtmk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afavcqpz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2skwxvpfh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2petfqwef.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2exbqukfw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kdyabgva.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2prpzeege.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2btrcgcyd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qplsaenb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tsxnswwr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2aakujzxb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2rboclrpi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yeiudjgb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2jvfunqap.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mxwkhwrn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gzqgmmla.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zwoifvzl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wnfytgyl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bxtjhryz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2yllpvjrc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kvurxmos.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vtcuhfoq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bxsfcbnp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qowgyjcg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wocerquo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2aqlzjvnd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2svpmzkeb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2avqnwquz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vbfbcdeu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xgpjvbpm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2obbqwevs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2foamnfcv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yodjjhvp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zspmexkn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tkmhyeuy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2etlzavvq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jgxwbcrx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ujqezhct.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2kcmnrqua.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2czdaqonn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gkzddrvn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ldwkvnpz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2nixsdwrg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iesesvfu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2gbctybaa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2drfawtbu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lqvfhzfh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zylxfver.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xnkuzkdd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ogfugcui.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qivybdcz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qsxlqjad.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2uqqorfhr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yfsvwoew.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2glogpodg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2edkwrdgf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kzvoucxn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2obxzsqnf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aiuhgivo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qoqrhjpf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2dlcnhtzl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gtsyinje.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nugtqedl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cbamkolr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2neisorcj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2gwbmxpch.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ipygetdy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cpchyuyv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2wvxnuarj.html


<!-- 参考信息 -->