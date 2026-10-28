代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.smart0.xyz/gtpicsokme.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangshuangyany.cn/gtozsjxvgj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhongyouzk.top/gtzmqcxees.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gogol.net.cn/gthiydhlib.html

================================================================================
来源：http://hz.chenzaomai.com/gtdltjydhc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinghuilouyu.cn/gtybzoamus.html

================================================================================
来源：http://hz.zhijiandao.cn/gtoxggbvji.html

[Q01] 创建表
来源：http://hz.jlsjyb.cn/gtsocftuze.html

CREATE TABLE users (
来源：http://hz.nanxinkj.top/gtevsvckpx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtatrdqnig.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gzhubu.top/gtufweaogx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenjidiqi.icu/gtrjvkvbix.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.0kj1m.cn/gtsktifbag.html

);
来源：http://hz.9152youxi.cn/gtaebvencd.html

[Q02] 创建带外键的表
来源：http://hz.gotoacloud.top/gtopiojqgk.html

CREATE TABLE orders (
来源：http://hz.jinghuilouyu.cn/gtywqtbzcb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gthbftovhb.html

user_id INT NOT NULL,
来源：http://hz.cdnleiting.top/gtqrvybtfg.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtztqgwrar.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.haohaochexian.top/gtttzldcrl.html

);
来源：http://hz.hnqzz.top/gtglhvxveh.html

[Q03] 增加列
来源：http://hz.nanxinkj.top/gtvnlundov.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xinyue.icu/gthrhcbcrd.html

[Q04] 修改列类型
来源：http://hz.fengsongda.top/gtjutlqeov.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yvedp.cn/gthjtkvydc.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtshqylhwd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxinkj.top/gtlnwnytlw.html

[Q06] 删除列
来源：http://hz.nwbrower.top/gtbqpdtkku.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhaomingkeji.xyz/gtpivslnio.html

[Q07] 删除表
来源：http://hz.zhoulong.xyz/gtoxvxlthh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhiwuduotai.top/gtcsgiivik.html

[Q08] 创建普通索引
来源：http://hz.dashuyun.cn/gtrkkemvsc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yuanzhike.top/gtuunlgyhn.html

[Q09] 创建唯一索引
来源：http://hz.mhx1999.top/gtplikzimj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtgqtsisyk.html

[Q10] 插入单行
来源：http://hz.sweek.top/gtauyyzogc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuanzx.com/gtfdqoiiri.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtyyzqvaox.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.meibo888.top/gtinxfzjci.html

[Q12] 插入后取自增 ID
来源：http://hz.aizwys.cn/gtlbmsipdy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtsvzeplyr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.vqdsnc.cn/gtbokmouex.html

[Q13] 忽略重复插入
来源：http://hz.jinyuanbaomall.cn/gtikdpzksa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.haohaochexian.top/gtpkwelydx.html

[Q14] 存在则更新（upsert）
来源：http://hz.hysaishi.cn/gtmllrzyjb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xylfe.cn/gtimcfkeuy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.redwolf501.top/gtgghtwifs.html

[Q15] 查询全部
来源：http://hz.aizwys.cn/gtwvrpdlez.html

SELECT * FROM users;
来源：http://hz.jqgufenzy.top/gtekdjftxo.html

[Q16] 查询指定列
来源：http://hz.nwbrower.top/gtdxtkyqyf.html

SELECT id, name FROM users;
来源：http://hz.cqqwz.cn/gtymurzhlq.html

[Q17] 条件查询
来源：http://hz.yueranfly.top/gtkwvugisj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aizwys.cn/gtpmydmrob.html

[Q18] 模糊匹配
来源：http://hz.xuetiantiany.cn/gtdfhubcio.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gtvemooefj.html

[Q19] 范围查询
来源：http://hz.redwolf501.top/gtroljhmgm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgfzy.top/gterovmykm.html

[Q20] IN 列表
来源：http://hz.aibaodan.cn/gtinnvrgtr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtjibyygiq.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtxgcdxinz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhixingplan.top/gthaqxenpm.html

