代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenjidiqi.icu/gtxvcadsvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guowangkeji.top/gtfbimeftz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daria6918.cn/gtfwrnbuiz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yueranfly.top/gtfezmushz.html

================================================================================
来源：http://hz.c1oappe.top/gtqxjoditr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xinyue.icu/gtddvhqkvv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqclhdudi.html

[Q01] 创建表
来源：http://hz.jyoumei.cn/gttgxruydo.html

CREATE TABLE users (
来源：http://hz.vqdsnc.cn/gtenrmcszg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ehwqpu.com/gtnbarmnyj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.bjfxy.top/gtjihwzwyd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinghuilouyu.cn/gtnjtbekfc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cqqwz.cn/gtyaqkvkiw.html

);
来源：http://hz.chenjidiqi.icu/gtxlrkviqn.html

[Q02] 创建带外键的表
来源：http://hz.yongpay.top/gttaomipsz.html

CREATE TABLE orders (
来源：http://hz.daria6918.cn/gtgtegpymu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtpmqtnnvd.html

user_id INT NOT NULL,
来源：http://hz.haohaochexian.top/gtqvksmbyh.html

amount DECIMAL(10, 2),
来源：http://hz.xziqi.cn/gtsvsxmdjx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shuidangran.top/gtewgkiqap.html

);
来源：http://hz.xylfe.cn/gtsqqijbpn.html

[Q03] 增加列
来源：http://hz.jinqigfzy.top/gtrfwvlnhf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenjidiqi.icu/gttdeseuuy.html

[Q04] 修改列类型
来源：http://hz.gotoacloud.top/gtisrhzssw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sysykeji.top/gtbdicqnot.html

[Q05] 重命名列
来源：http://hz.hysaishi.cn/gtogetqffz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhaomingkeji.xyz/gtebhvepda.html

[Q06] 删除列
来源：http://hz.hongshengwenyu.top/gtemsdzcmk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.52xcode.cn/gtsuxicahx.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtbmysgetk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhengqikj.top/gtwrqkixjb.html

[Q08] 创建普通索引
来源：http://hz.nanxuanxn.top/gtetzsbwda.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtclnakkow.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtezoxfegq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cdnleiting.top/gtbtjaexfb.html

[Q10] 插入单行
来源：http://hz.cashguo.top/gtyxtwprjt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenlongwang.top/gtqhhgahrq.html

[Q11] 一次插入多行
来源：http://hz.aizwys.cn/gtakphgged.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.birdmap.top/gtpgxylezw.html

[Q12] 插入后取自增 ID
来源：http://hz.hfpthk.cn/gtogwaayex.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.vqdsnc.cn/gtegocmuty.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtphvfgdmc.html

[Q13] 忽略重复插入
来源：http://hz.guowangkeji.top/gtwazcnuug.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxinkj.top/gtyitzyjpj.html

[Q14] 存在则更新（upsert）
来源：http://hz.gzhubu.top/gtgoirzwsy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cqqwz.cn/gtfmhmjfcj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hnxiangtu.top/gtvzifvnrx.html

[Q15] 查询全部
来源：http://hz.wangdashe.top/gtexxtgmwb.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtjrfzsjgd.html

[Q16] 查询指定列
来源：http://hz.iojbl.cn/gtibfcbptn.html

SELECT id, name FROM users;
来源：http://hz.wangdashe.top/gtzfwnfybb.html

[Q17] 条件查询
来源：http://hz.ydzc1.top/gtkooijwms.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xinyue.icu/gtyhixnlzr.html

[Q18] 模糊匹配
来源：http://hz.bjfxy.top/gtfsbfsyxg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangdashe.top/gtwgtropih.html

[Q19] 范围查询
来源：http://hz.pengpengdd.cyou/gtsrlsgnfr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxuanxn.top/gtjkqqhpow.html

[Q20] IN 列表
来源：http://hz.zhoulong.xyz/gtokcetcax.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guannengcc.top/gttmrxdqse.html

