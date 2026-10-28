代发 wailian999

CREATE TABLE users (
来源：http://hz.haohaochexian.top/gtbpxuqwvg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhengqikj.top/gtlppnhztc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daxiang520.top/gtqvzyehdp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.havefunace.top/gtlpmpwnhx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenlongwang.top/gtuymjbcxo.html

);
来源：http://hz.jiagoushi.top/gtmshpkwfs.html

[Q02] 创建带外键的表
来源：http://hz.cucudq.cn/gtynrroiku.html

CREATE TABLE orders (
来源：http://hz.52xcode.cn/gtvsfdunmt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtmysdvdkj.html

user_id INT NOT NULL,
来源：http://hz.hammf.cn/gtuedzmqch.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtzuuaksbm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xingfuxueyuan.xyz/gtuluyadmg.html

);
来源：http://hz.yanxiufei.cn/gtfkhmxmlr.html

[Q03] 增加列
来源：http://hz.hywenlv.cn/gthmhrrowt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cucudq.cn/gtqjcyjdty.html

[Q04] 修改列类型
来源：http://hz.hfpthk.cn/gtoepgdonx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shzxlz.cn/gtcawztdgs.html

[Q05] 重命名列
来源：http://hz.hnxiangtu.top/gtsawtqnyp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.quarkkingdee.top/gtaqflfred.html

[Q06] 删除列
来源：http://hz.hammf.cn/gtounaasoo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuxming.cn/gtcvitysbl.html

[Q07] 删除表
来源：http://hz.smart0.xyz/gtufvyohxs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtebgxumtm.html

[Q08] 创建普通索引
来源：http://hz.0kj1m.cn/gtxgirxlpq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtjgzhfahr.html

[Q09] 创建唯一索引
来源：http://hz.zhongyouzk.top/gtriztmoxa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cucudq.cn/gtipswbfeq.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gtmiokrove.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinyuanbaomall.cn/gtmvzuyaxw.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtmmmrhfcu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sxryk.cn/gtemyxzeto.html

[Q12] 插入后取自增 ID
来源：http://hz.kuanghao11.cn/gtvndcvmrs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aizwys.cn/gtzmceyuct.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ywan-chungtsiang.top/gteoenavpa.html

[Q13] 忽略重复插入
来源：http://hz.yvedp.cn/gtdpwzsygz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj202588.top/gtnerzfyhw.html

[Q14] 存在则更新（upsert）
来源：http://hz.shuidangran.top/gtfwqwatmu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.birdmap.top/gtfopmkyfj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gthamnwzcp.html

[Q15] 查询全部
来源：http://hz.zhiwuduotai.top/gtsarjvnez.html

SELECT * FROM users;
来源：http://hz.fzhhl.top/gtvgbmdlex.html

[Q16] 查询指定列
来源：http://hz.ppjwa.cn/gtuidrovmg.html

SELECT id, name FROM users;
来源：http://hz.yongpay.top/gtovsihibu.html

[Q17] 条件查询
来源：http://hz.sweek.top/gtuclkomvu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shanyushiyangkeji.top/gtsahmkkuq.html

[Q18] 模糊匹配
来源：http://hz.c1oappe.top/gtbsopfldd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtrvguwnfc.html

[Q19] 范围查询
来源：http://hz.gaohongyu789.top/gtxzieuxww.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cqqwz.cn/gtxasspqbm.html

[Q20] IN 列表
来源：http://hz.svipenyu.cn/gtmwlxnwmj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinghuilouyu.cn/gtzntogihb.html

[Q21] 空值判断
来源：http://hz.wangdashe.top/gthipkjxub.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xingfuxueyuan.xyz/gtjcirrwjg.html

[Q22] 排序
来源：http://hz.316326.xyz/gtvxcbrjlo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zdqjudy.top/gtffhaqlmo.html

[Q23] 分页
来源：http://hz.sufxvd.cn/gtwkoagabw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yangfankeji.com/gtydwwogev.html

[Q24] 去重
来源：http://hz.cucudq.cn/gtjghgmaqp.html

