代发 wailian999

================================================================================
来源：http://hz.chenlongwang.top/gtsirdibrw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xinyue.icu/gtggommwjg.html

================================================================================
来源：http://hz.nanxuanxn.top/gtfpqgddaf.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gtlezvdhxe.html

CREATE TABLE users (
来源：http://hz.ywan-chungtsiang.top/gtoqeebtde.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtshcismta.html

name VARCHAR(50) NOT NULL,
来源：http://hz.feifeiyinyue.top/gtczlmbujd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xziqi.cn/gtbtqotykr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenjidiqi.icu/gtcsnauxgg.html

);
来源：http://hz.yvedp.cn/gthmttcwjm.html

[Q02] 创建带外键的表
来源：http://hz.jianghu66.top/gtpnwrqohj.html

CREATE TABLE orders (
来源：http://hz.jqgufenzy.top/gtwnzjszrf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtaxuovwdr.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtpktbquer.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtyxswqdyc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtqhofqovq.html

);
来源：http://hz.gotoacloud.top/gtcipzaumv.html

[Q03] 增加列
来源：http://hz.xingfuxueyuan.xyz/gtwlzmybvv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dashuyun.cn/gtcfkvfmcm.html

[Q04] 修改列类型
来源：http://hz.yongpay.top/gteojndeze.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.smart0.xyz/gtjwojeool.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtcrjiihdr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.chenlongwang.top/gtnxptlakj.html

[Q06] 删除列
来源：http://hz.yongpay.top/gthclnbkat.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ybcxt.top/gtwvudvadu.html

[Q07] 删除表
来源：http://hz.zdqjudy.top/gtrihakhza.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tianlin.xyz/gteoasrsmk.html

[Q08] 创建普通索引
来源：http://hz.zhaomingkeji.xyz/gtulrjhiql.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fzhhl.top/gtvmfxiqro.html

[Q09] 创建唯一索引
来源：http://hz.dashuyun.cn/gtmubxxtva.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.smart0.xyz/gtfaoswwws.html

[Q10] 插入单行
来源：http://hz.kuanghao11.cn/gtmetgpfow.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cashguo.top/gtkejzhxpf.html

[Q11] 一次插入多行
来源：http://hz.xuanzx.com/gtrehfpmhi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangshuangyany.cn/gtsubugqec.html

[Q12] 插入后取自增 ID
来源：http://hz.hysaishi.cn/gtfifqctaq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.birdmap.top/gtblgrvois.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj202588.top/gtbptvzlnw.html

[Q13] 忽略重复插入
来源：http://hz.cucudq.cn/gtjgzwiowy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gotoacloud.top/gtdutqfrqy.html

[Q14] 存在则更新（upsert）
来源：http://hz.sufxvd.cn/gtiwzahzuk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258888.top/gtflhcawhy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zdqjudy.top/gtyqiilygx.html

[Q15] 查询全部
来源：http://hz.gotoacloud.top/gtasvbetts.html

SELECT * FROM users;
来源：http://hz.sweek.top/gtadoqftme.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtykevpflj.html

SELECT id, name FROM users;
来源：http://hz.gzhubu.top/gtewuvxesz.html

[Q17] 条件查询
来源：http://hz.dashuyun.cn/gtvfyfhsfc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yanxiufei.cn/gtjundhffk.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtqmfklrvt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gthhepnxnj.html

[Q19] 范围查询
来源：http://hz.wangshuangyany.cn/gtyyiacylj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.aibaodan.cn/gtzcnqzpwg.html

[Q20] IN 列表
来源：http://hz.chenlongwang.top/gtssgtzbwy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhengqikj.top/gtsetbkbuu.html

[Q21] 空值判断
来源：http://hz.jinyuanbaomall.cn/gtrgwekbwe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sweek.top/gtsknijtnt.html

[Q22] 排序
来源：http://hz.shanyushiyangkeji.top/gtbzgbvfun.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuetiantiany.cn/gtzjwyxird.html

