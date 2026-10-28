代发 wailian999

================================================================================
来源：http://hz.yj202588.top/gthowgctxf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zycfv.cn/gtwohyteic.html

================================================================================
来源：http://hz.daxiang520.top/gtohbrioot.html

[Q01] 创建表
来源：http://hz.iojbl.cn/gtxbkpkocz.html

CREATE TABLE users (
来源：http://hz.jinqigufen.top/gtsqraeyxv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hammf.cn/gtvoktvwjw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258.top/gtjogbahfx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhiwuduotai.top/gtututuyxl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zdqjudy.top/gtnbvglzay.html

);
来源：http://hz.sweek.top/gtztixkfsh.html

[Q02] 创建带外键的表
来源：http://hz.jlsjyb.cn/gtvattkvmo.html

CREATE TABLE orders (
来源：http://hz.gogol.net.cn/gtpkfzetmr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtvxgmcxux.html

user_id INT NOT NULL,
来源：http://hz.xziqi.cn/gtcngrsled.html

amount DECIMAL(10, 2),
来源：http://hz.havefunace.top/gtkbbfzeci.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cqqwz.cn/gtuimutfjc.html

);
来源：http://hz.c1oappe.top/gtydymffwc.html

[Q03] 增加列
来源：http://hz.hammf.cn/gthrlbrhcl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.kuanghao11.cn/gtizkytknp.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtpgybhkvz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.havefunace.top/gtqzpeeqfz.html

[Q05] 重命名列
来源：http://hz.hammf.cn/gtkdvdxulf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jiagoushi.top/gtptedzzwo.html

[Q06] 删除列
来源：http://hz.meibo888.top/gtoufhjnfw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.mhx1999.top/gtlslxygot.html

[Q07] 删除表
来源：http://hz.tian-w.cn/gtpyvwhksz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nanxinkj.top/gtjlolmwgb.html

[Q08] 创建普通索引
来源：http://hz.quarkkingdee.top/gtwhepwvrc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtwgfvlkqo.html

[Q09] 创建唯一索引
来源：http://hz.wangdashe.top/gtkiwkbfjd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtewdgdeho.html

[Q10] 插入单行
来源：http://hz.zhongyouzk.top/gtkahgfsvs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gotoacloud.top/gtwcrpmvex.html

[Q11] 一次插入多行
来源：http://hz.yj202588.top/gtmjbvoxrc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ywan-chungtsiang.top/gthucbsrzh.html

[Q12] 插入后取自增 ID
来源：http://hz.zhijiandao.cn/gttsuelabx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.tanke756.top/gtypathfxp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gtiotvgiqp.html

[Q13] 忽略重复插入
来源：http://hz.chenzaomai.com/gtfgsmhrxx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258.top/gtgxwatjcj.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gtndgtbztj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtvlxydwcq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinyuanbaomall.cn/gtflabagcc.html

[Q15] 查询全部
来源：http://hz.shzxlz.cn/gtnmswtsnn.html

SELECT * FROM users;
来源：http://hz.sxryk.cn/gtxuwonnhw.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gtcwnfcsta.html

SELECT id, name FROM users;
来源：http://hz.yuanzhike.top/gtdhimgidc.html

[Q17] 条件查询
来源：http://hz.52xcode.cn/gttmtpovhw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.c1oappe.top/gtspqhfxcw.html

[Q18] 模糊匹配
来源：http://hz.yuanzhike.top/gtkmefurgk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sweek.top/gtnzxqpkxk.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gtolzfsmnw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.aibaodan.cn/gtmxxanggn.html

[Q20] IN 列表
来源：http://hz.feifeiyinyue.top/gtskfnarmy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ppjwa.cn/gtafpkcgyf.html

[Q21] 空值判断
来源：http://hz.guannengcc.top/gtwmhctsrk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ywan-chungtsiang.top/gttfmaryqm.html

[Q22] 排序
来源：http://hz.chenzaomai.com/gtaxkpmtin.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtfebxibmo.html

