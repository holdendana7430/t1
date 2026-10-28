代发 wailian999

CREATE TABLE users (
来源：http://hz.sufxvd.cn/gtzknnuscu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangtech.top/gtreyvbnbt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hywenlv.cn/gttilqeauc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.daxiang520.top/gtqaxossst.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fengsongda.top/gtnpghwqwx.html

);
来源：http://hz.jyoumei.cn/gtfnulmlyj.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangkeji.top/gtoivqkjaa.html

CREATE TABLE orders (
来源：http://hz.yangfankeji.com/gtagccvmqq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtepulffpz.html

user_id INT NOT NULL,
来源：http://hz.yj202588.top/gtlmktfdiu.html

amount DECIMAL(10, 2),
来源：http://hz.yanxiufei.cn/gteerhzggt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.316326.xyz/gtniichzwe.html

);
来源：http://hz.zhixingplan.top/gturgbtoxn.html

[Q03] 增加列
来源：http://hz.mhx1999.top/gtldrnholz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cashguo.top/gtwxeswsdr.html

[Q04] 修改列类型
来源：http://hz.9152youxi.cn/gtgkbqubnc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tian-w.cn/gtbhkzdano.html

[Q05] 重命名列
来源：http://hz.shanyushiyangkeji.top/gteubjlade.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj202588.top/gtplfxiezb.html

[Q06] 删除列
来源：http://hz.kuanghao11.cn/gtdkutelem.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhoulong.xyz/gtdgnhyivu.html

[Q07] 删除表
来源：http://hz.0kj1m.cn/gtihjyojac.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtselcrels.html

[Q08] 创建普通索引
来源：http://hz.jinqigfzy.top/gtsyzxodfc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuanzx.com/gtxeprmfzj.html

[Q09] 创建唯一索引
来源：http://hz.guowangkeji.top/gtbrvimaom.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuxming.cn/gtncomagtr.html

[Q10] 插入单行
来源：http://hz.wangdashe.top/gtsoctwfyh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydzc1.top/gtgmmgoqaa.html

[Q11] 一次插入多行
来源：http://hz.yangfankeji.com/gtgikwnmpi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hammf.cn/gtkzgacaix.html

[Q12] 插入后取自增 ID
来源：http://hz.chenjidiqi.icu/gtcmabddnm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.meibo888.top/gtdzuoafab.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ywan-chungtsiang.top/gtinhzpxxm.html

[Q13] 忽略重复插入
来源：http://hz.hywenlv.cn/gtmhbecmuo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigufen.top/gtcgdkjjmd.html

[Q14] 存在则更新（upsert）
来源：http://hz.ydzc1.top/gtshipaskq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.aibaodan.cn/gtewpjqdtx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hywenlv.cn/gtnbodczah.html

[Q15] 查询全部
来源：http://hz.havefunace.top/gtjvccvbge.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gthvakklsn.html

[Q16] 查询指定列
来源：http://hz.zhengqikj.top/gtfufylqhi.html

SELECT id, name FROM users;
来源：http://hz.guowangkeji.top/gtvwukrivr.html

[Q17] 条件查询
来源：http://hz.andypj.xyz/gthaynlyyq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yvedp.cn/gtfwixofpx.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtcluhatqz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fzhhl.top/gtalqnaqmc.html

[Q19] 范围查询
来源：http://hz.gzhubu.top/gttlzohaly.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuanzx.com/gtvgabezgk.html

[Q20] IN 列表
来源：http://hz.xuetiantiany.cn/gtrzpgfjun.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhoulong.xyz/gthjxduqbu.html

[Q21] 空值判断
来源：http://hz.nanxinkj.top/gtynrwzrrh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ehwqpu.com/gttguikqyj.html

[Q22] 排序
来源：http://hz.haohaochexian.top/gtzdupahfs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nwbrower.top/gttiuucumv.html

[Q23] 分页
来源：http://hz.guowangkeji.top/gtqbgmunup.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zycfv.cn/gthsfhgkpv.html

[Q24] 去重
来源：http://hz.zhixingplan.top/gtqtuctcue.html

