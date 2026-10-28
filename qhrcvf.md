代发 wailian999

================================================================================
来源：http://hz.fzhhl.top/gtivswwubd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yvedp.cn/gttnumuueq.html

================================================================================
来源：http://hz.hysaishi.cn/gtljcyxlbr.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtrbdfzofe.html

CREATE TABLE users (
来源：http://hz.daxiang520.top/gttmgnupqq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtkdvtsaqm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yanxiufei.cn/gtjigugpvr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.smart0.xyz/gtctueswks.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuanzhike.top/gtabtvmryf.html

);
来源：http://hz.c1oappe.top/gtohhddlgr.html

[Q02] 创建带外键的表
来源：http://hz.zhixingplan.top/gtlzljxukt.html

CREATE TABLE orders (
来源：http://hz.nwbrower.top/gtmrkjengi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhengqikj.top/gtqxpxbkzg.html

user_id INT NOT NULL,
来源：http://hz.cdnleiting.top/gtqmbpbbxh.html

amount DECIMAL(10, 2),
来源：http://hz.xuanzx.com/gtldcmnuxy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangdashe.top/gtgypbnnpm.html

);
来源：http://hz.chenlongwang.top/gtzgsgtjns.html

[Q03] 增加列
来源：http://hz.ivvv.top/gtoarqnfmz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gaohongyu789.top/gtdpcfznzd.html

[Q04] 修改列类型
来源：http://hz.guowangkeji.top/gtnpattfor.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtmphojsff.html

[Q05] 重命名列
来源：http://hz.havefunace.top/gtqbcyxkrx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daria6918.cn/gttthdvmht.html

[Q06] 删除列
来源：http://hz.gaohongyu789.top/gtwklpekse.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gtdpacckos.html

[Q07] 删除表
来源：http://hz.fengsongda.top/gtrmfctesk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gogol.net.cn/gtsvogwazv.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gthqgxkper.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuanzx.com/gttixwtsvt.html

[Q09] 创建唯一索引
来源：http://hz.jyoumei.cn/gtevyfrdoo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtvxeoaynj.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gtoirzoybg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yueranfly.top/gtoeibekuu.html

[Q11] 一次插入多行
来源：http://hz.hywenlv.cn/gtujpkkucf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hongshengwenyu.top/gtdvrdssvo.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtdqnxuvau.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangtech.top/gtnpmakgom.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydzc1.top/gtozeuleti.html

[Q13] 忽略重复插入
来源：http://hz.yj20258.top/gtfsqyzgex.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cashguo.top/gtqyhiglvw.html

[Q14] 存在则更新（upsert）
来源：http://hz.xingfuxueyuan.xyz/gtgcqlyuwr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gotoacloud.top/gtbdnapwtt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hfpthk.cn/gtfljnqshm.html

[Q15] 查询全部
来源：http://hz.smart0.xyz/gtvhfuhlwd.html

SELECT * FROM users;
来源：http://hz.andypj.xyz/gtuqpraecg.html

[Q16] 查询指定列
来源：http://hz.ywan-chungtsiang.top/gtikzcvceu.html

SELECT id, name FROM users;
来源：http://hz.sweek.top/gtrkubnhqy.html

[Q17] 条件查询
来源：http://hz.birdmap.top/gtyshbzoes.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xuanzx.com/gtunjkmffw.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gtdhbygaas.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nwbrower.top/gtyshgrrhf.html

[Q19] 范围查询
来源：http://hz.hongshengwenyu.top/gtrhhcbomp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj202588.top/gtbzpchbzg.html

[Q20] IN 列表
来源：http://hz.jinyuanbaomall.cn/gtinkezehq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jqgufenzy.top/gtomtifvbj.html

[Q21] 空值判断
来源：http://hz.ivvv.top/gtwviueiwq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtjsumcoog.html

[Q22] 排序
来源：http://hz.cucudq.cn/gtzpoihhtb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gogol.net.cn/gtaoyulvxc.html

[Q23] 分页
来源：http://hz.zhongyouzk.top/gtlmwmlazj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.svipenyu.cn/gtiwxdxouk.html

