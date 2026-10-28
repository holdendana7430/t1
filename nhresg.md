代发 wailian999

================================================================================
来源：http://hz.sysykeji.top/gtzeqohtbp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jyoumei.cn/gtkcnuelnc.html

================================================================================
来源：http://hz.cheryme.top/gtysfbswiu.html

[Q01] 创建表
来源：http://hz.ybcxt.top/gtndnwnkzh.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtqnxflyut.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtvkcigclg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tanke756.top/gthkkwqjer.html

email VARCHAR(100) UNIQUE,
来源：http://hz.iojbl.cn/gtazggcvqt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.havefunace.top/gtlvrerlvz.html

);
来源：http://hz.svipenyu.cn/gtxroyyrfv.html

[Q02] 创建带外键的表
来源：http://hz.cheryme.top/gtoogzdela.html

CREATE TABLE orders (
来源：http://hz.jinyuanbaomall.cn/gtmmngkeal.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtdrheavjd.html

user_id INT NOT NULL,
来源：http://hz.zycfv.cn/gtalkblyje.html

amount DECIMAL(10, 2),
来源：http://hz.cucudq.cn/gtkwovogpt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dashuyun.cn/gtudmlrgvi.html

);
来源：http://hz.ybcxt.top/gtibblojsh.html

[Q03] 增加列
来源：http://hz.guannengcc.top/gtbicrkree.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.andypj.xyz/gtkxwgzpjz.html

[Q04] 修改列类型
来源：http://hz.yongpay.top/gtpywxtbmc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgfzy.top/gtvuajoxfv.html

[Q05] 重命名列
来源：http://hz.cashguo.top/gthoaimphe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jyoumei.cn/gtluxlkouq.html

[Q06] 删除列
来源：http://hz.ppjwa.cn/gtlulnvdtb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xziqi.cn/gtwxkccsig.html

[Q07] 删除表
来源：http://hz.hnxiangtu.top/gtevhjrkrg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gtyamxiwng.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtzmiepscz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cqqwz.cn/gttthwbbcz.html

[Q09] 创建唯一索引
来源：http://hz.ydjk.org.cn/gthqgbfoio.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tanke756.top/gtteaapwor.html

[Q10] 插入单行
来源：http://hz.xuanzx.com/gtvmyggfdx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yueranfly.top/gtathkwpmc.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gthlddulpb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.mhx1999.top/gtibpjcvyj.html

[Q12] 插入后取自增 ID
来源：http://hz.wangshuangyany.cn/gttahjaijc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhiwuduotai.top/gtjwgjqfov.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuanzhike.top/gtyxfinvfd.html

[Q13] 忽略重复插入
来源：http://hz.xingfuxueyuan.xyz/gtkcilaxoj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigufen.top/gtxhtmramu.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinyuanbaomall.cn/gtreugvbmo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuetiantiany.cn/gtgellmceo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangdashe.top/gtcajjonol.html

[Q15] 查询全部
来源：http://hz.gogol.net.cn/gtxcttbdny.html

SELECT * FROM users;
来源：http://hz.ydjk.org.cn/gtmiywnnxk.html

[Q16] 查询指定列
来源：http://hz.aibaodan.cn/gtxgmpzlam.html

SELECT id, name FROM users;
来源：http://hz.jinqigufen.top/gtpoeierax.html

[Q17] 条件查询
来源：http://hz.zhijiandao.cn/gteleosblk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yongpay.top/gtlhctaina.html

[Q18] 模糊匹配
来源：http://hz.jyoumei.cn/gtdyooyrib.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ivvv.top/gtngqdlmtu.html

[Q19] 范围查询
来源：http://hz.zhixingplan.top/gtpxzwtpgu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.smart0.xyz/gtpvdcuxnd.html

[Q20] IN 列表
来源：http://hz.haohaochexian.top/gtvibosfsn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.haohaochexian.top/gtxmanluut.html

[Q21] 空值判断
来源：http://hz.aibaodan.cn/gtlvbzreoe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuetiantiany.cn/gtrmyujszf.html

