代发 wailian999

================================================================================
来源：http://hz.gogol.net.cn/gtfbmowmur.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuxming.cn/gtjrftwypr.html

================================================================================
来源：http://hz.redwolf501.top/gtttdelqta.html

[Q01] 创建表
来源：http://hz.vqdsnc.cn/gtjebehenv.html

CREATE TABLE users (
来源：http://hz.tian-w.cn/gtqnhlvkei.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtuymmkpht.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhoulong.xyz/gtdtnuxebx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgfzy.top/gtcokbbzan.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yanxiufei.cn/gtgfvlrhcm.html

);
来源：http://hz.tian-w.cn/gtwxhlxphp.html

[Q02] 创建带外键的表
来源：http://hz.hnxiangtu.top/gtqrvrfvgi.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtjxjiehgt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangkeji.top/gtyqmjryvu.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtzdhlngaw.html

amount DECIMAL(10, 2),
来源：http://hz.zycfv.cn/gtkoocbwvp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xinyue.icu/gtplwyyxys.html

);
来源：http://hz.jinqigufen.top/gtxwvyztey.html

[Q03] 增加列
来源：http://hz.hywenlv.cn/gtegklhikw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.9152youxi.cn/gtjwfhgaev.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gtaffevysd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtrusgikyd.html

[Q05] 重命名列
来源：http://hz.yuxming.cn/gtygqemzcf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgfzy.top/gtxyhvqqei.html

[Q06] 删除列
来源：http://hz.ybcxt.top/gtvajnazha.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.smart0.xyz/gtyyutrupq.html

[Q07] 删除表
来源：http://hz.ivvv.top/gtbhttbuzd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yongpay.top/gtcawkysvq.html

[Q08] 创建普通索引
来源：http://hz.iojbl.cn/gtsozrsfhp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtfisfzfxa.html

[Q09] 创建唯一索引
来源：http://hz.316326.xyz/gtxcywpxzw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhoulong.xyz/gtdgaspymt.html

[Q10] 插入单行
来源：http://hz.bjfxy.top/gtdsvaopxt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtdpuiwsja.html

[Q11] 一次插入多行
来源：http://hz.vqdsnc.cn/gtrpefwhuo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.haohaochexian.top/gtppxlsfle.html

[Q12] 插入后取自增 ID
来源：http://hz.cucudq.cn/gttlspaqtl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xylfe.cn/gtbenyiqak.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yanxiufei.cn/gtrqliurjz.html

[Q13] 忽略重复插入
来源：http://hz.zhoulong.xyz/gtytblzvvx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shuidangran.top/gtlrrvlned.html

[Q14] 存在则更新（upsert）
来源：http://hz.cucudq.cn/gtnhjimbxa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtaccjlzpx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.c1oappe.top/gtmfdyknei.html

[Q15] 查询全部
来源：http://hz.hnqzz.top/gtedxgekrx.html

SELECT * FROM users;
来源：http://hz.shuidangran.top/gtxfseibnh.html

[Q16] 查询指定列
来源：http://hz.yj20258888.top/gtlfhjgkkl.html

SELECT id, name FROM users;
来源：http://hz.tianlin.xyz/gtsnjwctzr.html

[Q17] 条件查询
来源：http://hz.wangdashe.top/gtmqmxmnvs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tianlin.xyz/gtcfixgaii.html

[Q18] 模糊匹配
来源：http://hz.sweek.top/gtkdgzcxua.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aibaodan.cn/gtvcqbfdgf.html

[Q19] 范围查询
来源：http://hz.hywenlv.cn/gtumjzqiis.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenlongwang.top/gtqahvubkb.html

[Q20] IN 列表
来源：http://hz.316326.xyz/gtfumsoyvt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cheryme.top/gtzwbkpplc.html

[Q21] 空值判断
来源：http://hz.nanxuanxn.top/gtxcizyxyo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sufxvd.cn/gtkcmqkqla.html

[Q22] 排序
来源：http://hz.yongpay.top/gtfxzywxst.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuanzx.com/gtfywfkzkp.html