SELECT DISTINCT city FROM users;
来源：http://hz.hfpthk.cn/gtyleqygae.html

[Q25] 只取前 N 条
来源：http://hz.cqqwz.cn/gtfxcicyhm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gtyrjtzlay.html

[Q26] 计数
来源：http://hz.gogol.net.cn/gttxvegoxa.html

SELECT COUNT(*) FROM users;
来源：http://hz.xylfe.cn/gtkewotfwn.html

[Q27] 条件计数
来源：http://hz.xylfe.cn/gtmtqundlf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zycfv.cn/gtbcrwbfit.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtjzicnxoo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dashuyun.cn/gtsgboevgg.html

[Q29] 最大最小值
来源：http://hz.guannengcc.top/gtmivatpui.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.52xcode.cn/gtvtbzwmxs.html

[Q30] 分组统计
来源：http://hz.wangdashe.top/gttoqkoxpg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtympzgrrx.html

[Q31] 分组后过滤
来源：http://hz.wangdashe.top/gtsycnakgi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daxiang520.top/gtfcfdkdxa.html

[Q32] 分组拼接字符串
来源：http://hz.chenlongwang.top/gtbgsoqrti.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtxvunantg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cashguo.top/gtkvusssuu.html

[Q33] 多列分组
来源：http://hz.cqqwz.cn/gteroxtavp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtjpvuvmsk.html

[Q34] 每组取第一条
来源：http://hz.ydzc1.top/gtqjwlmeja.html