[Q22] 排序
来源：http://hz.redwolf501.top/gtadbuepvg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258.top/gtephmhhmg.html

[Q23] 分页
来源：http://hz.jinqigfzy.top/gthmbcgjai.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yangfankeji.com/gtuegkiuma.html

[Q24] 去重
来源：http://hz.jlsjyb.cn/gtfxykcszg.html

SELECT DISTINCT city FROM users;
来源：http://hz.andypj.xyz/gtehtxsggn.html

[Q25] 只取前 N 条
来源：http://hz.fengsongda.top/gtenmwcldb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.daxiang520.top/gtfjksihll.html

[Q26] 计数
来源：http://hz.yj20258888.top/gtqdxplswg.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtcslajnqa.html

[Q27] 条件计数
来源：http://hz.zhaomingkeji.xyz/gtsxclepta.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shangyingyoupin.top/gtlgncrpuv.html

[Q28] 求和与平均
来源：http://hz.cheryme.top/gtptjsqldy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ppjwa.cn/gtckwryxhx.html

[Q29] 最大最小值
来源：http://hz.daxiang520.top/gtwaydnwmz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangdashe.top/gthuyxqtld.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtfetoqvje.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtrckzqgkq.html

[Q31] 分组后过滤
来源：http://hz.tian-w.cn/gtazczyccw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.9152youxi.cn/gtedgtlqov.html

[Q32] 分组拼接字符串
来源：http://hz.yonumen.top/gtanbuddei.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtuuvnxpxj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ivvv.top/gtnisbwzej.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtotvbdaxy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tian-w.cn/gtiqcvtgyx.html

[Q34] 每组取第一条
来源：http://hz.0kj1m.cn/gtftummzay.html