[Q21] 空值判断
来源：http://hz.zhongyouzk.top/gtvhfqskiw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydzc1.top/gtftmvjtfv.html

[Q22] 排序
来源：http://hz.ywan-chungtsiang.top/gtnrliopfq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hfpthk.cn/gtkehhblli.html

[Q23] 分页
来源：http://hz.hysaishi.cn/gtadclxcvn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dianchejie.cn/gtldrdxoyx.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gtavkgvbbr.html

SELECT DISTINCT city FROM users;
来源：http://hz.ybcxt.top/gtsvoyhxmr.html

[Q25] 只取前 N 条
来源：http://hz.sufxvd.cn/gtlzkconyt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dashuyun.cn/gtrncqfvpd.html

[Q26] 计数
来源：http://hz.xuetiantiany.cn/gtlzkapjae.html

SELECT COUNT(*) FROM users;
来源：http://hz.yongpay.top/gtotozjgbz.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtllcbbaph.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ivvv.top/gtbzubtphe.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtfwpxmrfz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.kuanghao11.cn/gtvattxlnk.html

[Q29] 最大最小值
来源：http://hz.andypj.xyz/gtntyceyfk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgfzy.top/gtbhioaluv.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtxtcyxdyk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtggjdwavt.html

[Q31] 分组后过滤
来源：http://hz.sxryk.cn/gtmhmpzrym.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sysykeji.top/gtdrzoeoeh.html

[Q32] 分组拼接字符串
来源：http://hz.cucudq.cn/gtzqirveqt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gterdnnmgk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cdnleiting.top/gtafsmgsrs.html

[Q33] 多列分组
来源：http://hz.zhongyouzk.top/gtufrusqin.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnqzz.top/gtlhablkti.html

[Q34] 每组取第一条
来源：http://hz.shanyushiyangkeji.top/gtguiiciqh.html