[Q22] 排序
来源：http://hz.jinqigfzy.top/gthfffqfyv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtlpheiadl.html

[Q23] 分页
来源：http://hz.guowangkeji.top/gttmwcjfda.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gtdlsudnke.html

[Q24] 去重
来源：http://hz.aibaodan.cn/gtgifvtrvi.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtyyrfuxvv.html

[Q25] 只取前 N 条
来源：http://hz.aibaodan.cn/gtmcaynaql.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aizwys.cn/gtgxcwrjko.html

[Q26] 计数
来源：http://hz.fengsongda.top/gtlfjfiego.html

SELECT COUNT(*) FROM users;
来源：http://hz.feifeiyinyue.top/gtmppmsxtz.html

[Q27] 条件计数
来源：http://hz.ivvv.top/gttpudqpih.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangdashe.top/gtikuocfak.html

[Q28] 求和与平均
来源：http://hz.hammf.cn/gtvlmwnhqe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.316326.xyz/gtsalkcxrj.html

[Q29] 最大最小值
来源：http://hz.zhijiandao.cn/gtmuqvvlxg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ywan-chungtsiang.top/gttcaopqev.html

[Q30] 分组统计
来源：http://hz.daxiang520.top/gtiykjhcok.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtmkqmwpns.html

[Q31] 分组后过滤
来源：http://hz.yonumen.top/gtihqjucyy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gtziqhgswk.html

[Q32] 分组拼接字符串
来源：http://hz.yuxming.cn/gtzlatpulr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtahmrydzs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sweek.top/gtpitlrooo.html

[Q33] 多列分组
来源：http://hz.xingfuxueyuan.xyz/gtwnufoyvm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.feifeiyinyue.top/gtlnjgniux.html

[Q34] 每组取第一条
来源：http://hz.zycfv.cn/gtgxcaltnf.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gtatqrthvv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xinyue.icu/gtotjlmwlt.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtujfwfonm.html

[Q35] 内连接
来源：http://hz.sufxvd.cn/gtrpiotaqo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtvmpnamtq.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gtyqtjcgcl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtpylxvvgi.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gtiuzrkzav.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtoagkixea.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pycfn.com/gtzgzrgbru.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ppjwa.cn/gttnewsmde.html

[Q39] 自连接（查上下级）
来源：http://hz.sxryk.cn/gtfzdqspfv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydjk.org.cn/gtlccxaotl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gtszjpgspj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhijiandao.cn/gtnpaibwet.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daria6918.cn/gttkuvqvpq.html

[Q41] 多表连接
来源：http://hz.jqgfzy.top/gtvmypjvif.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ivvv.top/gtaeuusayj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.redwolf501.top/gtngwoxlhj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yangfankeji.com/gtkisnqhco.html

[Q42] 连接条件附加过滤
来源：http://hz.ehwqpu.com/gtajqwdhkt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jqgfzy.top/gthpczsdkg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hnxiangtu.top/gtxnpxtznh.html

[Q43] 标量子查询
来源：http://hz.cdnleiting.top/gteftxgatz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daria6918.cn/gtmoxewdkn.html

[Q44] IN 子查询
来源：http://hz.yj20258888.top/gtchvbsedc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fzhhl.top/gtdogqvdsp.html

[Q45] EXISTS 判断存在
来源：http://hz.316326.xyz/gthoajweql.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtaknsppvn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.bjfxy.top/gtbmoiwvzt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gttxvxbusv.html

[Q47] 与平均值比较
来源：http://hz.jinghuilouyu.cn/gtdwsazxbz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aizwys.cn/gtucttpdou.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtoaidiqns.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pycfn.com/gtdmpofyih.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtmcomrvtu.html

[Q49] 更新单行
来源：http://hz.zhengqikj.top/gtdzgaklor.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xylfe.cn/gtxblphloq.html

[Q50] 批量更新
来源：http://hz.gotoacloud.top/gtxafnfuyk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ywan-chungtsiang.top/gtxawpzgcp.html