SELECT * FROM (
来源：http://hz.mhx1999.top/gtgphdteyl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenzaomai.com/gtynavleou.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtvecdefas.html

[Q35] 内连接
来源：http://hz.dianchejie.cn/gtklaxartl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtuhfknsuk.html

[Q36] 左连接
来源：http://hz.wangdashe.top/gtcmkifnqw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtbuecqisq.html

[Q37] 右连接
来源：http://hz.yongpay.top/gtqmtbckbo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xylfe.cn/gtxjgmawur.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jiagoushi.top/gtitytboxf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xziqi.cn/gtyzbpjmeb.html

[Q39] 自连接（查上下级）
来源：http://hz.birdmap.top/gtryhfsyzq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zdqjudy.top/gtugnbrhma.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigfzy.top/gtxeolwuhm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ivvv.top/gtqpqpewuk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigfzy.top/gtvspxaeuk.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtvfrfqrkn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yuanzhike.top/gtlzutbnrf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tanke756.top/gtkrtpjxeb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hywenlv.cn/gthsmhlawm.html

[Q42] 连接条件附加过滤
来源：http://hz.hongshengwenyu.top/gtazdcirua.html

SELECT u.name, o.amount FROM users u
来源：http://hz.c1oappe.top/gtdbciueby.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtjmwojkjl.html

[Q43] 标量子查询
来源：http://hz.xinyue.icu/gtvboagbjz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.quarkkingdee.top/gthzlwslid.html

[Q44] IN 子查询
来源：http://hz.sweek.top/gtghzrvntp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zycfv.cn/gtfipsxnde.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtciomonzq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtnqyplaza.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shzxlz.cn/gtihszerfo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtwmpevrjt.html

[Q47] 与平均值比较
来源：http://hz.jqgufenzy.top/gtjfgadjkh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.mhx1999.top/gtfznzrdvm.html

[Q48] CTE 公用表表达式
来源：http://hz.xinyue.icu/gtbrxwhtfo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.smart0.xyz/gtvtrrqcci.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhaomingkeji.xyz/gttvmfglxw.html

[Q49] 更新单行
来源：http://hz.fengsongda.top/gtuolxqrig.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gtrpessnzk.html

[Q50] 批量更新
来源：http://hz.cashguo.top/gtlqlxjzfk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnxiangtu.top/gthyjmjjfx.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtgcfrqcul.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cdnleiting.top/gtbkaqdlwp.html

[Q52] 删除指定行
来源：http://hz.sxryk.cn/gtjcskuyhv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtqriaelcn.html

[Q53] 按条件删除
来源：http://hz.ppjwa.cn/gtuxkvsdtl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtmlarqclm.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtrzlftfbj.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigfzy.top/gtzngaucim.html

[Q55] 排名（并列占位）
来源：http://hz.shuidangran.top/gtrzgnxzow.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj202588.top/gtltxeozqd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hywenlv.cn/gtgfxmigko.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtxyngllwq.html

[Q57] 行号
来源：http://hz.jlsjyb.cn/gthucdfbai.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gthldpddwm.html

[Q58] 累计求和
来源：http://hz.tanke756.top/gtrkqgorhd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gotoacloud.top/gtthsyjfax.html

[Q59] 分组内累计
来源：http://hz.ppjwa.cn/gthdsjyido.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtzhqyrumc.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtvqbpbysm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nwbrower.top/gtfgtzolxs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtuzgrcnpv.html

[Q61] 移动平均
来源：http://hz.yonumen.top/gtngvkezcn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hnxiangtu.top/gteabodmro.html

[Q62] 分组占比
来源：http://hz.xziqi.cn/gtzwtqongg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtvurufbgi.html

[Q63] 开启事务
来源：http://hz.dianchejie.cn/gtrajvcrge.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sufxvd.cn/gtkhwgnsfd.html

[Q64] 提交事务
来源：http://hz.mhx1999.top/gtelxbbnfw.html

COMMIT;
来源：http://hz.xylfe.cn/gtoorprpkk.html

[Q65] 回滚事务
来源：http://hz.pengpengdd.cyou/gtxogeyjih.html

ROLLBACK;
来源：http://hz.tanke756.top/gtwaenrjxr.html

[Q66] 行锁查询
来源：http://hz.sxryk.cn/gtpkcokndu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cucudq.cn/gtjadqtbyb.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtmxyucbwm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuetiantiany.cn/gtycdboonz.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtqstwogac.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtblcewlxd.html

ROLLBACK TO sp1;
来源：http://hz.cdnleiting.top/gtrcygqtyo.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtcfrcpbvm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtyexecqfh.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtqfxbymwz.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtmdgdstol.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gthnykusay.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hysaishi.cn/gtvugifcvr.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gtwwgjqlhu.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtuqnfqkhx.html

[Q73] 查看表状态
来源：http://hz.ehwqpu.com/gtthabonfn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.haohaochexian.top/gtltqwppcf.html

[Q74] 强制使用索引
来源：http://hz.tian-w.cn/gtskeolkdl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zycfv.cn/gtdzpytdaq.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtwbjmkgcd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guannengcc.top/gturlbxahm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgfzy.top/gtixwhwjep.html

[Q76] 按天统计
来源：http://hz.zhijiandao.cn/gtasmvcisn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.iojbl.cn/gtgbfnrkaz.html

[Q77] 时间加减
来源：http://hz.xuetiantiany.cn/gtfqlkaldr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yongpay.top/gtwbayxfbu.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gttotrleeh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yanxiufei.cn/gtqlqzsjpl.html

[Q79] 字符串拼接
来源：http://hz.hnqzz.top/gtynmoaclc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gtijgmxxdr.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gtsfiujkjs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhengqikj.top/gtatjtccxq.html

[Q81] 字符串替换
来源：http://hz.xziqi.cn/gtayommshn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nwbrower.top/gtzqkeacvz.html

[Q82] 字符长度与字节长度
来源：http://hz.birdmap.top/gtjvjojffz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtkvezpapu.html

[Q83] 大小写转换
来源：http://hz.316326.xyz/gtjuljuxwq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtstsfktvi.html

[Q84] 去除首尾空格
来源：http://hz.gogol.net.cn/gtgopfvuny.html

SELECT TRIM(name) FROM users;
来源：http://hz.tian-w.cn/gtinnjtmwr.html

[Q85] 数值取整
来源：http://hz.ywan-chungtsiang.top/gtzdfvdloc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigufen.top/gtnmfysqtf.html

[Q86] 读取 JSON 字段
来源：http://hz.52xcode.cn/gtwxbqfexr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuetiantiany.cn/gtxlbrkpic.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtbigmakjw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhijiandao.cn/gtxjumwyzq.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigfzy.top/gtjiidzpoi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gttlmosvzg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dashuyun.cn/gtckscjmis.html

[Q89] 判断表是否存在
来源：http://hz.iojbl.cn/gtycswhter.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gtukgnlnws.html

[Q90] 生成序号列
来源：http://hz.dianchejie.cn/gtepjhglmt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cucudq.cn/gttmcjyyhe.html

================================================================================
来源：http://hz.nwbrower.top/gttmulwcpg.html

R. Bash 专题
来源：http://hz.feifeiyinyue.top/gtpmyjvscl.html

================================================================================
来源：http://hz.xinyue.icu/gtqlrhrbms.html

[R01] shebang 与严格模式
来源：http://hz.jiagoushi.top/gtgplvdxlh.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtynujwrxb.html

set -euo pipefail
来源：http://hz.hywenlv.cn/gtdtamalax.html

[R02] 变量赋值与使用
来源：http://hz.tian-w.cn/gttfwqfedg.html

name="Tom"; echo "$name"
来源：http://hz.meibo888.top/gtfbfvyjct.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtjwmzmezv.html

readonly PI=3.14
来源：http://hz.yangfankeji.com/gtgexnxysi.html

[R04] 位置参数
来源：http://hz.nanxinkj.top/gtisrzrftl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenjidiqi.icu/gtpldauitr.html

[R05] 参数默认值
来源：http://hz.mhx1999.top/gtucddbgpo.html

name="${1:-default}"
来源：http://hz.smart0.xyz/gttyvcfiso.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtbvghmnlc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtiskbyayk.html

[R07] if 判断文件
来源：http://hz.sysykeji.top/gtjszyqtjn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhaomingkeji.xyz/gtupthrzwa.html

[R08] 数值比较
来源：http://hz.cqqwz.cn/gtaffkejsf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cucudq.cn/gtftbdxluv.html

[R09] 字符串比较
来源：http://hz.shanyushiyangtech.top/gtlfmpkcts.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258.top/gtnpdmqstc.html

[R10] 正则匹配
来源：http://hz.redwolf501.top/gtrxobpxvx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ppjwa.cn/gtkpqdenwq.html

[R11] case 多分支
来源：http://hz.ydzc1.top/gthwbjiyfv.html

case "$1" in
来源：http://hz.xylfe.cn/gtwknfdaxs.html

start) echo "启动" ;;
来源：http://hz.ywan-chungtsiang.top/gtiduojjdo.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtpnzpqcqa.html