SELECT * FROM (
来源：http://hz.zhengqikj.top/gtiztgitkt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtvqzwxjgj.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtqtbsrkaj.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtbhheiduu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jiagoushi.top/gtrebohsov.html

[Q36] 左连接
来源：http://hz.vqdsnc.cn/gtcrxbiksj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtyzojvvnu.html

[Q37] 右连接
来源：http://hz.gotoacloud.top/gtzmfvxyim.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tian-w.cn/gtwciuxktc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daxiang520.top/gteieeapfa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jiagoushi.top/gtevnyfbkj.html

[Q39] 自连接（查上下级）
来源：http://hz.zhengqikj.top/gtdugrprgl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.iojbl.cn/gthrfowkbz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtbhlvojbt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinghuilouyu.cn/gteckrmlgs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cashguo.top/gtfggpreft.html

[Q41] 多表连接
来源：http://hz.daria6918.cn/gtcxfhsild.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sweek.top/gtryiqtknk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hysaishi.cn/gtbnwmtdep.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhixingplan.top/gtdgnfhcwq.html

[Q42] 连接条件附加过滤
来源：http://hz.shzxlz.cn/gtkwyoiruj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nwbrower.top/gtiobkkzkm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.snrcjt.cn/gtunpifohr.html

[Q43] 标量子查询
来源：http://hz.shanyushiyangkeji.top/gtanywmhvr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.c1oappe.top/gtlppwtlmt.html

[Q44] IN 子查询
来源：http://hz.shangyingyoupin.top/gtxeoumusq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shuidangran.top/gtmfpwfytk.html

[Q45] EXISTS 判断存在
来源：http://hz.hongshengwenyu.top/gtvgnfmftp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtwwbgjbsj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.guowangkeji.top/gtvtuctcyx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtlyaefhxy.html

[Q47] 与平均值比较
来源：http://hz.mhx1999.top/gteluqvmsx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yanxiufei.cn/gtrzmzthbp.html

[Q48] CTE 公用表表达式
来源：http://hz.guowangkeji.top/gtqoympbzo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangtech.top/gtphqwqtmn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigfzy.top/gtzuczmhtu.html

[Q49] 更新单行
来源：http://hz.zhaomingkeji.xyz/gtkriqcczo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtvtntpctc.html

[Q50] 批量更新
来源：http://hz.hnqzz.top/gtdxuakwal.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhiwuduotai.top/gttxfyalgy.html

[Q51] 用子查询更新
来源：http://hz.zhixingplan.top/gtvhjlfojv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hongshengwenyu.top/gtggroalfy.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtrezjxzsb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhixingplan.top/gtlmgaokch.html

[Q53] 按条件删除
来源：http://hz.xylfe.cn/gtgjasvmln.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenzaomai.com/gtrrhftprt.html

[Q54] 清空表
来源：http://hz.daria6918.cn/gtmczudqxm.html

TRUNCATE TABLE logs;
来源：http://hz.gzhubu.top/gtlsbpdyxq.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigufen.top/gtousdjljr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtykorsbsp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigfzy.top/gtkntapsnw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhiwuduotai.top/gtvhcdrmbc.html

[Q57] 行号
来源：http://hz.wangdashe.top/gtlogplsua.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sufxvd.cn/gtgghpgcsn.html

[Q58] 累计求和
来源：http://hz.hongshengwenyu.top/gtpzmvbaqi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guowangkeji.top/gttdvesgqp.html

[Q59] 分组内累计
来源：http://hz.zhengqikj.top/gtvyyohwlg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtttbvbfuc.html

[Q60] 取上一行 / 下一行
来源：http://hz.birdmap.top/gtwbpwvvbb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ybcxt.top/gtagegsjsc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigufen.top/gtyveubqlk.html

[Q61] 移动平均
来源：http://hz.xuanzx.com/gtoumtmocj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hnxiangtu.top/gtfhmxrbvl.html

[Q62] 分组占比
来源：http://hz.shanyushiyangkeji.top/gtiylvbecb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gttzozluao.html

[Q63] 开启事务
来源：http://hz.gogol.net.cn/gtvstpbyig.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtnxjkycqr.html

[Q64] 提交事务
来源：http://hz.iojbl.cn/gtllfetmlz.html

COMMIT;
来源：http://hz.hysaishi.cn/gteufefmha.html

[Q65] 回滚事务
来源：http://hz.pengpengdd.cyou/gtswufppls.html

ROLLBACK;
来源：http://hz.kuanghao11.cn/gtzmayjzht.html

[Q66] 行锁查询
来源：http://hz.hywenlv.cn/gtrqemsong.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxinkj.top/gtumpcnnob.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtkrugaoof.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuetiantiany.cn/gtqbyidrbp.html

[Q68] 保存点
来源：http://hz.nanxinkj.top/gtrjyyaxvo.html

SAVEPOINT sp1;
来源：http://hz.sufxvd.cn/gtkfkunoqr.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gturfvluaj.html

[Q69] 查看执行计划
来源：http://hz.cashguo.top/gtzhcxbrrx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtusxhnxnv.html

[Q70] 更新统计信息
来源：http://hz.bjfxy.top/gttawuxfkw.html

ANALYZE TABLE users;
来源：http://hz.aibaodan.cn/gttmbteuil.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtktoiehxz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gtiqzrdwmz.html

[Q72] 查看索引
来源：http://hz.shzxlz.cn/gtrlpvmtye.html

SHOW INDEX FROM users;
来源：http://hz.guowangkeji.top/gtpphipakc.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtmjwqxuqz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.9152youxi.cn/gtlacxhxsn.html

[Q74] 强制使用索引
来源：http://hz.xuanzx.com/gtjypvbzvn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtkfcrepdv.html

[Q75] 日期格式化
来源：http://hz.xziqi.cn/gtybvvrgla.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hysaishi.cn/gtyjihyvdo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xingfuxueyuan.xyz/gtjnphawlq.html

[Q76] 按天统计
来源：http://hz.guannengcc.top/gtpwzzgnyl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pengpengdd.cyou/gtvrqopbax.html

[Q77] 时间加减
来源：http://hz.aibaodan.cn/gtipvuqfxe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.andypj.xyz/gtbxegwmul.html

[Q78] 当前时间
来源：http://hz.shuidangran.top/gtjhclsfpb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.meibo888.top/gtxztzlddx.html

[Q79] 字符串拼接
来源：http://hz.yongpay.top/gtgosdctsc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj202588.top/gtrrqmdahs.html

[Q80] 字符串截取
来源：http://hz.jqgfzy.top/gtaihsvsdo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtacwpuucj.html

[Q81] 字符串替换
来源：http://hz.zhoulong.xyz/gtcolghrne.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.andypj.xyz/gtktfgxkau.html

[Q82] 字符长度与字节长度
来源：http://hz.shzxlz.cn/gthrzmiibl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenlongwang.top/gtxxmhsqif.html

[Q83] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtsjomcjjs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.havefunace.top/gtupmlhpxu.html

[Q84] 去除首尾空格
来源：http://hz.shangyingyoupin.top/gtimojmxgd.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gthferizfs.html

[Q85] 数值取整
来源：http://hz.aibaodan.cn/gtpmifatgr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yangfankeji.com/gtsokjrtqm.html

[Q86] 读取 JSON 字段
来源：http://hz.hfpthk.cn/gtznnqxctp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.iojbl.cn/gtrlndmzir.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gtdbtnvbzt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gtyulepkqm.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangshuangyany.cn/gthfsxncto.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.snrcjt.cn/gtzhbobstm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hfpthk.cn/gtwtofchop.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtlrjafumu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtzruhpgoc.html

[Q90] 生成序号列
来源：http://hz.fengsongda.top/gtmcqzyizc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.iojbl.cn/gtprbyvmto.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwpfgpaea.html

R. Bash 专题
来源：http://hz.zhixingplan.top/gttsmseyyo.html

================================================================================
来源：http://hz.mhx1999.top/gtaelvxecs.html

[R01] shebang 与严格模式
来源：http://hz.jyoumei.cn/gtltnkzsar.html

#!/usr/bin/env bash
来源：http://hz.snrcjt.cn/gtjpupofqy.html

set -euo pipefail
来源：http://hz.ivvv.top/gtcjqqzcdm.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtmjaraykh.html

name="Tom"; echo "$name"
来源：http://hz.xingfuxueyuan.xyz/gtzbvtxlhy.html

[R03] 只读变量
来源：http://hz.hongshengwenyu.top/gtthmghmwl.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtsnaangwu.html

[R04] 位置参数
来源：http://hz.yj20258.top/gtajrrqmac.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cucudq.cn/gtfrztglgy.html

[R05] 参数默认值
来源：http://hz.tianlin.xyz/gtqakvqsud.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtunrglnzc.html

[R06] 判断命令是否存在
来源：http://hz.nanxuanxn.top/gthutujqdy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtlbqhvrcv.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gtlqmkgrri.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.9152youxi.cn/gtplogwowo.html

[R08] 数值比较
来源：http://hz.yvedp.cn/gtxycycfop.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.52xcode.cn/gtfwxboyvu.html

[R09] 字符串比较
来源：http://hz.yuanzhike.top/gtbavurjnr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gtuhxlpsjs.html

[R10] 正则匹配
来源：http://hz.sxryk.cn/gtanrsdpyn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gttrxulrem.html

[R11] case 多分支
来源：http://hz.yueranfly.top/gtahxoatxr.html

case "$1" in
来源：http://hz.dashuyun.cn/gtkngsfnux.html

start) echo "启动" ;;
来源：http://hz.ppjwa.cn/gtovgwzyia.html