[Q23] 分页
来源：http://hz.tianlin.xyz/gtfkgwufuj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.redwolf501.top/gtnhaycsuu.html

[Q24] 去重
来源：http://hz.redwolf501.top/gtimrzepol.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtkbqyqfpd.html

[Q25] 只取前 N 条
来源：http://hz.bjfxy.top/gtuuuwzxmv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.haohaochexian.top/gthjjwyvnw.html

[Q26] 计数
来源：http://hz.gaohongyu789.top/gtqgnmndff.html

SELECT COUNT(*) FROM users;
来源：http://hz.svipenyu.cn/gtghjwckfy.html

[Q27] 条件计数
来源：http://hz.ybcxt.top/gtqbgyjbte.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.feifeiyinyue.top/gtsgfgppfe.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtjielbegq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gtrtdoxynx.html

[Q29] 最大最小值
来源：http://hz.jqgfzy.top/gtjqvturjq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtutgetasd.html

[Q30] 分组统计
来源：http://hz.fzhhl.top/gtldsyisns.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtlggynyfu.html

[Q31] 分组后过滤
来源：http://hz.aizwys.cn/gtlotrecyr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.316326.xyz/gtnkufblkt.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtspvgjraq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtjnwoaezc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jianghu66.top/gtmulrcull.html

[Q33] 多列分组
来源：http://hz.gzhubu.top/gtvfjjasdq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cheryme.top/gtfkjvgivn.html

[Q34] 每组取第一条
来源：http://hz.birdmap.top/gtktwpxryv.html

SELECT * FROM (
来源：http://hz.hongshengwenyu.top/gtdvqwrzpt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yangfankeji.com/gtotvejfbx.html

) t WHERE rn = 1;
来源：http://hz.cdnleiting.top/gttmvqvifi.html

[Q35] 内连接
来源：http://hz.zhixingplan.top/gtzjyyfboo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtpcydnaty.html

[Q36] 左连接
来源：http://hz.quarkkingdee.top/gtpfssyrii.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtrsplnkux.html

[Q37] 右连接
来源：http://hz.jiagoushi.top/gtztxaeekx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtprczqvxz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ybcxt.top/gtbirqqfox.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dashuyun.cn/gtifwlvtph.html

[Q39] 自连接（查上下级）
来源：http://hz.jlsjyb.cn/gtcsvyubxl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.svipenyu.cn/gtzcevsxqi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shangyingyoupin.top/gtzujcbpwa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtbyaqnxky.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jyoumei.cn/gtqytsxzca.html

[Q41] 多表连接
来源：http://hz.hfpthk.cn/gtganuxgtc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.havefunace.top/gtmfipklfq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258888.top/gtqujaqlss.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gaohongyu789.top/gttoagwxuw.html

[Q42] 连接条件附加过滤
来源：http://hz.jianghu66.top/gttujvfznu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nwbrower.top/gtpjqifwmk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yueranfly.top/gtseumgisd.html

[Q43] 标量子查询
来源：http://hz.jinqigfzy.top/gtagzpwfki.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.guannengcc.top/gtxkxkzepe.html

[Q44] IN 子查询
来源：http://hz.tianlin.xyz/gtosrewkae.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxuanxn.top/gtswilvvgt.html

[Q45] EXISTS 判断存在
来源：http://hz.guowangkeji.top/gtnmitawbl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtssxnlwma.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jiagoushi.top/gtrsbbsffn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtpvdjgfww.html

[Q47] 与平均值比较
来源：http://hz.zycfv.cn/gtrmsothap.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxuanxn.top/gtbwcdcmjr.html

[Q48] CTE 公用表表达式
来源：http://hz.chenlongwang.top/gtmnytkrfo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yongpay.top/gtuawahpfr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aizwys.cn/gtdpuktzdq.html

[Q49] 更新单行
来源：http://hz.nwbrower.top/gtywhhxbir.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xziqi.cn/gtjrgkpowd.html

[Q50] 批量更新
来源：http://hz.zhoulong.xyz/gtcmzrfpsl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtcgsekqzz.html