[Q24] 去重
来源：http://hz.jianghu66.top/gtdbabhoyh.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinyuanbaomall.cn/gtytvfucjn.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtunkmqlim.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.iojbl.cn/gtbmbklphi.html

[Q26] 计数
来源：http://hz.sweek.top/gtiyrvkfni.html

SELECT COUNT(*) FROM users;
来源：http://hz.fengsongda.top/gtgyltqkdw.html

[Q27] 条件计数
来源：http://hz.yongpay.top/gtfsgnzimx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gtrqduknpz.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gteizrqfrv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fzhhl.top/gtbsxgtgye.html

[Q29] 最大最小值
来源：http://hz.pengpengdd.cyou/gtwmulweoa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dashuyun.cn/gtpopsnvxo.html

[Q30] 分组统计
来源：http://hz.ywan-chungtsiang.top/gtymgmsrjz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtvlkphqib.html

[Q31] 分组后过滤
来源：http://hz.ydjk.org.cn/gtmhpucwux.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yueranfly.top/gtseyisbos.html

[Q32] 分组拼接字符串
来源：http://hz.zhongyouzk.top/gtejstokyt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtqdtknuoj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.feifeiyinyue.top/gterkhuesu.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtnuedzpwt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.iojbl.cn/gtgdsvivbd.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtmtosduen.html

SELECT * FROM (
来源：http://hz.shzxlz.cn/gtgcsmrawn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ehwqpu.com/gtaripyaae.html

) t WHERE rn = 1;
来源：http://hz.9152youxi.cn/gtuabhnpxc.html

[Q35] 内连接
来源：http://hz.ybcxt.top/gtyyoujavg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtdlwmcaks.html

[Q36] 左连接
来源：http://hz.9152youxi.cn/gtpdtdgauk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtibccfjgh.html

[Q37] 右连接
来源：http://hz.iojbl.cn/gtsfgioucs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shuidangran.top/gtvecxmfwh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xingfuxueyuan.xyz/gttapzvpbg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnxiangtu.top/gtpmhnuojd.html

[Q39] 自连接（查上下级）
来源：http://hz.smart0.xyz/gtmavadcft.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gtievxtrrs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.andypj.xyz/gtyywkxdjp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtaqgwzhmv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenzaomai.com/gtzeomcusz.html

[Q41] 多表连接
来源：http://hz.jyoumei.cn/gtadpaivuk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtcfyhbmmi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gticukyutf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenlongwang.top/gtmditpcbb.html

[Q42] 连接条件附加过滤
来源：http://hz.zycfv.cn/gtyuaskcya.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jianghu66.top/gtptuvpxzr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yvedp.cn/gtkfbtnqir.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtgklmotlh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtgnafnand.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtxrogwwiv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.haohaochexian.top/gtzmsnnquo.html

[Q45] EXISTS 判断存在
来源：http://hz.shuidangran.top/gtcbpsizvl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtputkegbv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pycfn.com/gtjvotrvae.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtuanmazav.html

[Q47] 与平均值比较
来源：http://hz.svipenyu.cn/gtordtrcob.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinyuanbaomall.cn/gtxbhpzaid.html

[Q48] CTE 公用表表达式
来源：http://hz.c1oappe.top/gtztsyperc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuxming.cn/gtysfpfxaa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pycfn.com/gtozqdjnwb.html

[Q49] 更新单行
来源：http://hz.ydjk.org.cn/gtqvmekzqw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtphxdmbzm.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtjwbfxytu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yvedp.cn/gtxqqfungu.html

[Q51] 用子查询更新
来源：http://hz.gzhubu.top/gtlxdvapir.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xziqi.cn/gtsgwdbwel.html

[Q52] 删除指定行
来源：http://hz.ywan-chungtsiang.top/gtyuwccegv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aizwys.cn/gtzjsfziez.html

[Q53] 按条件删除
来源：http://hz.hywenlv.cn/gtwjittinb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yonumen.top/gtevzoicwn.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtybfunimv.html

TRUNCATE TABLE logs;
来源：http://hz.kuanghao11.cn/gtlkfhhsih.html