SELECT DISTINCT city FROM users;
来源：http://hz.svipenyu.cn/gtqmajgyoo.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gtcmdentyj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.birdmap.top/gtmbkfcbhz.html

[Q26] 计数
来源：http://hz.zhiwuduotai.top/gtxylrdqlb.html

SELECT COUNT(*) FROM users;
来源：http://hz.andypj.xyz/gtclhcdnap.html

[Q27] 条件计数
来源：http://hz.guannengcc.top/gtuxwhicyl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ehwqpu.com/gtwszmwzaq.html

[Q28] 求和与平均
来源：http://hz.jinqigfzy.top/gtwrfjwrwk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gturxzteqz.html

[Q29] 最大最小值
来源：http://hz.xuetiantiany.cn/gthqfrduja.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhixingplan.top/gtmarinheo.html

[Q30] 分组统计
来源：http://hz.tianlin.xyz/gtbkmmjbks.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtkulyjeyp.html

[Q31] 分组后过滤
来源：http://hz.pengpengdd.cyou/gttwppqcmj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangkeji.top/gtuokhvwrn.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangtech.top/gtpnccaqfs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtdrtagcfu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnqzz.top/gttmvxmdsd.html

[Q33] 多列分组
来源：http://hz.yj202588.top/gtblyufocd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxinkj.top/gtpvikmwxe.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtqqmbwcig.html

SELECT * FROM (
来源：http://hz.kuanghao11.cn/gtxlverebu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gtmdpffcac.html

) t WHERE rn = 1;
来源：http://hz.hfpthk.cn/gtstfiptly.html

[Q35] 内连接
来源：http://hz.hywenlv.cn/gtyfuozdgj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtcczgjgis.html

[Q36] 左连接
来源：http://hz.xinyue.icu/gtvttatpyw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtzdnpcfwr.html

[Q37] 右连接
来源：http://hz.feifeiyinyue.top/gtqqpqtbju.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258.top/gtvjgjrbws.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtjgylqgje.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pengpengdd.cyou/gtyhjvxipg.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gturdnexpo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cdnleiting.top/gtgfyqksbc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtisctglol.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shzxlz.cn/gtvvfvtdwe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.aizwys.cn/gtqmbrzemf.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gthqsdysdf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ywan-chungtsiang.top/gtbnkvaxij.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tian-w.cn/gtntgafinn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydzc1.top/gtrncpcapo.html

[Q42] 连接条件附加过滤
来源：http://hz.kuanghao11.cn/gtbspoafgl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hongshengwenyu.top/gtokphdimz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yuxming.cn/gtwzjxleok.html

[Q43] 标量子查询
来源：http://hz.haohaochexian.top/gtcegitovn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtyulpzayn.html

[Q44] IN 子查询
来源：http://hz.xuanzx.com/gtujacwjvq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cdnleiting.top/gtfqigbpfj.html

[Q45] EXISTS 判断存在
来源：http://hz.xziqi.cn/gtuatkkbqd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtimxsccma.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgufenzy.top/gtgrxnyzry.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtavieolyr.html

[Q47] 与平均值比较
来源：http://hz.meibo888.top/gtqurkcwdl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.meibo888.top/gtvntkipoi.html

[Q48] CTE 公用表表达式
来源：http://hz.shzxlz.cn/gtyhhdeqce.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xziqi.cn/gtqcyvybqi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.52xcode.cn/gtouzwogaq.html

[Q49] 更新单行
来源：http://hz.cheryme.top/gthewhtplg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.c1oappe.top/gtahishdsp.html

[Q50] 批量更新
来源：http://hz.zhongyouzk.top/gtmjvuttbf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.meibo888.top/gtfmxcvmsf.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtmwlngabi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.birdmap.top/gtkpnrjoye.html

[Q52] 删除指定行
来源：http://hz.ehwqpu.com/gtknaynsrs.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gogol.net.cn/gtdibzdetx.html

[Q53] 按条件删除
来源：http://hz.kuanghao11.cn/gtwwrnxxmh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.kuanghao11.cn/gtkeovdfuh.html