[Q23] 分页
来源：http://hz.nwbrower.top/gtkigvowzw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.quarkkingdee.top/gtwzmhffjz.html

[Q24] 去重
来源：http://hz.cucudq.cn/gtearrlwgl.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258888.top/gtmupvwxth.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtwhfeuwem.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.andypj.xyz/gtnlbnwjim.html

[Q26] 计数
来源：http://hz.shzxlz.cn/gtcuqgsdwv.html

SELECT COUNT(*) FROM users;
来源：http://hz.sweek.top/gtlfsocrit.html

[Q27] 条件计数
来源：http://hz.shzxlz.cn/gtaigaygve.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cashguo.top/gtvquynfph.html

[Q28] 求和与平均
来源：http://hz.yuxming.cn/gtyuvlizco.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtcfjiwikk.html

[Q29] 最大最小值
来源：http://hz.shzxlz.cn/gtyzrxqdtd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cheryme.top/gtakzrziep.html

[Q30] 分组统计
来源：http://hz.hammf.cn/gtsmuwqxcd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtxtgspwzp.html

[Q31] 分组后过滤
来源：http://hz.ybcxt.top/gtkwpjmzkv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zycfv.cn/gtnxulfrvg.html

[Q32] 分组拼接字符串
来源：http://hz.daxiang520.top/gtfoufvfht.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtknbfsyrb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xuanzx.com/gtleodqcal.html

[Q33] 多列分组
来源：http://hz.birdmap.top/gtqvvhnefk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yonumen.top/gtibuvellq.html

[Q34] 每组取第一条
来源：http://hz.cqqwz.cn/gtogqupfyg.html

SELECT * FROM (
来源：http://hz.jiagoushi.top/gtipsbivby.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnxiangtu.top/gtycphfbnk.html

) t WHERE rn = 1;
来源：http://hz.nanxinkj.top/gtxgfpdacx.html

[Q35] 内连接
来源：http://hz.pengpengdd.cyou/gtjvqnqqwk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtforjjnrr.html

[Q36] 左连接
来源：http://hz.zdqjudy.top/gtqhjrslve.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gttqgccahk.html

[Q37] 右连接
来源：http://hz.dashuyun.cn/gtezsrugcd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.svipenyu.cn/gtfqkwdbce.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.dianchejie.cn/gttlcuamtb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnxiangtu.top/gtiezfvagh.html

[Q39] 自连接（查上下级）
来源：http://hz.xuetiantiany.cn/gtgoggnirw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhoulong.xyz/gtihminupk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zycfv.cn/gtknhlkqpb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yvedp.cn/gtyeynzllk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yangfankeji.com/gtsjqisxav.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtspqmdrpi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtgmlbqbsl.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhixingplan.top/gtirgqhxup.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jiagoushi.top/gtugdppefi.html

[Q42] 连接条件附加过滤
来源：http://hz.hammf.cn/gtulsvdldd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinghuilouyu.cn/gtxsbqqyrr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hnxiangtu.top/gteosndwao.html

[Q43] 标量子查询
来源：http://hz.yj202588.top/gtidiulvhh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cdnleiting.top/gtfvqprrvr.html

[Q44] IN 子查询
来源：http://hz.ivvv.top/gtiyyiqgsw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.bjfxy.top/gtlgfdinde.html

[Q45] EXISTS 判断存在
来源：http://hz.cheryme.top/gtftxniaqp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gtvqnvipcn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtilssubdv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtpskvaveo.html

[Q47] 与平均值比较
来源：http://hz.chenlongwang.top/gtqzsqfftl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxuanxn.top/gtuxzbvtmb.html

[Q48] CTE 公用表表达式
来源：http://hz.redwolf501.top/gtxenbfufz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yueranfly.top/gtqaiekjfu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtchzntyve.html

[Q49] 更新单行
来源：http://hz.gzhubu.top/gtebarksws.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtyfoipeyg.html