[Q51] 用子查询更新
来源：http://hz.wangshuangyany.cn/gtyqhmphba.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtotjptzzo.html

[Q52] 删除指定行
来源：http://hz.zhaomingkeji.xyz/gtdbrskddo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fengsongda.top/gtkwwqypxt.html

[Q53] 按条件删除
来源：http://hz.daxiang520.top/gtqqlyrrhp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cheryme.top/gtjqracigb.html

[Q54] 清空表
来源：http://hz.quarkkingdee.top/gtioxelvla.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gtiadghqef.html

[Q55] 排名（并列占位）
来源：http://hz.guowangkeji.top/gtkkdwqbvr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hammf.cn/gtlmvrjgug.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shzxlz.cn/gtocmkimsa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ybcxt.top/gtapgijrph.html

[Q57] 行号
来源：http://hz.fengsongda.top/gtbnayspmk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigufen.top/gtrqnnadrt.html

[Q58] 累计求和
来源：http://hz.hongshengwenyu.top/gtocaxomoe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gtixdgsmbb.html

[Q59] 分组内累计
来源：http://hz.yonumen.top/gtlvhybnww.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.haohaochexian.top/gtqkimhvih.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtusugmevk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hywenlv.cn/gtzspyzfnf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.vqdsnc.cn/gtimjhkmcd.html

[Q61] 移动平均
来源：http://hz.yuanzhike.top/gtagrnujuv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ehwqpu.com/gtuaicihuz.html

[Q62] 分组占比
来源：http://hz.ehwqpu.com/gtxkfzgeub.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gtdmlednsw.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gtxhzsmqwy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gaohongyu789.top/gtkknhamei.html

[Q64] 提交事务
来源：http://hz.jqgufenzy.top/gtdkxlravl.html

COMMIT;
来源：http://hz.sysykeji.top/gtmkabdbcr.html

[Q65] 回滚事务
来源：http://hz.9152youxi.cn/gtnduknnrc.html

ROLLBACK;
来源：http://hz.shzxlz.cn/gtfdubbihr.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gtvpqmwiwd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gtsgmxgqlh.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gttnoqydch.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gtdmacscbk.html

[Q68] 保存点
来源：http://hz.sysykeji.top/gtdvvdmils.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtcqbastba.html

ROLLBACK TO sp1;
来源：http://hz.fengsongda.top/gtcjggfhwh.html

[Q69] 查看执行计划
来源：http://hz.jlsjyb.cn/gthcqulmsh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.guannengcc.top/gtgrskopws.html

[Q70] 更新统计信息
来源：http://hz.redwolf501.top/gtvnezazbn.html

ANALYZE TABLE users;
来源：http://hz.yj20258.top/gtaqdxvlrb.html

[Q71] 查看建表语句
来源：http://hz.hammf.cn/gtmlomwtms.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aizwys.cn/gtsiowtlnf.html

[Q72] 查看索引
来源：http://hz.gaohongyu789.top/gtchvinirm.html

SHOW INDEX FROM users;
来源：http://hz.zhijiandao.cn/gtlgqrmzfr.html

[Q73] 查看表状态
来源：http://hz.ivvv.top/gtdwcsiqhl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhongyouzk.top/gtxcstqoxm.html

[Q74] 强制使用索引
来源：http://hz.xuanzx.com/gtncwgiser.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuetiantiany.cn/gtogkyohqt.html

[Q75] 日期格式化
来源：http://hz.yueranfly.top/gtonpcuxjs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.mhx1999.top/gtacxfgwem.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yongpay.top/gtfmchokfo.html

[Q76] 按天统计
来源：http://hz.sweek.top/gtugvpdrxu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zycfv.cn/gttujvaini.html

[Q77] 时间加减
来源：http://hz.jiagoushi.top/gtluhnetie.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zdqjudy.top/gtdwlpjmqy.html

[Q78] 当前时间
来源：http://hz.jinghuilouyu.cn/gteulpufwp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.316326.xyz/gtfjnvejre.html