stop)  echo "停止" ;;
来源：http://hz.jianghu66.top/gtvfgtdwer.html

*)     echo "未知命令" ;;
来源：http://hz.yuanzhike.top/gtxrnsizvi.html

esac
来源：http://hz.xuanzx.com/gtfrkfitxy.html

[R12] for 遍历文件
来源：http://hz.snrcjt.cn/gtvamozueo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pengpengdd.cyou/gtifzbjfhl.html

[R13] for 计数循环
来源：http://hz.nwbrower.top/gtdeyhpjha.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dashuyun.cn/gtbmnyxhmc.html

[R14] C 风格 for
来源：http://hz.shangyingyoupin.top/gtthduvnns.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gtcbamawgf.html

[R15] while 逐行读文件
来源：http://hz.jlsjyb.cn/gtyjtjjkod.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenlongwang.top/gtsvheluon.html

[R16] until 等待条件
来源：http://hz.jqgfzy.top/gtcbcczajp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hnxiangtu.top/gtgzpxtwan.html

[R17] 数组定义与取值
来源：http://hz.316326.xyz/gtxtnhgcpa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtgcmkqxen.html

[R18] 遍历数组
来源：http://hz.guannengcc.top/gtuxguomhz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fzhhl.top/gtwyoizwuo.html