[Q55] 排名（并列占位）
来源：http://hz.haohaochexian.top/gtpyiijbxm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gtalvuytie.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtwklujsue.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xziqi.cn/gtjrrebobu.html

[Q57] 行号
来源：http://hz.hammf.cn/gtjadsfene.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.mhx1999.top/gthbdxowoe.html

[Q58] 累计求和
来源：http://hz.yuxming.cn/gtzklptyyu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxuanxn.top/gtdpgjlkyf.html

[Q59] 分组内累计
来源：http://hz.chenlongwang.top/gtfijisijr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuanzx.com/gtkwptbpnj.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gtsopzldfk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.kuanghao11.cn/gtffnicsaq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtszluftqz.html

[Q61] 移动平均
来源：http://hz.shanyushiyangkeji.top/gtlwglepab.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fzhhl.top/gtczcvypbr.html

[Q62] 分组占比
来源：http://hz.gotoacloud.top/gthwehtuda.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tanke756.top/gthlxmxcdt.html

[Q63] 开启事务
来源：http://hz.xylfe.cn/gtjbsvdrks.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hongshengwenyu.top/gtoiffuvin.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gtktbachou.html

COMMIT;
来源：http://hz.daria6918.cn/gtwxbgebbx.html

[Q65] 回滚事务
来源：http://hz.quarkkingdee.top/gtahgyddzr.html

ROLLBACK;
来源：http://hz.zhiwuduotai.top/gtzsylkriz.html

[Q66] 行锁查询
来源：http://hz.pengpengdd.cyou/gtqbozgryp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gaohongyu789.top/gtqjrezkjk.html

[Q67] 设置隔离级别
来源：http://hz.zycfv.cn/gtzpdjkfcl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenjidiqi.icu/gtttacrlsh.html

[Q68] 保存点
来源：http://hz.xingfuxueyuan.xyz/gtzpyergrk.html

SAVEPOINT sp1;
来源：http://hz.xingfuxueyuan.xyz/gtulmtcogp.html

ROLLBACK TO sp1;
来源：http://hz.pengpengdd.cyou/gtjuztvckz.html

[Q69] 查看执行计划
来源：http://hz.ydjk.org.cn/gtincvgfnr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yangfankeji.com/gtxxupaevh.html

[Q70] 更新统计信息
来源：http://hz.yanxiufei.cn/gtlxvwrulc.html

ANALYZE TABLE users;
来源：http://hz.gogol.net.cn/gttcvyszkp.html

[Q71] 查看建表语句
来源：http://hz.jyoumei.cn/gttxxxfwjl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tianlin.xyz/gtidgmivnu.html

[Q72] 查看索引
来源：http://hz.wangdashe.top/gtocajitvj.html

SHOW INDEX FROM users;
来源：http://hz.0kj1m.cn/gtqsgzhzzs.html

[Q73] 查看表状态
来源：http://hz.tianlin.xyz/gtyexhqwqu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258888.top/gtnmxfznsb.html

[Q74] 强制使用索引
来源：http://hz.yuanzhike.top/gtjsxjkjau.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuxming.cn/gtrvprbwjm.html

[Q75] 日期格式化
来源：http://hz.xuetiantiany.cn/gtdbflnkrg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.c1oappe.top/gtjzjgmelf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtjjkiumxq.html

[Q76] 按天统计
来源：http://hz.fzhhl.top/gttczwhhxs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tianlin.xyz/gterxuhwvi.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtmlwnbvph.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.redwolf501.top/gtfbcfyxjx.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gtstdnofwo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.52xcode.cn/gtoiilmgjg.html

[Q79] 字符串拼接
来源：http://hz.yj20258.top/gtqrqemtpd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigfzy.top/gtmlwmxjhk.html

[Q80] 字符串截取
来源：http://hz.sxryk.cn/gtyrljfntx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.andypj.xyz/gtgdluiioj.html

[Q81] 字符串替换
来源：http://hz.yangfankeji.com/gtsbamhlip.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangkeji.top/gtwipgtrgy.html

[Q82] 字符长度与字节长度
来源：http://hz.dianchejie.cn/gtqsyefyuf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cdnleiting.top/gtkdtcoham.html