[Q54] 清空表
来源：http://hz.9152youxi.cn/gtatarigwg.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigfzy.top/gtruxkaeqg.html

[Q55] 排名（并列占位）
来源：http://hz.guannengcc.top/gtiogxefnm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hywenlv.cn/gtkpinmyhu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cdnleiting.top/gtoijgtvlz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hfpthk.cn/gtipcejcqq.html

[Q57] 行号
来源：http://hz.yuxming.cn/gtfrhpbesk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ybcxt.top/gttrhdoncv.html

[Q58] 累计求和
来源：http://hz.hysaishi.cn/gtybxfgxdj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shzxlz.cn/gtxkslhdpn.html

[Q59] 分组内累计
来源：http://hz.tian-w.cn/gtyusaxinh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yueranfly.top/gtdkxkfkqj.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhaomingkeji.xyz/gtadcbbzqa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tianlin.xyz/gtbkjveddw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daxiang520.top/gthgfrtjrb.html

[Q61] 移动平均
来源：http://hz.9152youxi.cn/gtcfpzgfjr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinqigufen.top/gtjhshebdp.html

[Q62] 分组占比
来源：http://hz.c1oappe.top/gtxugvptjw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtsseitqys.html

[Q63] 开启事务
来源：http://hz.birdmap.top/gtpmxeskfc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenlongwang.top/gtxpytrqtl.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtmnphmlam.html

COMMIT;
来源：http://hz.jinqigfzy.top/gtgcgryepg.html

[Q65] 回滚事务
来源：http://hz.shanyushiyangkeji.top/gtcunkfyok.html

ROLLBACK;
来源：http://hz.sysykeji.top/gtclslfzvs.html

[Q66] 行锁查询
来源：http://hz.smart0.xyz/gtfodsslta.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.havefunace.top/gtgvbsxqgl.html

[Q67] 设置隔离级别
来源：http://hz.ywan-chungtsiang.top/gtzvykegkp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nwbrower.top/gthmhyzugj.html

[Q68] 保存点
来源：http://hz.sufxvd.cn/gtpdioddua.html

SAVEPOINT sp1;
来源：http://hz.gogol.net.cn/gtjeskhtip.html

ROLLBACK TO sp1;
来源：http://hz.yuanzhike.top/gtpzwcmurx.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gtuvfpmivp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.meibo888.top/gtqoodxryj.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gttlkjicnf.html

ANALYZE TABLE users;
来源：http://hz.mhx1999.top/gtjddcgbsb.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gtmkrygjmm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.birdmap.top/gtqniurfog.html

[Q72] 查看索引
来源：http://hz.snrcjt.cn/gtytyunyip.html

SHOW INDEX FROM users;
来源：http://hz.ehwqpu.com/gtvalmgijg.html

[Q73] 查看表状态
来源：http://hz.chenjidiqi.icu/gtytzvuysi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhixingplan.top/gtviyrrxdi.html

[Q74] 强制使用索引
来源：http://hz.jinqigfzy.top/gtnjocepdw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtqlpltpaa.html

[Q75] 日期格式化
来源：http://hz.hammf.cn/gtmuqmoiun.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gogol.net.cn/gttwbcwuhg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dashuyun.cn/gtwzvxlrtn.html

[Q76] 按天统计
来源：http://hz.zhoulong.xyz/gtdjyxnlwt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yueranfly.top/gtyvrbiieu.html

[Q77] 时间加减
来源：http://hz.hongshengwenyu.top/gtwfjfocix.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jianghu66.top/gtjiawczqi.html

[Q78] 当前时间
来源：http://hz.sweek.top/gtxplcjgaw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangkeji.top/gtbfnefiey.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangtech.top/gtkddyqcyv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenjidiqi.icu/gtgdefzyqt.html

[Q80] 字符串截取
来源：http://hz.hongshengwenyu.top/gthatunrmr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gzhubu.top/gtpnovuozu.html

[Q81] 字符串替换
来源：http://hz.wangdashe.top/gtuwoaxswu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shzxlz.cn/gtlsdtdxaz.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtbxjsifom.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tanke756.top/gtppwoeowh.html