[R19] 数组长度
来源：http://hz.gaohongyu789.top/gtiuhgursb.html

echo "${#arr[@]}"
来源：http://hz.yj202588.top/gtcwmrnafa.html

[R20] 关联数组（字典）
来源：http://hz.ydjk.org.cn/gtsbyeaaxm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daria6918.cn/gtjooryylv.html

[R21] 字符串长度
来源：http://hz.hnxiangtu.top/gtbcedvfno.html

echo "${#s}"
来源：http://hz.chenzaomai.com/gtqtxmuvpx.html

[R22] 截取子串
来源：http://hz.jlsjyb.cn/gtjwxtrnnj.html

echo "${s:0:5}"
来源：http://hz.aibaodan.cn/gtvnuvfhjh.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gttlatfswl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gtxddaswmt.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtvlwaxkdg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.wangdashe.top/gtubthjhsx.html

[R25] 去后缀 / 去前缀
来源：http://hz.fengsongda.top/gtpauxwway.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gtmkihsgvx.html

[R26] 命令替换
来源：http://hz.zhengqikj.top/gttdotzaup.html

now=$(date +%F); echo "$now"
来源：http://hz.cucudq.cn/gtbrxvxnsq.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtzlilbnfu.html

echo $((1 + 2 * 3))
来源：http://hz.feifeiyinyue.top/gtkxrwncrt.html

[R28] 浮点运算
来源：http://hz.aizwys.cn/gtnhnlwasm.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnxiangtu.top/gtfayoucfg.html

[R29] 定义函数
来源：http://hz.zycfv.cn/gtgeovolym.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinyuanbaomall.cn/gtudypgixm.html

[R30] 函数返回状态码
来源：http://hz.yongpay.top/gtthlawwtt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ivvv.top/gtollwymhs.html

[R31] 局部变量
来源：http://hz.dianchejie.cn/gtkmmahqad.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgufenzy.top/gtpexmniva.html

[R32] 参数个数校验
来源：http://hz.jqgfzy.top/gtfxvhpnwh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.iojbl.cn/gtgbbmdvba.html

[R33] 捕获错误并提示行号
来源：http://hz.mhx1999.top/gttqfuucvf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gotoacloud.top/gtjfsbkeha.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gtqzzrokvu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtusihptgb.html

[R35] 后台执行并等待
来源：http://hz.c1oappe.top/gtcmezlhux.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fengsongda.top/gtckwdlbwe.html

[R36] 并发执行多个任务
来源：http://hz.yonumen.top/gtfesfjnql.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtbcbynycd.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtpdpbfpnu.html

files=$(ls -1)
来源：http://hz.cashguo.top/gtmykfowhf.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gtursycldh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sufxvd.cn/gtezzhbcbg.html

[R39] 重定向标准输出与错误
来源：http://hz.gogol.net.cn/gtiwmpyokw.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gthrqaeesm.html

[R40] 追加写日志
来源：http://hz.cucudq.cn/gtvxdpleso.html

echo "log" >> out.log
来源：http://hz.feifeiyinyue.top/gtgpsygpel.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gtetppwiqg.html


<!-- 参考信息 -->