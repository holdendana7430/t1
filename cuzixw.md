代发 wailian999

================================================================================
来源：http://hz.yj20258.top/gtxtjnuxcs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.9152youxi.cn/gtrnzviylj.html

================================================================================
来源：http://hz.tianlin.xyz/gtmudnyqho.html

[Q01] 创建表
来源：http://hz.smart0.xyz/gtvhpmldef.html

CREATE TABLE users (
来源：http://hz.chenjidiqi.icu/gtzgojusod.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtsowzycvz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sxryk.cn/gtcznyxrki.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuanzhike.top/gteiozwyvb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yanxiufei.cn/gtafjqqzuo.html

);
来源：http://hz.nwbrower.top/gtwppvhfho.html

[Q02] 创建带外键的表
来源：http://hz.ydzc1.top/gtqjgbalfx.html

CREATE TABLE orders (
来源：http://hz.redwolf501.top/gttjnerjid.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtwfvubxzs.html

user_id INT NOT NULL,
来源：http://hz.zhengqikj.top/gtazhzxyzf.html

amount DECIMAL(10, 2),
来源：http://hz.daria6918.cn/gtypyzvabt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigfzy.top/gtakfjgnva.html

);
来源：http://hz.52xcode.cn/gtlstcxizd.html

[Q03] 增加列
来源：http://hz.vqdsnc.cn/gtqxxisefl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtxttceqjx.html

[Q04] 修改列类型
来源：http://hz.yuxming.cn/gtgiebzryo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gotoacloud.top/gtzwfwpoqt.html

[Q05] 重命名列
来源：http://hz.daxiang520.top/gtzuigvwfy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.pycfn.com/gteehnxkns.html

[Q06] 删除列
来源：http://hz.vqdsnc.cn/gtjxfkfgac.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.iojbl.cn/gtfiiagavc.html

[Q07] 删除表
来源：http://hz.chenzaomai.com/gtetwzftzs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigufen.top/gtcawzvyuh.html

[Q08] 创建普通索引
来源：http://hz.xuanzx.com/gthjcveijw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gthvqbaush.html

[Q09] 创建唯一索引
来源：http://hz.xylfe.cn/gtzeblnctg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.aibaodan.cn/gtqdwtytau.html

[Q10] 插入单行
来源：http://hz.chenjidiqi.icu/gtamrteayi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.0kj1m.cn/gtylfcriai.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtqlcvojok.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nanxuanxn.top/gticryixcg.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gtnkjcsfcf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtzwzrflfq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ehwqpu.com/gtbbkxniuq.html

[Q13] 忽略重复插入
来源：http://hz.xylfe.cn/gtgktrajyn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.dashuyun.cn/gtshynlqtn.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenzaomai.com/gtkcemihfx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xylfe.cn/gtkmzdemvp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gtskigaocg.html

[Q15] 查询全部
来源：http://hz.daria6918.cn/gtgscvfbxh.html

SELECT * FROM users;
来源：http://hz.xylfe.cn/gtvfubfnvx.html

[Q16] 查询指定列
来源：http://hz.jyoumei.cn/gtmqxlnfbt.html

SELECT id, name FROM users;
来源：http://hz.snrcjt.cn/gtwiiiovdd.html

[Q17] 条件查询
来源：http://hz.316326.xyz/gthpmhlsbz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aibaodan.cn/gtfggejhvg.html

[Q18] 模糊匹配
来源：http://hz.ybcxt.top/gtxxnxzmog.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jyoumei.cn/gtlvhdclyz.html

[Q19] 范围查询
来源：http://hz.9152youxi.cn/gtdswoqrul.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yongpay.top/gtojmadkop.html

[Q20] IN 列表
来源：http://hz.meibo888.top/gthfpxomiy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gaohongyu789.top/gtitaijcgd.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtixnqhpbv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuanzhike.top/gtyhzckhpb.html

[Q22] 排序
来源：http://hz.redwolf501.top/gtumcttnnp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aibaodan.cn/gtwqwvdtsh.html

[Q23] 分页
来源：http://hz.gzhubu.top/gtenhuoyns.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj202588.top/gtbytbaufl.html