[Q51] 用子查询更新
来源：http://hz.yuanzhike.top/gttwuyzrqi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aizwys.cn/gtbqsshuzo.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtxtgatcza.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtyaylnoso.html

[Q53] 按条件删除
来源：http://hz.0kj1m.cn/gtammuoekw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.andypj.xyz/gtrqmjtqej.html

[Q54] 清空表
来源：http://hz.xingfuxueyuan.xyz/gtuxlywakf.html

TRUNCATE TABLE logs;
来源：http://hz.zhongyouzk.top/gtyshonsvm.html

[Q55] 排名（并列占位）
来源：http://hz.svipenyu.cn/gtwfmqqnqw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tianlin.xyz/gtsppoyvbn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtzmmxbxap.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.guowangkeji.top/gtvkihomlm.html

[Q57] 行号
来源：http://hz.gaohongyu789.top/gtyebkmdhc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtfhveubue.html

[Q58] 累计求和
来源：http://hz.feifeiyinyue.top/gtfakwcfxl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dashuyun.cn/gtdxbvfsvf.html

[Q59] 分组内累计
来源：http://hz.quarkkingdee.top/gtqzgbkxkb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tian-w.cn/gtfjqqcvsh.html

[Q60] 取上一行 / 下一行
来源：http://hz.gzhubu.top/gthkxsjxrf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.smart0.xyz/gtgymanctp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuetiantiany.cn/gtxsugwakb.html

[Q61] 移动平均
来源：http://hz.yj202588.top/gtrmkatenk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj20258888.top/gtjmggsxxg.html

[Q62] 分组占比
来源：http://hz.sxryk.cn/gtkfvbhdlv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuanzhike.top/gtyaaauixd.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtobxflspq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtfdqeoowl.html

[Q64] 提交事务
来源：http://hz.dianchejie.cn/gtgtsustaf.html

COMMIT;
来源：http://hz.ydjk.org.cn/gtbumceara.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gtqbgqyhye.html

ROLLBACK;
来源：http://hz.yuxming.cn/gtprinrkqh.html

[Q66] 行锁查询
来源：http://hz.yueranfly.top/gtxkjbqynl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.smart0.xyz/gtxmsdivgm.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtwbspgpfn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gzhubu.top/gtpyjljgzu.html

[Q68] 保存点
来源：http://hz.jqgfzy.top/gtrdhhvtty.html

SAVEPOINT sp1;
来源：http://hz.sufxvd.cn/gthlzzkuay.html

ROLLBACK TO sp1;
来源：http://hz.xingfuxueyuan.xyz/gtxkdhyvbz.html

[Q69] 查看执行计划
来源：http://hz.svipenyu.cn/gtdcohsgml.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aibaodan.cn/gtourqavcj.html

[Q70] 更新统计信息
来源：http://hz.smart0.xyz/gttpenyunp.html

ANALYZE TABLE users;
来源：http://hz.yueranfly.top/gtwgtdvxik.html

[Q71] 查看建表语句
来源：http://hz.c1oappe.top/gtjsfluvav.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yvedp.cn/gtlpwxayik.html

[Q72] 查看索引
来源：http://hz.ppjwa.cn/gtwxhxwxmr.html

SHOW INDEX FROM users;
来源：http://hz.tanke756.top/gtxqecjvii.html

[Q73] 查看表状态
来源：http://hz.52xcode.cn/gtvmgtoqoz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hywenlv.cn/gtgbdaimvj.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gtrtidygme.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenzaomai.com/gtyofpyqig.html

[Q75] 日期格式化
来源：http://hz.yueranfly.top/gtxjpdekxa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinqigufen.top/gtszzfpxhp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhoulong.xyz/gtvuhqkzae.html

[Q76] 按天统计
来源：http://hz.jqgufenzy.top/gtuorjmyyf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhoulong.xyz/gtplwxnhcf.html

[Q77] 时间加减
来源：http://hz.52xcode.cn/gtndhjjbov.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hammf.cn/gtakebncps.html