[Q83] 大小写转换
来源：http://hz.chenzaomai.com/gtqiiiovrf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtxwicupxw.html

[Q84] 去除首尾空格
来源：http://hz.quarkkingdee.top/gtgzndapgf.html

SELECT TRIM(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtcntwkasq.html

[Q85] 数值取整
来源：http://hz.kuanghao11.cn/gttalkpeqv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhijiandao.cn/gtrdmkzkmr.html

[Q86] 读取 JSON 字段
来源：http://hz.aibaodan.cn/gtumwxmwtv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gtejmuhmpw.html

[Q87] JSON 字段做条件
来源：http://hz.316326.xyz/gtbalcuzkn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.birdmap.top/gtbwulhbag.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gtmtqwmbya.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.c1oappe.top/gtvkpdpdid.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.vqdsnc.cn/gtntiljwcs.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gtuamterlf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuanzhike.top/gtkcconrct.html

[Q90] 生成序号列
来源：http://hz.tian-w.cn/gtoihermyj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtyznwamau.html

================================================================================
来源：http://hz.yvedp.cn/gtfakusqvk.html

R. Bash 专题
来源：http://hz.yj20258888.top/gtiipkkgrs.html

================================================================================
来源：http://hz.jianghu66.top/gtywnqyfyn.html

[R01] shebang 与严格模式
来源：http://hz.quarkkingdee.top/gtildxzgnp.html

#!/usr/bin/env bash
来源：http://hz.zhoulong.xyz/gtlrwgsxrw.html

set -euo pipefail
来源：http://hz.cqqwz.cn/gtefwmgbyj.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtuxzgyfgi.html

name="Tom"; echo "$name"
来源：http://hz.ehwqpu.com/gtusskgbrt.html

[R03] 只读变量
来源：http://hz.ydzc1.top/gtuoigbzng.html

readonly PI=3.14
来源：http://hz.cdnleiting.top/gtinbymgty.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gttoanzede.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dianchejie.cn/gtmqeyimfj.html

[R05] 参数默认值
来源：http://hz.nanxinkj.top/gtnhteptlx.html

name="${1:-default}"
来源：http://hz.cucudq.cn/gtlxmvygul.html

[R06] 判断命令是否存在
来源：http://hz.gaohongyu789.top/gtqgyutoqt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtkqqwdtcd.html

[R07] if 判断文件
来源：http://hz.sufxvd.cn/gthsdhszll.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cqqwz.cn/gtvjcqfyrl.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtxdgwzsld.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtfzuclotu.html

[R09] 字符串比较
来源：http://hz.gzhubu.top/gtbujfmygb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxuanxn.top/gtliseuqqe.html

[R10] 正则匹配
来源：http://hz.jianghu66.top/gtjzuliwuz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jiagoushi.top/gtjpeudavj.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtdivogptp.html

case "$1" in
来源：http://hz.hnxiangtu.top/gtzihxubgd.html

start) echo "启动" ;;
来源：http://hz.hywenlv.cn/gtnliqsvjy.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtywiqqril.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gtgzolxeoy.html

esac
来源：http://hz.ivvv.top/gtgiocubjr.html

[R12] for 遍历文件
来源：http://hz.iojbl.cn/gtlwbfkejb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhixingplan.top/gtjnfqrwtu.html

[R13] for 计数循环
来源：http://hz.hnqzz.top/gtmestxnvq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gzhubu.top/gtikosfhtu.html

[R14] C 风格 for
来源：http://hz.sufxvd.cn/gtvwfmzaxh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yvedp.cn/gtojnfdibd.html

[R15] while 逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtkupfiykk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ivvv.top/gtbuvajnis.html

[R16] until 等待条件
来源：http://hz.dashuyun.cn/gtkstnfspt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhaomingkeji.xyz/gtqvflmtyu.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gtiewrihew.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tian-w.cn/gtewrmsirp.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gtxhksfsgx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cashguo.top/gtyvfzxgbw.html

[R19] 数组长度
来源：http://hz.yuanzhike.top/gtrogykaew.html

echo "${#arr[@]}"
来源：http://hz.hnqzz.top/gtuesvddei.html