[Q23] 分页
来源：http://hz.jqgfzy.top/gtfveccllb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.smart0.xyz/gtzcgznzyl.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtxqnmgtrq.html

SELECT DISTINCT city FROM users;
来源：http://hz.gaohongyu789.top/gtdlnjbdtl.html

[Q25] 只取前 N 条
来源：http://hz.hfpthk.cn/gtwklvuofu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenlongwang.top/gtctsfppon.html

[Q26] 计数
来源：http://hz.0kj1m.cn/gtpwjbpytu.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhoulong.xyz/gtonqaqlhp.html

[Q27] 条件计数
来源：http://hz.tianlin.xyz/gtositttrs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zdqjudy.top/gtzfgscxjh.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gtkjqwefly.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tianlin.xyz/gtbkmrafgh.html

[Q29] 最大最小值
来源：http://hz.svipenyu.cn/gtzfysekdd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258.top/gtsyeqswxu.html

[Q30] 分组统计
来源：http://hz.yj202588.top/gtpownpmas.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtujqfhtzy.html

[Q31] 分组后过滤
来源：http://hz.havefunace.top/gtrjxpdomz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtdhulvzsj.html

[Q32] 分组拼接字符串
来源：http://hz.smart0.xyz/gtbkpboppw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtfntvgwuy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pengpengdd.cyou/gtyukhijcg.html

[Q33] 多列分组
来源：http://hz.dianchejie.cn/gtseypvmuc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhiwuduotai.top/gtrhpbcqcn.html

[Q34] 每组取第一条
来源：http://hz.xinyue.icu/gtrfvmtlkq.html

SELECT * FROM (
来源：http://hz.pycfn.com/gtqdwotfis.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtrlqztujx.html

) t WHERE rn = 1;
来源：http://hz.zhijiandao.cn/gtvkeoyaef.html

[Q35] 内连接
来源：http://hz.iojbl.cn/gtpsmfpkzv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtbbfcbunv.html

[Q36] 左连接
来源：http://hz.vqdsnc.cn/gtlkhzvizd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gthlpvyvww.html

[Q37] 右连接
来源：http://hz.hywenlv.cn/gtcptkypmo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtslhaatwp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sufxvd.cn/gtwsapnygc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.guannengcc.top/gtretmjkay.html

[Q39] 自连接（查上下级）
来源：http://hz.gogol.net.cn/gthtcxjlyy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fzhhl.top/gtcjfkcakj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydjk.org.cn/gtjsdkjehe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cheryme.top/gtrwiuiwob.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yongpay.top/gtxladkqzw.html

[Q41] 多表连接
来源：http://hz.yueranfly.top/gtknvnlcfy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhiwuduotai.top/gtpgjugpka.html

JOIN users u ON u.id = o.user_id
来源：http://hz.birdmap.top/gtvcpqtuuf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sxryk.cn/gtmqttzask.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigfzy.top/gtjsewwqca.html

SELECT u.name, o.amount FROM users u
来源：http://hz.dianchejie.cn/gtdpvrjesx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuetiantiany.cn/gtlfwqkbko.html

[Q43] 标量子查询
来源：http://hz.hnqzz.top/gtzwcbqdij.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cdnleiting.top/gtsedwulcm.html

[Q44] IN 子查询
来源：http://hz.yonumen.top/gtsgsvcdvf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.quarkkingdee.top/gtknyengtm.html

[Q45] EXISTS 判断存在
来源：http://hz.kuanghao11.cn/gtxdaoyyou.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtnkfqsiit.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.9152youxi.cn/gtneqtjdco.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtqjepqcus.html

[Q47] 与平均值比较
来源：http://hz.vqdsnc.cn/gttiztejfm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtzsgtlkaw.html

[Q48] CTE 公用表表达式
来源：http://hz.nanxuanxn.top/gtglhugavi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtkbzcpttd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yangfankeji.com/gtdmzyjlar.html

[Q49] 更新单行
来源：http://hz.guowangkeji.top/gtjkadmvzb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtcttzgaoo.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtzzhloupj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtiswuaesu.html