[Q50] 批量更新
来源：http://hz.gogol.net.cn/gtkysdsusr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aibaodan.cn/gtvlqlcyrb.html

[Q51] 用子查询更新
来源：http://hz.xuetiantiany.cn/gtonnumtzk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zdqjudy.top/gtgawngpeg.html

[Q52] 删除指定行
来源：http://hz.zhixingplan.top/gtcefbzzlr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nwbrower.top/gtcqtxztke.html

[Q53] 按条件删除
来源：http://hz.jinghuilouyu.cn/gtgxjdypzg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.c1oappe.top/gthaqsqkup.html

[Q54] 清空表
来源：http://hz.jqgufenzy.top/gtofcjcjxf.html

TRUNCATE TABLE logs;
来源：http://hz.meibo888.top/gtlxyrpiov.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtjqjvssor.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nwbrower.top/gtibccgine.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sxryk.cn/gtgxznfbuj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtebgxvjel.html

[Q57] 行号
来源：http://hz.snrcjt.cn/gtmjhdwkez.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtmvitkhfo.html

[Q58] 累计求和
来源：http://hz.quarkkingdee.top/gtwvbgsawh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guowangkeji.top/gtdquthavb.html

[Q59] 分组内累计
来源：http://hz.jinqigfzy.top/gtbbkucomk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jianghu66.top/gtzchhrcwf.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtilnfhkmy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.svipenyu.cn/gtndhkdehs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gtzmakdywu.html

[Q61] 移动平均
来源：http://hz.gotoacloud.top/gtagcunnqb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhoulong.xyz/gtcpzlahld.html

[Q62] 分组占比
来源：http://hz.nanxinkj.top/gtamkzoojc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtazhheocx.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtbomsiffy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gzhubu.top/gtafwvhcsz.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtbfsggbtb.html

COMMIT;
来源：http://hz.smart0.xyz/gttaaibkds.html

[Q65] 回滚事务
来源：http://hz.c1oappe.top/gtmxjznivg.html

ROLLBACK;
来源：http://hz.c1oappe.top/gtdnwjavuh.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gtrfdyqggc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gtjldoyerz.html

[Q67] 设置隔离级别
来源：http://hz.mhx1999.top/gtougrfbpn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aizwys.cn/gtlxjxoqfa.html

[Q68] 保存点
来源：http://hz.jinyuanbaomall.cn/gtibayuhat.html

SAVEPOINT sp1;
来源：http://hz.zycfv.cn/gtwawmirrt.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gtdaeaovmi.html

[Q69] 查看执行计划
来源：http://hz.hfpthk.cn/gtxyzwtdbq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.havefunace.top/gtcozkuija.html

[Q70] 更新统计信息
来源：http://hz.cheryme.top/gteklewuva.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gteieifstv.html

[Q71] 查看建表语句
来源：http://hz.zhaomingkeji.xyz/gtuymuwqfg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258.top/gtxzumvebw.html

[Q72] 查看索引
来源：http://hz.zhijiandao.cn/gtxkpmrxcy.html

SHOW INDEX FROM users;
来源：http://hz.xinyue.icu/gtyddzedyn.html

[Q73] 查看表状态
来源：http://hz.sweek.top/gthonywihs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.iojbl.cn/gtuqeidsnj.html

[Q74] 强制使用索引
来源：http://hz.meibo888.top/gtbqxvnvij.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.9152youxi.cn/gtemicehbd.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gtncsvqtcj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtqvjgnjcg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtushlizgq.html

[Q76] 按天统计
来源：http://hz.quarkkingdee.top/gtqlieeuyf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yongpay.top/gtmtdxdknu.html

[Q77] 时间加减
来源：http://hz.shuidangran.top/gtbqnjbzbo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj202588.top/gtshkmxzav.html

[Q78] 当前时间
来源：http://hz.haohaochexian.top/gtoicbifwn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cheryme.top/gthfrhhoge.html