[Q24] 去重
来源：http://hz.andypj.xyz/gtqzgcddfy.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenzaomai.com/gtwpilahnp.html

[Q25] 只取前 N 条
来源：http://hz.zhengqikj.top/gtqacinlfu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sufxvd.cn/gtmfthhkff.html

[Q26] 计数
来源：http://hz.shuidangran.top/gtrholnfbk.html

SELECT COUNT(*) FROM users;
来源：http://hz.mhx1999.top/gtmevkmxfk.html

[Q27] 条件计数
来源：http://hz.yanxiufei.cn/gtfsfkpewz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuanzx.com/gtzblgoafp.html

[Q28] 求和与平均
来源：http://hz.gotoacloud.top/gtrhiasedb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cashguo.top/gtgfosxuda.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gtlvjbmruh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.quarkkingdee.top/gtrtkikyjc.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtbitxgfsf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtwvpygoqj.html

[Q31] 分组后过滤
来源：http://hz.xuetiantiany.cn/gtjqtltjqm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hammf.cn/gtvhnpizmd.html

[Q32] 分组拼接字符串
来源：http://hz.svipenyu.cn/gtfxjtwate.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtacyxkvzb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.birdmap.top/gtvmxwqqlh.html

[Q33] 多列分组
来源：http://hz.ivvv.top/gtepehspde.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tianlin.xyz/gtwcvuxsml.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtjnuuocmn.html

SELECT * FROM (
来源：http://hz.jqgufenzy.top/gtbhbtporo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fengsongda.top/gtewfnlieb.html

) t WHERE rn = 1;
来源：http://hz.0kj1m.cn/gtsgxbpyks.html

[Q35] 内连接
来源：http://hz.yvedp.cn/gtnvqjspcd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtfnlntnkc.html

[Q36] 左连接
来源：http://hz.yj20258888.top/gtphkgbleo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtpzrssfzl.html

[Q37] 右连接
来源：http://hz.tian-w.cn/gtwmcvvkvx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yanxiufei.cn/gtzgzreyfp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yuxming.cn/gtgknuawon.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenzaomai.com/gtzdrkrsqd.html

[Q39] 自连接（查上下级）
来源：http://hz.jinghuilouyu.cn/gtvwxuyspg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gtfuvxswao.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daxiang520.top/gtbshbqsfz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangshuangyany.cn/gtplahzmse.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gaohongyu789.top/gtjtzzjoyn.html

[Q41] 多表连接
来源：http://hz.hywenlv.cn/gtlteruedk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.52xcode.cn/gtbaeufxmc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jyoumei.cn/gtmpvdbnbt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinyuanbaomall.cn/gtgzswowzu.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgfzy.top/gtxancpgzh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenlongwang.top/gthiwtgctk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.haohaochexian.top/gtcoijnpem.html

[Q43] 标量子查询
来源：http://hz.zhengqikj.top/gtpruzfdvi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtvvgjflhz.html

[Q44] IN 子查询
来源：http://hz.9152youxi.cn/gtrxjxhqxq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gtmgybtrdf.html

[Q45] EXISTS 判断存在
来源：http://hz.ybcxt.top/gtdcogypml.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtfecqeihr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pycfn.com/gtpogfcjwc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtvazjgorm.html

[Q47] 与平均值比较
来源：http://hz.jyoumei.cn/gtrfvczbbt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnqzz.top/gtgulcklas.html

[Q48] CTE 公用表表达式
来源：http://hz.c1oappe.top/gthbojiwdr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ybcxt.top/gtsjtuonml.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangshuangyany.cn/gtpudbdaee.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtievwgssg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258.top/gtyycnfypn.html

[Q50] 批量更新
来源：http://hz.wangdashe.top/gtzuaxwvqn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtffavhxhj.html

[Q51] 用子查询更新
来源：http://hz.yj20258888.top/gtqivbnsjd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xylfe.cn/gtymzjttac.html

[Q52] 删除指定行
来源：http://hz.ybcxt.top/gtilgorglc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xylfe.cn/gtsqwiufxh.html

[Q53] 按条件删除
来源：http://hz.ehwqpu.com/gtynzcpqtr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ivvv.top/gtuyezqtgm.html