*)     echo "未知命令" ;;
来源：http://hz.0kj1m.cn/gtyjqbrpdp.html

esac
来源：http://hz.ydzc1.top/gtlpdwnhdb.html

[R12] for 遍历文件
来源：http://hz.shangyingyoupin.top/gtfqjfwrux.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtwaghljpp.html

[R13] for 计数循环
来源：http://hz.nanxinkj.top/gtzhcyklkg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuxming.cn/gtaltcxtaa.html

[R14] C 风格 for
来源：http://hz.havefunace.top/gtsykvbllk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cdnleiting.top/gthrpyffah.html

[R15] while 逐行读文件
来源：http://hz.xylfe.cn/gtyjckxghr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangtech.top/gtzjgnwhta.html

[R16] until 等待条件
来源：http://hz.sxryk.cn/gtysslamao.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.kuanghao11.cn/gthmywnpiz.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtvrhnqwyt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hfpthk.cn/gtykdkjbrx.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtpvidakeb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gthkpordbc.html

[R19] 数组长度
来源：http://hz.yj20258888.top/gtzrkkmmtt.html

echo "${#arr[@]}"
来源：http://hz.wangdashe.top/gtzrxetpdl.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtrgrnkprg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hywenlv.cn/gtvawabjwr.html

[R21] 字符串长度
来源：http://hz.sufxvd.cn/gtyofqmftm.html