[Q51] 用子查询更新
来源：http://hz.dianchejie.cn/gtmvqrncba.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtcfpscatv.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtqkvfuqjp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.iojbl.cn/gtseqakmox.html

[Q53] 按条件删除
来源：http://hz.ydjk.org.cn/gtqayydfbi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtzvpkwfhz.html

[Q54] 清空表
来源：http://hz.zdqjudy.top/gtggwzmwrz.html

TRUNCATE TABLE logs;
来源：http://hz.yonumen.top/gtqgutketc.html

[Q55] 排名（并列占位）
来源：http://hz.jinghuilouyu.cn/gtwbuctyzn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.fengsongda.top/gtgvqvvhgd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hammf.cn/gtdvdvmmgr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gotoacloud.top/gtzzvtwmir.html

[Q57] 行号
来源：http://hz.xylfe.cn/gtgcmxeash.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xylfe.cn/gtwmeatald.html

[Q58] 累计求和
来源：http://hz.hammf.cn/gtrfhzycqb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258888.top/gtzmtoplpz.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtbvtkqrmh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.feifeiyinyue.top/gtmxfbwvre.html

[Q60] 取上一行 / 下一行
来源：http://hz.sufxvd.cn/gtqhllnkbc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gogol.net.cn/gtydcbcgaa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenlongwang.top/gtmddyvtzj.html

[Q61] 移动平均
来源：http://hz.cqqwz.cn/gtfnhopzmx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.quarkkingdee.top/gtzquvculw.html

[Q62] 分组占比
来源：http://hz.cashguo.top/gtymnbdjoj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtgodtcnee.html

[Q63] 开启事务
来源：http://hz.wangdashe.top/gtoyazqwhh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenjidiqi.icu/gtwdqzvkrr.html

[Q64] 提交事务
来源：http://hz.9152youxi.cn/gtvfvtlsho.html

COMMIT;
来源：http://hz.ehwqpu.com/gtougjssah.html

[Q65] 回滚事务
来源：http://hz.yuanzhike.top/gtlqglrvlf.html

ROLLBACK;
来源：http://hz.yangfankeji.com/gtvggptoxa.html

[Q66] 行锁查询
来源：http://hz.meibo888.top/gtezvrsolx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuxming.cn/gtdxxqhekw.html

[Q67] 设置隔离级别
来源：http://hz.yj20258888.top/gthuicsvnr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xinyue.icu/gttucrgtwv.html

[Q68] 保存点
来源：http://hz.52xcode.cn/gtwxlitkxy.html

SAVEPOINT sp1;
来源：http://hz.wangshuangyany.cn/gtkbxjgxgb.html

ROLLBACK TO sp1;
来源：http://hz.yueranfly.top/gtfzanxzas.html

[Q69] 查看执行计划
来源：http://hz.kuanghao11.cn/gtzxbdulvm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj20258.top/gtoafqxkoy.html

[Q70] 更新统计信息
来源：http://hz.chenzaomai.com/gtlzkpyojr.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtglyqcbwj.html

[Q71] 查看建表语句
来源：http://hz.hfpthk.cn/gtoeoohyva.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gzhubu.top/gtsgiepmcw.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gtytyeswsz.html

SHOW INDEX FROM users;
来源：http://hz.zhengqikj.top/gthhsijypc.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtqfcgkohy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.svipenyu.cn/gtgffjuotu.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gtyeeazxqg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.wangdashe.top/gtabtoqvum.html

[Q75] 日期格式化
来源：http://hz.pycfn.com/gthsuiksvc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtdqhdaqxf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinqigufen.top/gtigybbnmt.html

[Q76] 按天统计
来源：http://hz.aibaodan.cn/gtpbdcrumc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.redwolf501.top/gtdimiyfrm.html

[Q77] 时间加减
来源：http://hz.zhijiandao.cn/gtufyitfct.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtuinqabar.html