[Q78] 当前时间
来源：http://hz.wangshuangyany.cn/gtwythcwgj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zycfv.cn/gtswiocjca.html

[Q79] 字符串拼接
来源：http://hz.52xcode.cn/gtgkermidq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gtxliyaaou.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtwkqhhphc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxinkj.top/gtnjfgbpvz.html

[Q81] 字符串替换
来源：http://hz.jiagoushi.top/gtarwcphqq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtdiujnosx.html

[Q82] 字符长度与字节长度
来源：http://hz.cheryme.top/gtnrminvss.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnxiangtu.top/gtzivrljct.html

[Q83] 大小写转换
来源：http://hz.snrcjt.cn/gtwxersvxm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtpkqppaju.html

[Q84] 去除首尾空格
来源：http://hz.shuidangran.top/gtuzyauzty.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigufen.top/gteokfjaqk.html

[Q85] 数值取整
来源：http://hz.zhaomingkeji.xyz/gtglzmpovv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtomdgvnrx.html

[Q86] 读取 JSON 字段
来源：http://hz.xuetiantiany.cn/gtxsonwaya.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnqzz.top/gtyrcsqjsd.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtmvkykjqf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zdqjudy.top/gttyuapkur.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gthmjofknh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gtvfrbvgyb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cashguo.top/gtorlwozjt.html

[Q89] 判断表是否存在
来源：http://hz.ybcxt.top/gtkyiwclot.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sysykeji.top/gtyxuiioni.html

[Q90] 生成序号列
来源：http://hz.nwbrower.top/gtxejehsnr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhaomingkeji.xyz/gtjazdfmty.html

================================================================================
来源：http://hz.chenzaomai.com/gtiykoufgf.html

R. Bash 专题
来源：http://hz.shzxlz.cn/gtitaloxhl.html

================================================================================
来源：http://hz.0kj1m.cn/gtjvnhhdkp.html

[R01] shebang 与严格模式
来源：http://hz.dianchejie.cn/gtfeghjbkw.html

#!/usr/bin/env bash
来源：http://hz.wangdashe.top/gteegvaopg.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtiyqrhldf.html

[R02] 变量赋值与使用
来源：http://hz.wangdashe.top/gtoomogfws.html

name="Tom"; echo "$name"
来源：http://hz.ybcxt.top/gtstyayopx.html

[R03] 只读变量
来源：http://hz.gaohongyu789.top/gtvvxtrxdn.html

readonly PI=3.14
来源：http://hz.jlsjyb.cn/gtvmkftzgy.html

[R04] 位置参数
来源：http://hz.aibaodan.cn/gtzsfxxuuj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ybcxt.top/gtjrxkphbh.html

[R05] 参数默认值
来源：http://hz.daria6918.cn/gtmegvdtjj.html

name="${1:-default}"
来源：http://hz.hfpthk.cn/gtcygtonir.html

[R06] 判断命令是否存在
来源：http://hz.xuanzx.com/gtrqgxkbfs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tianlin.xyz/gtznindsph.html

[R07] if 判断文件
来源：http://hz.hammf.cn/gthgscvnht.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jqgfzy.top/gtfryxlxre.html

[R08] 数值比较
来源：http://hz.cdnleiting.top/gttqvacalh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gtvqipevze.html

[R09] 字符串比较
来源：http://hz.sweek.top/gtiauuiqfl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shzxlz.cn/gtobctmbsr.html

[R10] 正则匹配
来源：http://hz.zhongyouzk.top/gthzvyornp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangkeji.top/gtzxsusfph.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtzhnyytyk.html

case "$1" in
来源：http://hz.jqgfzy.top/gtqcwcasnt.html

start) echo "启动" ;;
来源：http://hz.cheryme.top/gtbplfhijf.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gtttrofqay.html

*)     echo "未知命令" ;;
来源：http://hz.cdnleiting.top/gttlfarkvn.html

esac
来源：http://hz.cqqwz.cn/gtqvvlixlg.html