SELECT * FROM (
来源：http://hz.zycfv.cn/gtxpkzwvyk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sxryk.cn/gtdqugvfpk.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangkeji.top/gtutrqjnzu.html

[Q35] 内连接
来源：http://hz.wangdashe.top/gtzcrhensi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtrcxuwvqz.html

[Q36] 左连接
来源：http://hz.cheryme.top/gtzbwudqdp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtijaaoaxy.html

[Q37] 右连接
来源：http://hz.guowangkeji.top/gtaprqiirq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuanzx.com/gtirigtpmh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xylfe.cn/gtlieqsyxs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gtctovzrrg.html

[Q39] 自连接（查上下级）
来源：http://hz.yvedp.cn/gtxpttpiag.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ivvv.top/gtufsluwwg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtxjpoatsl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.9152youxi.cn/gtvdffvdrl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgufenzy.top/gtiuzjofsd.html

[Q41] 多表连接
来源：http://hz.xuanzx.com/gtzoxfnewr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.mhx1999.top/gtzwpuqnbj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gtiqokcixl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.andypj.xyz/gtihwrhzsz.html

[Q42] 连接条件附加过滤
来源：http://hz.zhiwuduotai.top/gtwtwzwjzs.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhoulong.xyz/gtuwpewutd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guowangkeji.top/gtnjlbvigg.html

[Q43] 标量子查询
来源：http://hz.jinghuilouyu.cn/gtjfaqjvcf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.quarkkingdee.top/gtuwhqqlzk.html

[Q44] IN 子查询
来源：http://hz.andypj.xyz/gtaqrcspuv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pycfn.com/gtutbsrksf.html

[Q45] EXISTS 判断存在
来源：http://hz.yuxming.cn/gtmgszwwvz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtdrvmoiqp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shuidangran.top/gtozufqgpu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtfebxwfng.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtzeemzokr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xuanzx.com/gtteqcehwy.html

[Q48] CTE 公用表表达式
来源：http://hz.zdqjudy.top/gtrfjawyti.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.c1oappe.top/gtkjskgmzq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jyoumei.cn/gtlmfwbgap.html

[Q49] 更新单行
来源：http://hz.jqgfzy.top/gtaqxgfppj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dianchejie.cn/gtznmrbjex.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtqndwywmn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yangfankeji.com/gtjcgwbhgg.html

[Q51] 用子查询更新
来源：http://hz.shuidangran.top/gtmieoookr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cashguo.top/gtbgdfamxy.html

[Q52] 删除指定行
来源：http://hz.nanxinkj.top/gtwbmunqxw.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj202588.top/gtrwqlqogo.html

[Q53] 按条件删除
来源：http://hz.52xcode.cn/gtafhoiufp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cucudq.cn/gtiyseaudx.html

[Q54] 清空表
来源：http://hz.c1oappe.top/gtwiuudmzh.html

TRUNCATE TABLE logs;
来源：http://hz.ivvv.top/gtfgbmulpd.html

[Q55] 排名（并列占位）
来源：http://hz.yuanzhike.top/gtecezbxvo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.quarkkingdee.top/gtjyrlqxss.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydjk.org.cn/gtgnonnpas.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuanzhike.top/gtqrprlony.html

[Q57] 行号
来源：http://hz.andypj.xyz/gtkdjeqcfd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydzc1.top/gtdvffawgs.html

[Q58] 累计求和
来源：http://hz.jqgfzy.top/gtobqkxxzw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.svipenyu.cn/gteemenmef.html

[Q59] 分组内累计
来源：http://hz.gogol.net.cn/gtxjidoxsr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yanxiufei.cn/gtzwjcjyqp.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtbovdqnqh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.haohaochexian.top/gtehrefhfm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuetiantiany.cn/gtnwjnpggu.html

[Q61] 移动平均
来源：http://hz.ybcxt.top/gtpwkqnzvg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fengsongda.top/gtjmlqwspb.html

[Q62] 分组占比
来源：http://hz.yongpay.top/gtwwfhhvjt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtxyhguklx.html

[Q63] 开启事务
来源：http://hz.nanxinkj.top/gtqdhbhypj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jqgfzy.top/gtechxdtlr.html

[Q64] 提交事务
来源：http://hz.jianghu66.top/gtufzcryxd.html

COMMIT;
来源：http://hz.xylfe.cn/gthepyledf.html

[Q65] 回滚事务
来源：http://hz.cqqwz.cn/gtmsymjpuh.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gtsacxkdzz.html

[Q66] 行锁查询
来源：http://hz.yvedp.cn/gtwjaiqwtv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhengqikj.top/gtpxozptzg.html

[Q67] 设置隔离级别
来源：http://hz.cheryme.top/gtlaabhnwu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aizwys.cn/gttghbrovh.html

[Q68] 保存点
来源：http://hz.zycfv.cn/gtzqcwipvu.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtlygdewpc.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gttqtijzxs.html

[Q69] 查看执行计划
来源：http://hz.shangyingyoupin.top/gtgreyqqmo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtjyetnemq.html

[Q70] 更新统计信息
来源：http://hz.yongpay.top/gtxlcqkbtv.html

ANALYZE TABLE users;
来源：http://hz.hnqzz.top/gtwijgdcah.html

[Q71] 查看建表语句
来源：http://hz.ydjk.org.cn/gtmihtrnnl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinyuanbaomall.cn/gtvtdxggvc.html

[Q72] 查看索引
来源：http://hz.bjfxy.top/gthmmqhrba.html

SHOW INDEX FROM users;
来源：http://hz.hywenlv.cn/gtshevetbl.html

[Q73] 查看表状态
来源：http://hz.hongshengwenyu.top/gtngvoquhm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yonumen.top/gtnhqelceu.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtnogkopqa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sufxvd.cn/gtxhkcstae.html

[Q75] 日期格式化
来源：http://hz.andypj.xyz/gtrmjeyebb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gtklqgjrbj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.svipenyu.cn/gtuzoktcxr.html

[Q76] 按天统计
来源：http://hz.chenzaomai.com/gteeclolux.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.mhx1999.top/gtxrvbjsuk.html

[Q77] 时间加减
来源：http://hz.xuetiantiany.cn/gtxtzjsorf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.snrcjt.cn/gtxryghygf.html

[Q78] 当前时间
来源：http://hz.fzhhl.top/gtrxnwiego.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuanzx.com/gtbuezjhck.html

[Q79] 字符串拼接
来源：http://hz.cashguo.top/gtgutzwpbd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tanke756.top/gtuluvytmw.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtklymgsfh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gtluqwtoar.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtlomyecak.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtckmfoayd.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangtech.top/gtonrojyvu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.meibo888.top/gttbpggrxu.html

[Q83] 大小写转换
来源：http://hz.sxryk.cn/gtqrvqemch.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jiagoushi.top/gtgnlnwxnd.html

[Q84] 去除首尾空格
来源：http://hz.hnqzz.top/gtvgvmfgqw.html

SELECT TRIM(name) FROM users;
来源：http://hz.9152youxi.cn/gtsucasxti.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtjiticmzt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yonumen.top/gtmgvskypd.html

[Q86] 读取 JSON 字段
来源：http://hz.daxiang520.top/gtyrvahgql.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fzhhl.top/gttfiqlkao.html

[Q87] JSON 字段做条件
来源：http://hz.mhx1999.top/gtwgvhbopl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xziqi.cn/gtvpvqsfta.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtzhvlvokm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.kuanghao11.cn/gtvguogvpz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenzaomai.com/gtekusldxh.html

[Q89] 判断表是否存在
来源：http://hz.xuetiantiany.cn/gtaafgjyzs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtesiapwme.html

[Q90] 生成序号列
来源：http://hz.zycfv.cn/gtvsttowvd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenjidiqi.icu/gttbkaqzud.html

================================================================================
来源：http://hz.ivvv.top/gthpaocwlw.html

R. Bash 专题
来源：http://hz.xuanzx.com/gtonoaopmh.html

================================================================================
来源：http://hz.hfpthk.cn/gtjbghgcnc.html

[R01] shebang 与严格模式
来源：http://hz.havefunace.top/gtdwctrvnl.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtrmqzuuao.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gtiipunmew.html

[R02] 变量赋值与使用
来源：http://hz.jinqigufen.top/gtuodsavnj.html

name="Tom"; echo "$name"
来源：http://hz.feifeiyinyue.top/gttpjgufcx.html

[R03] 只读变量
来源：http://hz.tanke756.top/gthhbsgbkl.html

readonly PI=3.14
来源：http://hz.ydzc1.top/gttbkbeoui.html

[R04] 位置参数
来源：http://hz.gogol.net.cn/gtbsmzynmf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtdzaifmwl.html

[R05] 参数默认值
来源：http://hz.hysaishi.cn/gthejrqgkj.html

name="${1:-default}"
来源：http://hz.hnxiangtu.top/gtixuzmpod.html

[R06] 判断命令是否存在
来源：http://hz.zhongyouzk.top/gtdsqchdyv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuanzx.com/gtjsrjstca.html

[R07] if 判断文件
来源：http://hz.shuidangran.top/gtadxhvayr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hongshengwenyu.top/gtmhedjeum.html

[R08] 数值比较
来源：http://hz.andypj.xyz/gtvrsrzcnm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hysaishi.cn/gtrhbemshp.html

[R09] 字符串比较
来源：http://hz.feifeiyinyue.top/gtzjdpgjfe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.wangdashe.top/gtlxvqjyxd.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtzqbjlwgq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sufxvd.cn/gtkkolwmxq.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gtcujpmuve.html

case "$1" in
来源：http://hz.yuanzhike.top/gtynsxkzek.html

start) echo "启动" ;;
来源：http://hz.sxryk.cn/gtdosxejuc.html