[Q54] 清空表
来源：http://hz.zhiwuduotai.top/gtkfhjdxdk.html

TRUNCATE TABLE logs;
来源：http://hz.fengsongda.top/gttcaqifhn.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtzdotixyr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tanke756.top/gtkzmmfate.html

[Q56] 密集排名（并列不占位）
来源：http://hz.316326.xyz/gttpgjskbj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nwbrower.top/gtmuielvoi.html

[Q57] 行号
来源：http://hz.daxiang520.top/gtuztqxscq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yanxiufei.cn/gtmjhroanh.html

[Q58] 累计求和
来源：http://hz.hnxiangtu.top/gtktripeul.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ybcxt.top/gtjtvuclqb.html

[Q59] 分组内累计
来源：http://hz.xuanzx.com/gtgeobfuzz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgufenzy.top/gtfkqnqyas.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenjidiqi.icu/gtcjnfdbxe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.feifeiyinyue.top/gtsesmyebn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xziqi.cn/gtkhdfrjto.html

[Q61] 移动平均
来源：http://hz.zhoulong.xyz/gttlzsolad.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenzaomai.com/gtcgiuexyt.html

[Q62] 分组占比
来源：http://hz.hnxiangtu.top/gtvsvofdma.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtkoczjzyc.html

[Q63] 开启事务
来源：http://hz.ywan-chungtsiang.top/gtoufgwmos.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.pengpengdd.cyou/gtmnrjroum.html

[Q64] 提交事务
来源：http://hz.52xcode.cn/gttnenjota.html

COMMIT;
来源：http://hz.jqgufenzy.top/gtrfmzwpuf.html

[Q65] 回滚事务
来源：http://hz.ppjwa.cn/gtszfznzup.html

ROLLBACK;
来源：http://hz.hysaishi.cn/gttxvzfzug.html

[Q66] 行锁查询
来源：http://hz.hammf.cn/gttmwadvhy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ydzc1.top/gtbuqdjyvx.html

[Q67] 设置隔离级别
来源：http://hz.aibaodan.cn/gtvtsjpjri.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tanke756.top/gtzyxckuhm.html

[Q68] 保存点
来源：http://hz.aizwys.cn/gtlzkogvbb.html

SAVEPOINT sp1;
来源：http://hz.quarkkingdee.top/gtzwjeibtp.html

ROLLBACK TO sp1;
来源：http://hz.tanke756.top/gtsntkztzg.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gtydoqgmcp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.9152youxi.cn/gtlovznzad.html

[Q70] 更新统计信息
来源：http://hz.cdnleiting.top/gtoqjidthn.html

ANALYZE TABLE users;
来源：http://hz.ybcxt.top/gtiwimkomx.html

[Q71] 查看建表语句
来源：http://hz.nanxuanxn.top/gtyltxhiyq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gtmusardpz.html

[Q72] 查看索引
来源：http://hz.ivvv.top/gtfwpngvws.html

SHOW INDEX FROM users;
来源：http://hz.redwolf501.top/gtgiffxdxl.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gtaikkntgs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gogol.net.cn/gtswqwgqxo.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangkeji.top/gtosysnpmx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hfpthk.cn/gtrltkohju.html

[Q75] 日期格式化
来源：http://hz.hnxiangtu.top/gthrxlivwu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gaohongyu789.top/gtszzfbnij.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guannengcc.top/gtvgcjxnuw.html

[Q76] 按天统计
来源：http://hz.zhaomingkeji.xyz/gtfbyjsrlu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigufen.top/gthetkyacf.html

[Q77] 时间加减
来源：http://hz.iojbl.cn/gtcaoyrcak.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtlgijkjfc.html

[Q78] 当前时间
来源：http://hz.xziqi.cn/gtmscodjsd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhijiandao.cn/gtqpttcwtm.html

[Q79] 字符串拼接
来源：http://hz.jinghuilouyu.cn/gtcrgfcmpt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hysaishi.cn/gtjbnwmzvw.html

[Q80] 字符串截取
来源：http://hz.zdqjudy.top/gthsekehpk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgufenzy.top/gtzefosegw.html