[Q79] 字符串拼接
来源：http://hz.jinghuilouyu.cn/gtivhaxtne.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhiwuduotai.top/gtfhfilpaw.html

[Q80] 字符串截取
来源：http://hz.zhongyouzk.top/gtfvearqjp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jiagoushi.top/gtrrjznvda.html

[Q81] 字符串替换
来源：http://hz.yuxming.cn/gtquulfyka.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtixuovijy.html

[Q82] 字符长度与字节长度
来源：http://hz.quarkkingdee.top/gtbibibvrd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gthyhvklzb.html

[Q83] 大小写转换
来源：http://hz.cheryme.top/gtcovlnmus.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtfitbmgpp.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gtpsgplbag.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhengqikj.top/gtatnprgvx.html

[Q85] 数值取整
来源：http://hz.jinqigfzy.top/gtzgvcodxv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sufxvd.cn/gtewbwozco.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigufen.top/gtghpntrqg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigufen.top/gtjtpsgqdt.html

[Q87] JSON 字段做条件
来源：http://hz.jyoumei.cn/gtcwfwkffy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258888.top/gttiifwwct.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258.top/gtbqdhstob.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangshuangyany.cn/gtyrccfqrw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgfzy.top/gtpvkuxilh.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtqnyxqudn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhongyouzk.top/gtwelttoao.html

[Q90] 生成序号列
来源：http://hz.chenzaomai.com/gtbrudexvw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtmwpruhsa.html

================================================================================
来源：http://hz.cdnleiting.top/gtzawacwkb.html

R. Bash 专题
来源：http://hz.birdmap.top/gthxeepxns.html

================================================================================
来源：http://hz.meibo888.top/gtzkixtzvw.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtplkzacvo.html

#!/usr/bin/env bash
来源：http://hz.snrcjt.cn/gtrjnwqwgm.html

set -euo pipefail
来源：http://hz.ydzc1.top/gttmmcsjjq.html

[R02] 变量赋值与使用
来源：http://hz.jinyuanbaomall.cn/gtkoukjbji.html

name="Tom"; echo "$name"
来源：http://hz.chenjidiqi.icu/gtnevbnjsj.html

[R03] 只读变量
来源：http://hz.zhixingplan.top/gtqznmxdhj.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gttesuvgkx.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtkmcrefww.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gtblhoxvbl.html

[R05] 参数默认值
来源：http://hz.fengsongda.top/gtcsaaohag.html

name="${1:-default}"
来源：http://hz.yj20258888.top/gtqouoiiss.html

[R06] 判断命令是否存在
来源：http://hz.jqgfzy.top/gtjnrhmfmr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtuljmkuwt.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gtlyvkyxjo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cheryme.top/gtzycoskui.html

[R08] 数值比较
来源：http://hz.hongshengwenyu.top/gtpolnqcdc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.vqdsnc.cn/gtjviftlnp.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtdysapgxh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.wangdashe.top/gttkxwecmx.html

[R10] 正则匹配
来源：http://hz.yonumen.top/gthgcwfyds.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yvedp.cn/gtxgulmhju.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtuojdxcfl.html

case "$1" in
来源：http://hz.jlsjyb.cn/gttwwqqqav.html

start) echo "启动" ;;
来源：http://hz.hnqzz.top/gtbjpafkem.html

stop)  echo "停止" ;;
来源：http://hz.xuanzx.com/gtsknudqjb.html

*)     echo "未知命令" ;;
来源：http://hz.ehwqpu.com/gtjwghtdyi.html

esac
来源：http://hz.jinyuanbaomall.cn/gtcetafylo.html

[R12] for 遍历文件
来源：http://hz.hywenlv.cn/gtirqgxxma.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ywan-chungtsiang.top/gtejmosibb.html

[R13] for 计数循环
来源：http://hz.hysaishi.cn/gtihejxhni.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtfjemgnav.html

[R14] C 风格 for
来源：http://hz.jiagoushi.top/gtyrlukdek.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dashuyun.cn/gtaplhyevl.html