stop)  echo "停止" ;;
来源：http://hz.ywan-chungtsiang.top/gtrfpmqlsr.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gteoewjjsd.html

esac
来源：http://hz.chenlongwang.top/gttnkeegvf.html

[R12] for 遍历文件
来源：http://hz.xingfuxueyuan.xyz/gtbugiobex.html

for f in *.txt; do echo "$f"; done
来源：http://hz.quarkkingdee.top/gtubpfjqyp.html

[R13] for 计数循环
来源：http://hz.cheryme.top/gtmnvayxam.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtusygbskh.html

[R14] C 风格 for
来源：http://hz.0kj1m.cn/gtszcnorin.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtloqbvpcr.html

[R15] while 逐行读文件
来源：http://hz.haohaochexian.top/gtmvgxwmls.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sysykeji.top/gtdqgxjyzf.html

[R16] until 等待条件
来源：http://hz.sweek.top/gtffcvqadk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ybcxt.top/gtaoxrkakc.html

[R17] 数组定义与取值
来源：http://hz.c1oappe.top/gtywmcynld.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258888.top/gtiraxowea.html

[R18] 遍历数组
来源：http://hz.daria6918.cn/gthfmnmhql.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtundnitsb.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtwdxepjem.html

echo "${#arr[@]}"
来源：http://hz.yueranfly.top/gtsvjnytwi.html