[Q81] 字符串替换
来源：http://hz.xuetiantiany.cn/gtpamsboxw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj202588.top/gtvziucjxy.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtnwcpckse.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhijiandao.cn/gtaoyttvqz.html

[Q83] 大小写转换
来源：http://hz.sufxvd.cn/gtifjttzzq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.vqdsnc.cn/gtsfjadbdc.html

[Q84] 去除首尾空格
来源：http://hz.redwolf501.top/gtipnoxdqa.html

SELECT TRIM(name) FROM users;
来源：http://hz.jlsjyb.cn/gtelsilsra.html

[Q85] 数值取整
来源：http://hz.ppjwa.cn/gtzcpmntce.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.vqdsnc.cn/gtcnfgybej.html

[Q86] 读取 JSON 字段
来源：http://hz.xinyue.icu/gtlqsesdzs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tianlin.xyz/gtkcbuowlz.html

[Q87] JSON 字段做条件
来源：http://hz.hammf.cn/gtreogxlem.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hammf.cn/gtamvdhepg.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtpoffsdmp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ppjwa.cn/gtmpbiipfv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sysykeji.top/gtcwqnzvck.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtqedfddqe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnxiangtu.top/gtlprztbvo.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtedbeysee.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shangyingyoupin.top/gthoqmxyae.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtorqousrl.html

R. Bash 专题
来源：http://hz.yuxming.cn/gtuetpirmg.html

================================================================================
来源：http://hz.havefunace.top/gtcjumfnrq.html

[R01] shebang 与严格模式
来源：http://hz.chenlongwang.top/gtugwbpwam.html

#!/usr/bin/env bash
来源：http://hz.zhijiandao.cn/gtmyaquuhy.html

set -euo pipefail
来源：http://hz.aizwys.cn/gtqqcpbmvd.html

[R02] 变量赋值与使用
来源：http://hz.jqgfzy.top/gthapvcina.html

name="Tom"; echo "$name"
来源：http://hz.gogol.net.cn/gtavuywwky.html

[R03] 只读变量
来源：http://hz.ydjk.org.cn/gttgfnmhxi.html

readonly PI=3.14
来源：http://hz.ywan-chungtsiang.top/gtchzqoyrj.html

[R04] 位置参数
来源：http://hz.wangshuangyany.cn/gtxefucsou.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangkeji.top/gtbtwlggbw.html

[R05] 参数默认值
来源：http://hz.daria6918.cn/gtgiqqzybm.html

name="${1:-default}"
来源：http://hz.jlsjyb.cn/gtssirayyw.html

[R06] 判断命令是否存在
来源：http://hz.jlsjyb.cn/gtdxxydpnz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.haohaochexian.top/gtachlceuy.html

[R07] if 判断文件
来源：http://hz.chenzaomai.com/gtiydrzrpo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.vqdsnc.cn/gtgdlbxbig.html

[R08] 数值比较
来源：http://hz.tian-w.cn/gtrgjjvyed.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.bjfxy.top/gtsjwoogkb.html

[R09] 字符串比较
来源：http://hz.ppjwa.cn/gtjdvwecxp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtdqirzehl.html

[R10] 正则匹配
来源：http://hz.jqgufenzy.top/gteahrzpdw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtrqcysibg.html

[R11] case 多分支
来源：http://hz.zycfv.cn/gtpnfngvpk.html

case "$1" in
来源：http://hz.birdmap.top/gtgtrzgbxb.html

start) echo "启动" ;;
来源：http://hz.jianghu66.top/gtxysszbrt.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtrfyrylfo.html

*)     echo "未知命令" ;;
来源：http://hz.yonumen.top/gtjhiwnwim.html

esac
来源：http://hz.yvedp.cn/gthqqlfpxv.html

[R12] for 遍历文件
来源：http://hz.ydjk.org.cn/gtarfcafkd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.fzhhl.top/gtuyictzse.html

[R13] for 计数循环
来源：http://hz.cdnleiting.top/gttlsulqvu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenzaomai.com/gtaveedyuw.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gtabxzagjj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xylfe.cn/gtleghqnfu.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtqsboxcap.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tanke756.top/gtowfoxktd.html