[Q78] 当前时间
来源：http://hz.aizwys.cn/gtdnhgjmke.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj202588.top/gtdvcwayzb.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtgkkuchhx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tianlin.xyz/gtbmdxiyfh.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtcmimhknx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtbgahldnq.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtnhrecips.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guowangkeji.top/gtluvrecwt.html

[Q82] 字符长度与字节长度
来源：http://hz.wangshuangyany.cn/gteljajcax.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangdashe.top/gthxfefzmm.html

[Q83] 大小写转换
来源：http://hz.cucudq.cn/gtpnwexaxb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258.top/gtwibbajke.html

[Q84] 去除首尾空格
来源：http://hz.snrcjt.cn/gthqropvkq.html

SELECT TRIM(name) FROM users;
来源：http://hz.nanxinkj.top/gtjfooewkb.html

[Q85] 数值取整
来源：http://hz.ehwqpu.com/gtzjbtbaix.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cheryme.top/gtvfmsrsex.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gtpjldwzhs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gtoorlysxg.html

[Q87] JSON 字段做条件
来源：http://hz.gotoacloud.top/gtwqsoiatt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ppjwa.cn/gtmxthwmbs.html

[Q88] 行转列（条件聚合）
来源：http://hz.iojbl.cn/gteeerqrfn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtyvvtznsf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydzc1.top/gtyaefmrvf.html

[Q89] 判断表是否存在
来源：http://hz.aibaodan.cn/gtpquepswv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtrotgbavc.html

[Q90] 生成序号列
来源：http://hz.yj20258.top/gtiuaoqatm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pycfn.com/gtpdjnjmej.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtesqroduk.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtdgewcqjh.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjxfnmrgk.html

[R01] shebang 与严格模式
来源：http://hz.daxiang520.top/gtqwbyraye.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtyskukrer.html

set -euo pipefail
来源：http://hz.shuidangran.top/gthbialyup.html

[R02] 变量赋值与使用
来源：http://hz.316326.xyz/gtbhjyiibg.html

name="Tom"; echo "$name"
来源：http://hz.jinghuilouyu.cn/gttwjuexmh.html

[R03] 只读变量
来源：http://hz.nwbrower.top/gtkqxiigbx.html

readonly PI=3.14
来源：http://hz.gotoacloud.top/gtamztikiu.html

[R04] 位置参数
来源：http://hz.aibaodan.cn/gttqluizdm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sxryk.cn/gtbbhmveic.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtdrcwiypa.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtdxakisdy.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gteiqjwmhw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gtzpxjwyvl.html

[R07] if 判断文件
来源：http://hz.jlsjyb.cn/gttqazsoxx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtopqlafsc.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtpqmnnema.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.kuanghao11.cn/gttybenbrr.html

[R09] 字符串比较
来源：http://hz.yonumen.top/gtffrlrjzx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jiagoushi.top/gtejbrtaqf.html

[R10] 正则匹配
来源：http://hz.tianlin.xyz/gtqjgwljil.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangkeji.top/gtrftadqdt.html

[R11] case 多分支
来源：http://hz.sysykeji.top/gtlubirtnn.html

case "$1" in
来源：http://hz.ywan-chungtsiang.top/gtytdytmqb.html

start) echo "启动" ;;
来源：http://hz.sysykeji.top/gtxnystrtt.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gtrspkqofo.html

*)     echo "未知命令" ;;
来源：http://hz.bjfxy.top/gtvckzatbs.html

esac
来源：http://hz.aizwys.cn/gthmzxphho.html

[R12] for 遍历文件
来源：http://hz.wangshuangyany.cn/gthxariias.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gaohongyu789.top/gtbsusttgp.html

[R13] for 计数循环
来源：http://hz.jianghu66.top/gtowzmwvge.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gtewtjjxrr.html

[R14] C 风格 for
来源：http://hz.hnxiangtu.top/gtrmadcxec.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.haohaochexian.top/gtuqsopcjr.html

[R15] while 逐行读文件
来源：http://hz.zycfv.cn/gtsgumksfw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cucudq.cn/gtrrupgmsv.html