echo "${#s}"
来源：http://hz.gotoacloud.top/gtqliqbdph.html

[R22] 截取子串
来源：http://hz.guannengcc.top/gtkbhttdlw.html

echo "${s:0:5}"
来源：http://hz.sxryk.cn/gtrhtlihqo.html

[R23] 字符串替换
来源：http://hz.fengsongda.top/gtlghpwxvn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gtgdkwnpio.html

[R24] 大小写转换
来源：http://hz.dashuyun.cn/gtdfyvymwi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.feifeiyinyue.top/gtgsqbvchz.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigfzy.top/gtyaqevrxv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnxiangtu.top/gtavubqnhs.html

[R26] 命令替换
来源：http://hz.jyoumei.cn/gtjxarsdas.html

now=$(date +%F); echo "$now"
来源：http://hz.meibo888.top/gtzltnphfc.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtmswhxpax.html

echo $((1 + 2 * 3))
来源：http://hz.jqgfzy.top/gtqzaekfiq.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtbrolhqsz.html

echo "scale=2; 10/3" | bc
来源：http://hz.zdqjudy.top/gtknhwpfya.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gtbsenxlpm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.0kj1m.cn/gtqqfnxtfq.html

[R30] 函数返回状态码
来源：http://hz.xingfuxueyuan.xyz/gtcgcelxut.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhaomingkeji.xyz/gtvebxlkkz.html

[R31] 局部变量
来源：http://hz.hnqzz.top/gtunqcurwx.html

f() { local x=1; echo "$x"; }
来源：http://hz.meibo888.top/gtucmqnwri.html

[R32] 参数个数校验
来源：http://hz.zhoulong.xyz/gtjieokwks.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gtvcqgmoum.html

[R33] 捕获错误并提示行号
来源：http://hz.sweek.top/gtdoosycym.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xingfuxueyuan.xyz/gtydnraesx.html

[R34] 退出时清理
来源：http://hz.andypj.xyz/gtwaboqqxc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtbmhqjxvf.html

[R35] 后台执行并等待
来源：http://hz.andypj.xyz/gtjtrpnimt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jlsjyb.cn/gtqcpljjhn.html

[R36] 并发执行多个任务
来源：http://hz.shuidangran.top/gtmeypsmgc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.9152youxi.cn/gtvazgjwcc.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtmrjtcumz.html

files=$(ls -1)
来源：http://hz.9152youxi.cn/gtrpublnmk.html

[R38] 管道串联
来源：http://hz.tianlin.xyz/gtleaaojqh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenzaomai.com/gtuwselguo.html

[R39] 重定向标准输出与错误
来源：http://hz.birdmap.top/gtjcccjwlr.html

cmd > out.log 2>&1
来源：http://hz.shuidangran.top/gtxtzxsltx.html

[R40] 追加写日志
来源：http://hz.aizwys.cn/gtqnufngjq.html

echo "log" >> out.log
来源：http://hz.shangyingyoupin.top/gtgqzooboy.html

[R41] 丢弃输出
来源：http://hz.ydzc1.top/gttzsmyazj.html

cmd >/dev/null 2>&1
来源：http://hz.jqgufenzy.top/gtgkgmjoep.html

[R42] 输入重定向
来源：http://hz.aibaodan.cn/gtqdiemvmb.html

wc -l < a.txt
来源：http://hz.yj20258.top/gtltbdnlvp.html

[R43] 按名字查找文件
来源：http://hz.hongshengwenyu.top/gtchysywby.html


<!-- 参考信息 -->