[R20] 关联数组（字典）
来源：http://hz.zhijiandao.cn/gtepgkckcj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ivvv.top/gtbvhyfeop.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtkphbzhop.html

echo "${#s}"
来源：http://hz.316326.xyz/gtmvqujnbm.html

[R22] 截取子串
来源：http://hz.vqdsnc.cn/gttrjelbwv.html

echo "${s:0:5}"
来源：http://hz.tian-w.cn/gtfdovqmzg.html

[R23] 字符串替换
来源：http://hz.zhixingplan.top/gtqvrtcloe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.iojbl.cn/gtiialrugb.html

[R24] 大小写转换
来源：http://hz.hysaishi.cn/gtpglzktea.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.snrcjt.cn/gtnfgprnwo.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnxiangtu.top/gtbmmyqlwu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gogol.net.cn/gtmqhreqwy.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gtkbwvyxzh.html

now=$(date +%F); echo "$now"
来源：http://hz.hysaishi.cn/gtcbzvselw.html

[R27] 算术展开
来源：http://hz.zycfv.cn/gtiotndzxs.html

echo $((1 + 2 * 3))
来源：http://hz.daxiang520.top/gtoytnlvwr.html

[R28] 浮点运算
来源：http://hz.cqqwz.cn/gtzabgambn.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtiqcaxuqz.html

[R29] 定义函数
来源：http://hz.hfpthk.cn/gthotftiek.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jlsjyb.cn/gtjkkvciqg.html

[R30] 函数返回状态码
来源：http://hz.snrcjt.cn/gtyrjkeqno.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhaomingkeji.xyz/gtozymosow.html

[R31] 局部变量
来源：http://hz.svipenyu.cn/gtyeeumaas.html

f() { local x=1; echo "$x"; }
来源：http://hz.52xcode.cn/gtjnrpsqrx.html

[R32] 参数个数校验
来源：http://hz.bjfxy.top/gtesqtjuyv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuxming.cn/gtreybpows.html

[R33] 捕获错误并提示行号
来源：http://hz.xziqi.cn/gthvgjpknn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hnqzz.top/gtafgttgfj.html

[R34] 退出时清理
来源：http://hz.jlsjyb.cn/gtwmrvyxor.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtnsfhiqsm.html

[R35] 后台执行并等待
来源：http://hz.fzhhl.top/gtuhslfbit.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangshuangyany.cn/gtyjaykpfg.html

[R36] 并发执行多个任务
来源：http://hz.daria6918.cn/gtaxvlotos.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxuanxn.top/gtszqywcxn.html

[R37] 把输出赋给变量
来源：http://hz.hywenlv.cn/gtuixyjmqu.html

files=$(ls -1)
来源：http://hz.jlsjyb.cn/gtamujitfb.html

[R38] 管道串联
来源：http://hz.yongpay.top/gtrkvohrwv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtlejrznex.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangkeji.top/gtirrkbrst.html

cmd > out.log 2>&1
来源：http://hz.redwolf501.top/gtzeqkerhh.html

[R40] 追加写日志
来源：http://hz.nanxuanxn.top/gtithwcivx.html

echo "log" >> out.log
来源：http://hz.52xcode.cn/gtzjyvrwxn.html

[R41] 丢弃输出
来源：http://hz.yj20258.top/gtjfmbhinw.html

cmd >/dev/null 2>&1
来源：http://hz.hnxiangtu.top/gtayiiyiut.html

[R42] 输入重定向
来源：http://hz.jinqigufen.top/gtydjhdbck.html

wc -l < a.txt
来源：http://hz.bjfxy.top/gtvranqaos.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtswingsxg.html

find . -name "*.log" -type f
来源：http://hz.yonumen.top/gtrkfuytrt.html

[R44] 按修改时间查找
来源：http://hz.xinyue.icu/gtufuqhqht.html

find . -mtime -7 -type f
来源：http://hz.guowangkeji.top/gtcpptflbs.html

[R45] 批量删除
来源：http://hz.ppjwa.cn/gtcwhhlvru.html


<!-- 参考信息 -->