[R12] for 遍历文件
来源：http://hz.haohaochexian.top/gtxlpgbivd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258.top/gtrulumtlq.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtnhqtseni.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cqqwz.cn/gtxtugzsad.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtasosxkzd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtrbetizcj.html

[R15] while 逐行读文件
来源：http://hz.jinghuilouyu.cn/gtlwxnjoxv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gtetifppqt.html

[R16] until 等待条件
来源：http://hz.wangshuangyany.cn/gtluziognf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hnxiangtu.top/gteehstiaw.html

[R17] 数组定义与取值
来源：http://hz.sufxvd.cn/gtbjyohqth.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangdashe.top/gttnjlvosw.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtuwyffxru.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydjk.org.cn/gtnpietzhv.html

[R19] 数组长度
来源：http://hz.xylfe.cn/gtqftaaprn.html

echo "${#arr[@]}"
来源：http://hz.mhx1999.top/gtehwnjqsr.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtrljtjugz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tanke756.top/gtjerrgbrd.html

[R21] 字符串长度
来源：http://hz.vqdsnc.cn/gtwycqytvt.html

echo "${#s}"
来源：http://hz.yonumen.top/gtwvsiouig.html

[R22] 截取子串
来源：http://hz.kuanghao11.cn/gtyafiyepv.html

echo "${s:0:5}"
来源：http://hz.quarkkingdee.top/gtdckewtjx.html

[R23] 字符串替换
来源：http://hz.zhiwuduotai.top/gterqtdtpr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gtqqzxkhyg.html

[R24] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtwifcwgap.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenlongwang.top/gtpefqpwva.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gtajrtybwp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zycfv.cn/gtfgaapecb.html

[R26] 命令替换
来源：http://hz.jinghuilouyu.cn/gtulmtshvk.html

now=$(date +%F); echo "$now"
来源：http://hz.zhoulong.xyz/gtomtogiqw.html

[R27] 算术展开
来源：http://hz.0kj1m.cn/gtiooxosyr.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtthqgftko.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtkljklbpa.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gtxmtavmdf.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gtuyevwoxb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.haohaochexian.top/gtntqmqwqp.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gtqcisuxdb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.birdmap.top/gtedypkyvp.html

[R31] 局部变量
来源：http://hz.ppjwa.cn/gtdlehoqya.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gtoyhlphab.html

[R32] 参数个数校验
来源：http://hz.dianchejie.cn/gtnitvqqxk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtfsgafzsk.html

[R33] 捕获错误并提示行号
来源：http://hz.nanxuanxn.top/gtdoxadegc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtglbatkzn.html

[R34] 退出时清理
来源：http://hz.zdqjudy.top/gttywznngz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gtakchnihx.html

[R35] 后台执行并等待
来源：http://hz.gogol.net.cn/gtiiwryqwu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinghuilouyu.cn/gtibrqytgz.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtmfmashub.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dashuyun.cn/gtrkxduckh.html

[R37] 把输出赋给变量
来源：http://hz.tianlin.xyz/gtvyijvsda.html

files=$(ls -1)
来源：http://hz.xuanzx.com/gttjoftljo.html

[R38] 管道串联
来源：http://hz.xingfuxueyuan.xyz/gtxqctjbje.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtxnyeffqd.html

[R39] 重定向标准输出与错误
来源：http://hz.yanxiufei.cn/gtbgieehrv.html

cmd > out.log 2>&1
来源：http://hz.xylfe.cn/gtrgizxhfd.html

[R40] 追加写日志
来源：http://hz.shanyushiyangtech.top/gtkikbkbkl.html

echo "log" >> out.log
来源：http://hz.cqqwz.cn/gtbirzifac.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gtiylhvixk.html

cmd >/dev/null 2>&1
来源：http://hz.tianlin.xyz/gtnuawlvvi.html

[R42] 输入重定向
来源：http://hz.zhijiandao.cn/gtjmlgqkoa.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtvfxauzcv.html

[R43] 按名字查找文件
来源：http://hz.zhoulong.xyz/gthhjuedgv.html


<!-- 参考信息 -->