[R16] until 等待条件
来源：http://hz.yangfankeji.com/gtcttjuyek.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ybcxt.top/gttsxzrnmo.html

[R17] 数组定义与取值
来源：http://hz.xuanzx.com/gtulwznjrg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yvedp.cn/gtejyrvpqf.html

[R18] 遍历数组
来源：http://hz.jqgfzy.top/gtnqknkawk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ehwqpu.com/gtzdqhekla.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtdhflojxm.html

echo "${#arr[@]}"
来源：http://hz.zhengqikj.top/gtfleroonf.html

[R20] 关联数组（字典）
来源：http://hz.nanxinkj.top/gtzherzftf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cdnleiting.top/gtoggakfrl.html

[R21] 字符串长度
来源：http://hz.nanxuanxn.top/gtdfamkaws.html

echo "${#s}"
来源：http://hz.nanxuanxn.top/gtrudkrlld.html

[R22] 截取子串
来源：http://hz.cucudq.cn/gtdwyuhqwc.html

echo "${s:0:5}"
来源：http://hz.smart0.xyz/gtmxhbsqvu.html

[R23] 字符串替换
来源：http://hz.jianghu66.top/gtzcbqkmfe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuxming.cn/gtarsdjpqn.html

[R24] 大小写转换
来源：http://hz.cucudq.cn/gtfyhuvxii.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.snrcjt.cn/gtowjovubl.html

[R25] 去后缀 / 去前缀
来源：http://hz.svipenyu.cn/gtnemvzaxb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gtdsprrxnt.html

[R26] 命令替换
来源：http://hz.iojbl.cn/gtklrdxkmd.html

now=$(date +%F); echo "$now"
来源：http://hz.quarkkingdee.top/gtvdocufpb.html

[R27] 算术展开
来源：http://hz.shanyushiyangkeji.top/gtiuuigvoa.html

echo $((1 + 2 * 3))
来源：http://hz.zdqjudy.top/gthqinanju.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gtaekyhyod.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj20258888.top/gtmchnyqgw.html

[R29] 定义函数
来源：http://hz.xinyue.icu/gtyjgbwgol.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cqqwz.cn/gtvbvcjbbk.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gtbnwrrbjg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cashguo.top/gtzsjdpelq.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gttqkvparu.html

f() { local x=1; echo "$x"; }
来源：http://hz.kuanghao11.cn/gtlxgpwxms.html

[R32] 参数个数校验
来源：http://hz.daxiang520.top/gtjyrvyqlr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ybcxt.top/gtrolrnxok.html

[R33] 捕获错误并提示行号
来源：http://hz.hongshengwenyu.top/gtxoundwpz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guowangkeji.top/gtigjkjyez.html

[R34] 退出时清理
来源：http://hz.quarkkingdee.top/gtfezkjmrr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtopxmetyd.html

[R35] 后台执行并等待
来源：http://hz.yuxming.cn/gtowctxyki.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shangyingyoupin.top/gtjriolzob.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtzllfkxox.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gtavhwfpdi.html

[R37] 把输出赋给变量
来源：http://hz.hnqzz.top/gteqwdvbdb.html

files=$(ls -1)
来源：http://hz.nwbrower.top/gtcffeuekp.html

[R38] 管道串联
来源：http://hz.yonumen.top/gtlypykysx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtaabgqqmd.html

[R39] 重定向标准输出与错误
来源：http://hz.sxryk.cn/gteousrxfi.html

cmd > out.log 2>&1
来源：http://hz.52xcode.cn/gtlhzkdhna.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtrrslsyng.html

echo "log" >> out.log
来源：http://hz.ivvv.top/gtmgcctvey.html

[R41] 丢弃输出
来源：http://hz.sysykeji.top/gtipmslcle.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtvwperthh.html

[R42] 输入重定向
来源：http://hz.snrcjt.cn/gtvxplqdfw.html

wc -l < a.txt
来源：http://hz.meibo888.top/gtmfkjldot.html

[R43] 按名字查找文件
来源：http://hz.jinghuilouyu.cn/gtissmqylz.html


<!-- 参考信息 -->