[R16] until 等待条件
来源：http://hz.52xcode.cn/gtczqgjgaf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtfsxebcnb.html

[R17] 数组定义与取值
来源：http://hz.316326.xyz/gtefynbsae.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhixingplan.top/gtvbjvdnez.html

[R18] 遍历数组
来源：http://hz.yuanzhike.top/gthymailnf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgfzy.top/gtcsiawvxz.html

[R19] 数组长度
来源：http://hz.mhx1999.top/gtpcoehbwj.html

echo "${#arr[@]}"
来源：http://hz.cqqwz.cn/gtiobvnscq.html

[R20] 关联数组（字典）
来源：http://hz.ybcxt.top/gtirdvnnkl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yvedp.cn/gttbnpophp.html

[R21] 字符串长度
来源：http://hz.havefunace.top/gticladuyh.html

echo "${#s}"
来源：http://hz.zhiwuduotai.top/gtnpfaxwgq.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gttsthpyev.html

echo "${s:0:5}"
来源：http://hz.cashguo.top/gtjbkqdpts.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gteaazyjwb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.quarkkingdee.top/gtjrqrbpei.html

[R24] 大小写转换
来源：http://hz.daxiang520.top/gtnqrismws.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hfpthk.cn/gtcffswagl.html

[R25] 去后缀 / 去前缀
来源：http://hz.kuanghao11.cn/gtexuhnwnu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258.top/gtxtvvqqla.html

[R26] 命令替换
来源：http://hz.hywenlv.cn/gtilnvqnnd.html

now=$(date +%F); echo "$now"
来源：http://hz.ybcxt.top/gtdxfhcgtm.html

[R27] 算术展开
来源：http://hz.jinghuilouyu.cn/gtjtqytbva.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtoblzfmar.html

[R28] 浮点运算
来源：http://hz.guowangkeji.top/gtzbdoyijo.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhijiandao.cn/gttoqdzqha.html

[R29] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtwufwtuin.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gtkyklcvwi.html

[R30] 函数返回状态码
来源：http://hz.ppjwa.cn/gtqjcpbaty.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtkjuucrxt.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtersutign.html

f() { local x=1; echo "$x"; }
来源：http://hz.dashuyun.cn/gtpglmvkdo.html

[R32] 参数个数校验
来源：http://hz.nanxuanxn.top/gtwalxcfpb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtsyselcto.html

[R33] 捕获错误并提示行号
来源：http://hz.316326.xyz/gthbzdnqkf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinyuanbaomall.cn/gtyasztwll.html

[R34] 退出时清理
来源：http://hz.jiagoushi.top/gtygjwhixt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtdtvkcgaf.html

[R35] 后台执行并等待
来源：http://hz.zhongyouzk.top/gtarbemocy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.nwbrower.top/gtumayqahv.html

[R36] 并发执行多个任务
来源：http://hz.sweek.top/gtttqbggih.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jiagoushi.top/gtzpsjxawl.html

[R37] 把输出赋给变量
来源：http://hz.jinyuanbaomall.cn/gtjcbqhfug.html

files=$(ls -1)
来源：http://hz.zhaomingkeji.xyz/gtglwxfoag.html

[R38] 管道串联
来源：http://hz.andypj.xyz/gtxczrwtji.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuxming.cn/gtzbqgntos.html

[R39] 重定向标准输出与错误
来源：http://hz.ywan-chungtsiang.top/gtmwvmpcao.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtcrsblzzk.html

[R40] 追加写日志
来源：http://hz.xinyue.icu/gtuvxrokyh.html

echo "log" >> out.log
来源：http://hz.daria6918.cn/gtcfsnglui.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtrrtqejww.html

cmd >/dev/null 2>&1
来源：http://hz.cheryme.top/gtksxarkao.html

[R42] 输入重定向
来源：http://hz.snrcjt.cn/gtvuhknkhz.html

wc -l < a.txt
来源：http://hz.ppjwa.cn/gtvkrcprse.html

[R43] 按名字查找文件
来源：http://hz.quarkkingdee.top/gtkflpuilh.html


<!-- 参考信息 -->