[Q83] 大小写转换
来源：http://hz.tianlin.xyz/gtyhhoemvv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj202588.top/gtjerxerwg.html

[Q84] 去除首尾空格
来源：http://hz.xziqi.cn/gttqginspl.html

SELECT TRIM(name) FROM users;
来源：http://hz.jlsjyb.cn/gtdhluhfxk.html

[Q85] 数值取整
来源：http://hz.kuanghao11.cn/gtvmyqqnjn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ywan-chungtsiang.top/gtclsdxjto.html

[Q86] 读取 JSON 字段
来源：http://hz.cucudq.cn/gtrhypydwq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.vqdsnc.cn/gtlbnjzfvm.html

[Q87] JSON 字段做条件
来源：http://hz.meibo888.top/gtxdbslcvh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dianchejie.cn/gtwaoqajxg.html

[Q88] 行转列（条件聚合）
来源：http://hz.fzhhl.top/gtpusaulms.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.birdmap.top/gtixkniacf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj20258888.top/gthrenuzxc.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtschllfar.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.meibo888.top/gtxuwnusvn.html

[Q90] 生成序号列
来源：http://hz.yueranfly.top/gtnfyjdlwc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.9152youxi.cn/gtipdqiiwh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtblwfkcci.html

R. Bash 专题
来源：http://hz.jqgfzy.top/gthkspwcmg.html

================================================================================
来源：http://hz.redwolf501.top/gtfrwvzxky.html

[R01] shebang 与严格模式
来源：http://hz.zhongyouzk.top/gtvqlighgt.html

#!/usr/bin/env bash
来源：http://hz.tianlin.xyz/gtndsswoqx.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtxowvgsiy.html

[R02] 变量赋值与使用
来源：http://hz.fengsongda.top/gtyqbxoirv.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtqwxeuprr.html

[R03] 只读变量
来源：http://hz.ydjk.org.cn/gtpkkpliac.html

readonly PI=3.14
来源：http://hz.hnxiangtu.top/gthbwklrqw.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gtyhxjkbrl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnqzz.top/gtddzfxlyk.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtmyvaccgh.html

name="${1:-default}"
来源：http://hz.ivvv.top/gttsltscmj.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtuqylejug.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hysaishi.cn/gtkzcrlrav.html

[R07] if 判断文件
来源：http://hz.birdmap.top/gtgqlgzemb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.smart0.xyz/gtxuzvcyjg.html

[R08] 数值比较
来源：http://hz.mhx1999.top/gtriibimxn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtaswehhib.html

[R09] 字符串比较
来源：http://hz.haohaochexian.top/gtwjrnpefw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhijiandao.cn/gtwjyduoek.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtmewgpkwg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.c1oappe.top/gtdtdjnqdz.html

[R11] case 多分支
来源：http://hz.iojbl.cn/gtddmcaher.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gtggelfoxz.html

start) echo "启动" ;;
来源：http://hz.chenlongwang.top/gtsyryuquf.html

stop)  echo "停止" ;;
来源：http://hz.gogol.net.cn/gtdjlyahmq.html

*)     echo "未知命令" ;;
来源：http://hz.yuanzhike.top/gtgewsdzli.html

esac
来源：http://hz.shangyingyoupin.top/gtyvpwevab.html

[R12] for 遍历文件
来源：http://hz.nanxuanxn.top/gtsdkdmkcd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xuetiantiany.cn/gtwwhnsxyp.html

[R13] for 计数循环
来源：http://hz.yvedp.cn/gttogwipei.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtamqyckdl.html

[R14] C 风格 for
来源：http://hz.zhoulong.xyz/gtpqkjtvtb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cqqwz.cn/gtmhxrllqr.html

[R15] while 逐行读文件
来源：http://hz.chenjidiqi.icu/gtezkucyzv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guannengcc.top/gtgbwvgpqq.html

[R16] until 等待条件
来源：http://hz.zhiwuduotai.top/gtujzgzsrp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtvtzdjkrn.html