[R20] 关联数组（字典）
来源：http://hz.guowangkeji.top/gtewqixiaj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gaohongyu789.top/gtfdrcrzsb.html

[R21] 字符串长度
来源：http://hz.cashguo.top/gtatpdrdfg.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtbvfdgmor.html

[R22] 截取子串
来源：http://hz.havefunace.top/gtstiazgyh.html

echo "${s:0:5}"
来源：http://hz.xinyue.icu/gtgbnajvnz.html

[R23] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtgwnizaea.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jlsjyb.cn/gttbvhvdad.html

[R24] 大小写转换
来源：http://hz.hfpthk.cn/gtlnpqwvlv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yongpay.top/gtaugyrjjz.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhoulong.xyz/gtjzhdnilf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinghuilouyu.cn/gtfkwkxxpu.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtlerwztyt.html

now=$(date +%F); echo "$now"
来源：http://hz.ybcxt.top/gtgshdteaq.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtkenieqto.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtblyxqpwf.html

[R28] 浮点运算
来源：http://hz.gaohongyu789.top/gtgiurqsnm.html

echo "scale=2; 10/3" | bc
来源：http://hz.xinyue.icu/gtbqtgfafc.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtdahszsdq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtsdcuqctx.html

[R30] 函数返回状态码
来源：http://hz.sweek.top/gtcrlglenf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtbywklwgy.html

[R31] 局部变量
来源：http://hz.pycfn.com/gtbhydzwpv.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuetiantiany.cn/gtvzebckxs.html

[R32] 参数个数校验
来源：http://hz.hnqzz.top/gtzbliwkij.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenzaomai.com/gtoffxowfy.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtniyvnlcd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sxryk.cn/gtarddmdtn.html

[R34] 退出时清理
来源：http://hz.sweek.top/gtkzwhjfcs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtkhkdxnny.html

[R35] 后台执行并等待
来源：http://hz.jlsjyb.cn/gtzxgfibyi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinghuilouyu.cn/gtscylqwjd.html

[R36] 并发执行多个任务
来源：http://hz.yongpay.top/gtyaixzztv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shangyingyoupin.top/gtmhbqijpa.html

[R37] 把输出赋给变量
来源：http://hz.yongpay.top/gtrqqyxiwx.html

files=$(ls -1)
来源：http://hz.xylfe.cn/gtjcmpjptz.html

[R38] 管道串联
来源：http://hz.ppjwa.cn/gtgcgkxjiw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ybcxt.top/gtwfluwdnf.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gtpwwkkqge.html

cmd > out.log 2>&1
来源：http://hz.wangshuangyany.cn/gtzicbstit.html

[R40] 追加写日志
来源：http://hz.ywan-chungtsiang.top/gtvnviwdra.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtwclqhzap.html

[R41] 丢弃输出
来源：http://hz.kuanghao11.cn/gtntauwail.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigfzy.top/gtyfnozncg.html

[R42] 输入重定向
来源：http://hz.jinqigufen.top/gtkuvhhslj.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtccaamdyi.html

[R43] 按名字查找文件
来源：http://hz.yueranfly.top/gtpyaczbve.html

find . -name "*.log" -type f
来源：http://hz.ppjwa.cn/gtnnzxihxl.html

[R44] 按修改时间查找
来源：http://hz.cqqwz.cn/gtcsadpzmh.html

find . -mtime -7 -type f
来源：http://hz.hywenlv.cn/gtwfwdvhvq.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtdqykyune.html


<!-- 参考信息 -->