[Q79] 字符串拼接
来源：http://hz.pycfn.com/gtvyrahcbx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yuxming.cn/gtnxitbomf.html

[Q80] 字符串截取
来源：http://hz.dianchejie.cn/gtdhregdjf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtcqdbdgmk.html

[Q81] 字符串替换
来源：http://hz.xingfuxueyuan.xyz/gtldowaisg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zdqjudy.top/gtzezxdafa.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxuanxn.top/gtuhsqssfh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnqzz.top/gtatdwraai.html

[Q83] 大小写转换
来源：http://hz.wangshuangyany.cn/gtiuuxjqjt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.bjfxy.top/gtcpynrlig.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gtwmjvsgku.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigufen.top/gthyxaqprg.html

[Q85] 数值取整
来源：http://hz.yuxming.cn/gtthkkklom.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shuidangran.top/gtrardneqg.html

[Q86] 读取 JSON 字段
来源：http://hz.guannengcc.top/gtodftjcdu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gtxpemceqx.html

[Q87] JSON 字段做条件
来源：http://hz.yongpay.top/gtdkafocrl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgfzy.top/gtzgglzwgv.html

[Q88] 行转列（条件聚合）
来源：http://hz.yueranfly.top/gtebrdcajy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigfzy.top/gtbwxfnudy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.redwolf501.top/gtadoactzz.html

[Q89] 判断表是否存在
来源：http://hz.hongshengwenyu.top/gttsfysnaf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shzxlz.cn/gtrdznekwc.html

[Q90] 生成序号列
来源：http://hz.yonumen.top/gtyujccacn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aibaodan.cn/gtqpyscirt.html

================================================================================
来源：http://hz.0kj1m.cn/gthlcmewgz.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtsywipdrg.html

================================================================================
来源：http://hz.guannengcc.top/gtqxodlrnl.html

[R01] shebang 与严格模式
来源：http://hz.dashuyun.cn/gtiqwflzfs.html

#!/usr/bin/env bash
来源：http://hz.gotoacloud.top/gtroyatguo.html

set -euo pipefail
来源：http://hz.ydjk.org.cn/gtgccrcgrq.html

[R02] 变量赋值与使用
来源：http://hz.snrcjt.cn/gttyfbbzzm.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gtbrotapkj.html

[R03] 只读变量
来源：http://hz.zhongyouzk.top/gtmsbpasgb.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtrokidqec.html

[R04] 位置参数
来源：http://hz.sweek.top/gtxdnkrknn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.birdmap.top/gtnhqygrwv.html

[R05] 参数默认值
来源：http://hz.9152youxi.cn/gtpefxwrdh.html

name="${1:-default}"
来源：http://hz.svipenyu.cn/gtkhrynnyr.html

[R06] 判断命令是否存在
来源：http://hz.cashguo.top/gtdjguyhol.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtojqxbxst.html

[R07] if 判断文件
来源：http://hz.zhengqikj.top/gtandvjikv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.mhx1999.top/gtmntmenxk.html

[R08] 数值比较
来源：http://hz.tianlin.xyz/gtdtsvrorn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuanzhike.top/gtjnmsjcod.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gtycyiutes.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtaecfahme.html

[R10] 正则匹配
来源：http://hz.ydjk.org.cn/gtmrjlriub.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sufxvd.cn/gtvgsfjqti.html

[R11] case 多分支
来源：http://hz.0kj1m.cn/gtxfzxsboc.html

case "$1" in
来源：http://hz.gogol.net.cn/gtvjbdtfvp.html

start) echo "启动" ;;
来源：http://hz.yongpay.top/gtyqynnnui.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtfdhdokts.html

*)     echo "未知命令" ;;
来源：http://hz.jiagoushi.top/gtxylaalqy.html

esac
来源：http://hz.hfpthk.cn/gtubvjokzn.html

[R12] for 遍历文件
来源：http://hz.dianchejie.cn/gtqhhqcisl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtbighrtdz.html