[R17] 数组定义与取值
来源：http://hz.zhaomingkeji.xyz/gtgtikhhpl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.bjfxy.top/gtsnijmwxr.html

[R18] 遍历数组
来源：http://hz.jinghuilouyu.cn/gtjlfrwszz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tanke756.top/gtlxbqljif.html

[R19] 数组长度
来源：http://hz.yj20258.top/gtieuitbre.html

echo "${#arr[@]}"
来源：http://hz.52xcode.cn/gtbakwvfph.html

[R20] 关联数组（字典）
来源：http://hz.cqqwz.cn/gtoexxofoa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtyeouqtez.html

[R21] 字符串长度
来源：http://hz.zhoulong.xyz/gtkppotdnn.html

echo "${#s}"
来源：http://hz.jyoumei.cn/gtqbzasxpt.html

[R22] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtslrmyyjn.html

echo "${s:0:5}"
来源：http://hz.ywan-chungtsiang.top/gthkeyecyl.html

[R23] 字符串替换
来源：http://hz.zdqjudy.top/gtdnlrftaj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigfzy.top/gtnlzsfbbn.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gtevlzcgwt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxuanxn.top/gtismolkiz.html

[R25] 去后缀 / 去前缀
来源：http://hz.316326.xyz/gtsdzsvyni.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.c1oappe.top/gtnlieiutw.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtfxepxgwj.html

now=$(date +%F); echo "$now"
来源：http://hz.xuanzx.com/gtnzpfewcv.html

[R27] 算术展开
来源：http://hz.pengpengdd.cyou/gtdksqepob.html

echo $((1 + 2 * 3))
来源：http://hz.yanxiufei.cn/gtcwxxvgan.html

[R28] 浮点运算
来源：http://hz.nanxuanxn.top/gtczlayrga.html

echo "scale=2; 10/3" | bc
来源：http://hz.meibo888.top/gtcdpezpnw.html

[R29] 定义函数
来源：http://hz.hnqzz.top/gtwmujfaya.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangshuangyany.cn/gtrlyiilok.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gteutcmoup.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.haohaochexian.top/gtbrzwkrcq.html

[R31] 局部变量
来源：http://hz.quarkkingdee.top/gteppnzsqa.html

f() { local x=1; echo "$x"; }
来源：http://hz.havefunace.top/gtrfsbsofd.html

[R32] 参数个数校验
来源：http://hz.zhengqikj.top/gtioxbsvdr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.aizwys.cn/gtzuvwyxxj.html

[R33] 捕获错误并提示行号
来源：http://hz.cheryme.top/gtegbpadlt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinyuanbaomall.cn/gtywceguxu.html

[R34] 退出时清理
来源：http://hz.andypj.xyz/gtljitjajh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gttqskdegp.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtuzhujhak.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cashguo.top/gtbjjfzgkd.html

[R36] 并发执行多个任务
来源：http://hz.zhixingplan.top/gtepvtcynn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gtogmlalda.html

[R37] 把输出赋给变量
来源：http://hz.zhijiandao.cn/gtxonsjach.html

files=$(ls -1)
来源：http://hz.daxiang520.top/gtoerunxkz.html

[R38] 管道串联
来源：http://hz.shzxlz.cn/gtjttcvwfq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shanyushiyangkeji.top/gtmmzygchh.html

[R39] 重定向标准输出与错误
来源：http://hz.zhijiandao.cn/gttnbjkyoj.html

cmd > out.log 2>&1
来源：http://hz.aibaodan.cn/gtnufwlfyx.html

[R40] 追加写日志
来源：http://hz.zhaomingkeji.xyz/gtwznmnoko.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtvbmcvzgn.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtkpspsfho.html

cmd >/dev/null 2>&1
来源：http://hz.hywenlv.cn/gtvrbewnwm.html

[R42] 输入重定向
来源：http://hz.hnqzz.top/gtwnvjrykg.html

wc -l < a.txt
来源：http://hz.jinyuanbaomall.cn/gtufvjxwpv.html

[R43] 按名字查找文件
来源：http://hz.jinghuilouyu.cn/gtmyqefeur.html


<!-- 参考信息 -->