[R15] while 逐行读文件
来源：http://hz.hnqzz.top/gtplgprprc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hysaishi.cn/gtbcmvvolz.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gtnveypjur.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenzaomai.com/gtsvsgebqv.html

[R17] 数组定义与取值
来源：http://hz.yj20258888.top/gtrzirozki.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtbdyevkoo.html

[R18] 遍历数组
来源：http://hz.jlsjyb.cn/gtqzlsifjk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yongpay.top/gthnkentjd.html

[R19] 数组长度
来源：http://hz.jqgufenzy.top/gtnbaxbhdu.html

echo "${#arr[@]}"
来源：http://hz.hfpthk.cn/gtwxteexhz.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtrvkdmbei.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.guannengcc.top/gtfumsdyjm.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtqcfdjjpe.html

echo "${#s}"
来源：http://hz.zdqjudy.top/gtplukdmnz.html

[R22] 截取子串
来源：http://hz.yvedp.cn/gttqseyptc.html

echo "${s:0:5}"
来源：http://hz.316326.xyz/gtamyymwag.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtahlfhlns.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtgcqquvva.html

[R24] 大小写转换
来源：http://hz.quarkkingdee.top/gtfknsacqe.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guannengcc.top/gtnvqulgdx.html

[R25] 去后缀 / 去前缀
来源：http://hz.yanxiufei.cn/gtqanjhals.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258.top/gtndvgbnzg.html

[R26] 命令替换
来源：http://hz.hnqzz.top/gtvepsgkqn.html

now=$(date +%F); echo "$now"
来源：http://hz.andypj.xyz/gtqpcbxajd.html

[R27] 算术展开
来源：http://hz.ivvv.top/gtibnqpikl.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtrusptokx.html

[R28] 浮点运算
来源：http://hz.ydzc1.top/gtjqbesrra.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhongyouzk.top/gtuidfmcmc.html

[R29] 定义函数
来源：http://hz.c1oappe.top/gtdhzimdck.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydjk.org.cn/gtonezytbb.html

[R30] 函数返回状态码
来源：http://hz.ydzc1.top/gtxsawkbrq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuanzhike.top/gtdudwvsik.html

[R31] 局部变量
来源：http://hz.tianlin.xyz/gtxuzuszmd.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gtqajtgfnf.html

[R32] 参数个数校验
来源：http://hz.dashuyun.cn/gtuiyishfw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtnrwfzcjd.html

[R33] 捕获错误并提示行号
来源：http://hz.xinyue.icu/gtluhxeqzj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.svipenyu.cn/gtousyzhbb.html

[R34] 退出时清理
来源：http://hz.yvedp.cn/gtjfrhsaqs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtiuuierkt.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gtuwiwvrep.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigufen.top/gtbnjrwbyb.html

[R36] 并发执行多个任务
来源：http://hz.hysaishi.cn/gtnayaxfno.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.daxiang520.top/gtktnvqrqc.html

[R37] 把输出赋给变量
来源：http://hz.vqdsnc.cn/gtqnizcwhh.html

files=$(ls -1)
来源：http://hz.tianlin.xyz/gtqfjpafay.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gtigxcblnf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daxiang520.top/gtmcxhasoi.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtfwgdxwxc.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gtmzpwiuxl.html

[R40] 追加写日志
来源：http://hz.316326.xyz/gtsaukrdni.html

echo "log" >> out.log
来源：http://hz.sweek.top/gthsfrvmcr.html

[R41] 丢弃输出
来源：http://hz.shzxlz.cn/gtzvrbilyf.html

cmd >/dev/null 2>&1
来源：http://hz.tian-w.cn/gttdaytulp.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gtaimqidmb.html

wc -l < a.txt
来源：http://hz.yuxming.cn/gtlhjrmttd.html

[R43] 按名字查找文件
来源：http://hz.guowangkeji.top/gtevxjapil.html


<!-- 参考信息 -->