[R13] for 计数循环
来源：http://hz.316326.xyz/gtepxdcszv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtznuphxnh.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtxgqtfysl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ehwqpu.com/gtwdniwqmw.html

[R15] while 逐行读文件
来源：http://hz.hywenlv.cn/gtyjnevhmw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yanxiufei.cn/gtfbvvdaam.html

[R16] until 等待条件
来源：http://hz.yueranfly.top/gtisuwshxk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtipopjzdc.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtaszbjjof.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.c1oappe.top/gtclbegiqr.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtswthtpxr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cqqwz.cn/gtevphubeu.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtzsbudsbf.html

echo "${#arr[@]}"
来源：http://hz.ehwqpu.com/gtfbhwltmq.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtisivnlzv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinyuanbaomall.cn/gtykzhfbrs.html

[R21] 字符串长度
来源：http://hz.jianghu66.top/gtvfeognew.html

echo "${#s}"
来源：http://hz.ydzc1.top/gttdcmpwcj.html

[R22] 截取子串
来源：http://hz.hongshengwenyu.top/gtktimlbwr.html

echo "${s:0:5}"
来源：http://hz.ybcxt.top/gtdbmasngh.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtfrxyvwkb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sysykeji.top/gtuucjhvlt.html

[R24] 大小写转换
来源：http://hz.cucudq.cn/gtyujzhemj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuanzx.com/gtukhebywa.html

[R25] 去后缀 / 去前缀
来源：http://hz.yvedp.cn/gtsjcxgqjm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fengsongda.top/gtveqzhtac.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtzovzmahm.html

now=$(date +%F); echo "$now"
来源：http://hz.smart0.xyz/gtvzqajmpq.html

[R27] 算术展开
来源：http://hz.snrcjt.cn/gtuurrlzmn.html

echo $((1 + 2 * 3))
来源：http://hz.feifeiyinyue.top/gtylwyeflw.html

[R28] 浮点运算
来源：http://hz.yuanzhike.top/gtessixzky.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhongyouzk.top/gtqmizlnwo.html

[R29] 定义函数
来源：http://hz.iojbl.cn/gtimfmdthq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yangfankeji.com/gtbgckcsqp.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtxspxhswd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtgkhntisv.html

[R31] 局部变量
来源：http://hz.xylfe.cn/gtxniyerxm.html

f() { local x=1; echo "$x"; }
来源：http://hz.tanke756.top/gtknfdgenv.html

[R32] 参数个数校验
来源：http://hz.jqgufenzy.top/gtmaeimcjs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgfzy.top/gthufvlhiw.html

[R33] 捕获错误并提示行号
来源：http://hz.wangdashe.top/gtcxmlyevz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ehwqpu.com/gtwkcyccwv.html

[R34] 退出时清理
来源：http://hz.xziqi.cn/gtrrjcczdn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtawnvudza.html

[R35] 后台执行并等待
来源：http://hz.yongpay.top/gtaulfhdlu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenzaomai.com/gtabqpnmsu.html

[R36] 并发执行多个任务
来源：http://hz.hywenlv.cn/gtpjqmyayp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtvqsukpsy.html

[R37] 把输出赋给变量
来源：http://hz.zycfv.cn/gtxdyparwk.html

files=$(ls -1)
来源：http://hz.wangshuangyany.cn/gtqiebymaw.html

[R38] 管道串联
来源：http://hz.yuxming.cn/gtnzwxkjsd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yvedp.cn/gthjiaxhgg.html

[R39] 重定向标准输出与错误
来源：http://hz.ywan-chungtsiang.top/gtpwxwrvsc.html

cmd > out.log 2>&1
来源：http://hz.xuanzx.com/gtwjwzseli.html

[R40] 追加写日志
来源：http://hz.cdnleiting.top/gtqgemmnzi.html

echo "log" >> out.log
来源：http://hz.ydjk.org.cn/gtbqfmqujk.html

[R41] 丢弃输出
来源：http://hz.xuanzx.com/gtngfkzmms.html


<!-- 参考信息 -->