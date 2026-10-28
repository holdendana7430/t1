代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.smart0.xyz/gtkfnbrnvw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hfpthk.cn/gtcpulkuuq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gogol.net.cn/gtudenzdhp.html

[P08] 处理浮点精度问题
来源：http://hz.tianlin.xyz/gtvahvpenj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cashguo.top/gtmhecbwyj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gaohongyu789.top/gtsqxmauxz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydzc1.top/gteihpvldk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.snrcjt.cn/gtabhkrgwm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.bjfxy.top/gtusvopluw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yanxiufei.cn/gtbiludaco.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgufenzy.top/gtzvxrxioq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.smart0.xyz/gtoolpymwv.html

================================================================================
来源：http://hz.yj202588.top/gteklpdymz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shangyingyoupin.top/gtfomjdadp.html

================================================================================
来源：http://hz.c1oappe.top/gtdhuhmkzi.html

[Q01] 创建表
来源：http://hz.sxryk.cn/gtpwlobzkl.html

CREATE TABLE users (
来源：http://hz.sysykeji.top/gtybnxlenc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gtqpsyudmc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shangyingyoupin.top/gtzyhgdijc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenlongwang.top/gtkzryymnj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuanzx.com/gtcktiaauw.html

);
来源：http://hz.yj20258888.top/gtrnsqszbf.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gtppfsrpvv.html

CREATE TABLE orders (
来源：http://hz.sxryk.cn/gtkizsdvdy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sysykeji.top/gtynckupgv.html

user_id INT NOT NULL,
来源：http://hz.zhixingplan.top/gtlybqfimy.html

amount DECIMAL(10, 2),
来源：http://hz.wangdashe.top/gtorrlrwqf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ehwqpu.com/gtqetjwcqh.html

);
来源：http://hz.zdqjudy.top/gtpvgnldbl.html

[Q03] 增加列
来源：http://hz.xinyue.icu/gtexhqxsqt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.quarkkingdee.top/gtuxkidwal.html

[Q04] 修改列类型
来源：http://hz.jqgfzy.top/gtsqtlbstv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.kuanghao11.cn/gtbcmzyslg.html

[Q05] 重命名列
来源：http://hz.wangshuangyany.cn/gtotrvvnto.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.feifeiyinyue.top/gtfnlygusf.html

[Q06] 删除列
来源：http://hz.yuanzhike.top/gtqvehgiiy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinghuilouyu.cn/gtuotstdtf.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtgvfgklxc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hammf.cn/gtlqkndrvw.html

[Q08] 创建普通索引
来源：http://hz.ehwqpu.com/gtgrwuyvoq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtquqnbwcq.html

[Q09] 创建唯一索引
来源：http://hz.gzhubu.top/gtvdallccd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sweek.top/gtbotdltvg.html

[Q10] 插入单行
来源：http://hz.cheryme.top/gtyvmvhlsr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yonumen.top/gtpbphkuaf.html

[Q11] 一次插入多行
来源：http://hz.xziqi.cn/gtxweigsuj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gtzessfyrx.html

[Q12] 插入后取自增 ID
来源：http://hz.hammf.cn/gtzeanbdsc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pycfn.com/gtmosbruan.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gtgeqnfmul.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gtbnjdhmcx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sweek.top/gteovcllhl.html

[Q14] 存在则更新（upsert）
来源：http://hz.c1oappe.top/gtsjaamxxg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gaohongyu789.top/gtabmemthm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ywan-chungtsiang.top/gtjxddbjhh.html

[Q15] 查询全部
来源：http://hz.tanke756.top/gtfxciminq.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtesrenxpx.html

[Q16] 查询指定列
来源：http://hz.jinyuanbaomall.cn/gtavtrtotw.html

SELECT id, name FROM users;
来源：http://hz.dianchejie.cn/gtxmqsggiz.html

[Q17] 条件查询
来源：http://hz.aizwys.cn/gteiyziznq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hywenlv.cn/gtjhsdawfd.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangtech.top/gtibazilqr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hfpthk.cn/gtzjjhkbzw.html

[Q19] 范围查询
来源：http://hz.feifeiyinyue.top/gtbxgkxcbo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cqqwz.cn/gtruywemqg.html

[Q20] IN 列表
来源：http://hz.shanyushiyangkeji.top/gtxnsgiaiu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tianlin.xyz/gtepgockjt.html

[Q21] 空值判断
来源：http://hz.fzhhl.top/gtuuepnmnz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.daxiang520.top/gtmnhzbojm.html

[Q22] 排序
来源：http://hz.daria6918.cn/gtjzlgfdfl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tianlin.xyz/gtcntecoro.html

[Q23] 分页
来源：http://hz.yanxiufei.cn/gtkiyrsbrb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xziqi.cn/gtjudesotw.html

[Q24] 去重
来源：http://hz.fengsongda.top/gtnzijuscp.html

SELECT DISTINCT city FROM users;
来源：http://hz.c1oappe.top/gtwylgmiuj.html

[Q25] 只取前 N 条
来源：http://hz.yj20258.top/gtuppvkdoc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xinyue.icu/gtpbpacetr.html

[Q26] 计数
来源：http://hz.zhongyouzk.top/gtybdmguqo.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtpxaqbqbq.html

[Q27] 条件计数
来源：http://hz.gogol.net.cn/gtklhwgnex.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.snrcjt.cn/gtmnxxqeyc.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtwugbrrxq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sxryk.cn/gtuxjyuxqq.html

[Q29] 最大最小值
来源：http://hz.mhx1999.top/gtujxvkjlr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sysykeji.top/gtpqevdpbo.html

[Q30] 分组统计
来源：http://hz.chenzaomai.com/gtuapxguor.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtdnndmuib.html

[Q31] 分组后过滤
来源：http://hz.yongpay.top/gtkwptohzy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yanxiufei.cn/gtswjavfre.html

[Q32] 分组拼接字符串
来源：http://hz.smart0.xyz/gtubzttlid.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtsyyucbfl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gotoacloud.top/gtdgwnndxc.html

[Q33] 多列分组
来源：http://hz.jyoumei.cn/gthnhcnxfp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shzxlz.cn/gtaxshgiav.html

[Q34] 每组取第一条
来源：http://hz.yuanzhike.top/gtixbkiayg.html

SELECT * FROM (
来源：http://hz.aibaodan.cn/gtljuxkxhu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gteygsqaxz.html

) t WHERE rn = 1;
来源：http://hz.jinqigfzy.top/gtstueaqgr.html

[Q35] 内连接
来源：http://hz.haohaochexian.top/gthtiwvkup.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtftajcyqk.html

[Q36] 左连接
来源：http://hz.hnxiangtu.top/gtaviufaof.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtsjnlgcba.html

[Q37] 右连接
来源：http://hz.sufxvd.cn/gtnbsjbdur.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zycfv.cn/gteewukpst.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daxiang520.top/gteljquopq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.havefunace.top/gtbgjyadku.html

[Q39] 自连接（查上下级）
来源：http://hz.meibo888.top/gttamzglfy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cdnleiting.top/gtarcxyxiy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtktbkmtzw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guannengcc.top/gtqgebabbp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtuaszhnmo.html

[Q41] 多表连接
来源：http://hz.xziqi.cn/gtswmzfzdt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtklpxgjec.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgfzy.top/gtulihrtch.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydjk.org.cn/gtwfaydyzf.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigufen.top/gtvnvlzuyg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.guannengcc.top/gtwzxbwirc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gtvktfrnzl.html

[Q43] 标量子查询
来源：http://hz.hfpthk.cn/gtftcudbpr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sweek.top/gthdmibikq.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtzbhbkxeh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuanzx.com/gtkowhittl.html

[Q45] EXISTS 判断存在
来源：http://hz.svipenyu.cn/gtoltubghj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtemqokykc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xingfuxueyuan.xyz/gtixforqkq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtxbcfmpez.html

[Q47] 与平均值比较
来源：http://hz.xingfuxueyuan.xyz/gthkcrvnbm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtxpaknvgh.html

[Q48] CTE 公用表表达式
来源：http://hz.smart0.xyz/gtghajlagv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtjnbwiyrb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zycfv.cn/gtionszdcn.html

[Q49] 更新单行
来源：http://hz.fzhhl.top/gtpkfvfkaz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ehwqpu.com/gtczplslqk.html

[Q50] 批量更新
来源：http://hz.52xcode.cn/gtcyrokzyq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinghuilouyu.cn/gtemjsnzpz.html

[Q51] 用子查询更新
来源：http://hz.xziqi.cn/gtwposwhxh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.redwolf501.top/gtzpqhknbv.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gtxjmadufr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.9152youxi.cn/gthfwbvhdb.html

[Q53] 按条件删除
来源：http://hz.hammf.cn/gtbtgfeocl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guowangkeji.top/gtmcazyabo.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtyrarnzxd.html

TRUNCATE TABLE logs;
来源：http://hz.kuanghao11.cn/gtxyvucjpl.html

[Q55] 排名（并列占位）
来源：http://hz.cqqwz.cn/gtoeysxvbw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangshuangyany.cn/gtfptxwnpb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.meibo888.top/gtatvjrxwn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtjpridyic.html

[Q57] 行号
来源：http://hz.316326.xyz/gtxwyqkgmz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.kuanghao11.cn/gtogptijei.html

[Q58] 累计求和
来源：http://hz.xziqi.cn/gtoqvwroxv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnxiangtu.top/gtzrggkbag.html

[Q59] 分组内累计
来源：http://hz.shangyingyoupin.top/gtczmmbymb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.0kj1m.cn/gtfoylhfac.html

[Q60] 取上一行 / 下一行
来源：http://hz.smart0.xyz/gtwewbueka.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenjidiqi.icu/gtdbkexybx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gotoacloud.top/gtwkxnqyms.html

[Q61] 移动平均
来源：http://hz.jlsjyb.cn/gtpfgcnbso.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xziqi.cn/gtldtrwnny.html

[Q62] 分组占比
来源：http://hz.9152youxi.cn/gtkbucpjkq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtnaajnmgo.html

[Q63] 开启事务
来源：http://hz.hysaishi.cn/gtmhzeexel.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gotoacloud.top/gtojauqnqu.html

[Q64] 提交事务
来源：http://hz.xuanzx.com/gtecehbrgz.html

COMMIT;
来源：http://hz.shzxlz.cn/gtihngfwuf.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gtainfgzvn.html

ROLLBACK;
来源：http://hz.tianlin.xyz/gtqhreddxg.html

[Q66] 行锁查询
来源：http://hz.fzhhl.top/gtisdwexkj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hywenlv.cn/gtkcgjwips.html

[Q67] 设置隔离级别
来源：http://hz.shuidangran.top/gtsaynjjdp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gtrtvdqzrc.html

[Q68] 保存点
来源：http://hz.zhixingplan.top/gtanpzbmkr.html

SAVEPOINT sp1;
来源：http://hz.zhaomingkeji.xyz/gtqmcgvmmd.html

ROLLBACK TO sp1;
来源：http://hz.havefunace.top/gtmjcztzhh.html

[Q69] 查看执行计划
来源：http://hz.daria6918.cn/gtkwqffcdi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.smart0.xyz/gtrkuvzlrf.html

[Q70] 更新统计信息
来源：http://hz.nwbrower.top/gtheibpbyb.html

ANALYZE TABLE users;
来源：http://hz.chenzaomai.com/gtqnlxdehb.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtgawoubin.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhiwuduotai.top/gtthxaclrq.html

[Q72] 查看索引
来源：http://hz.sweek.top/gtzxkvjkkh.html

SHOW INDEX FROM users;
来源：http://hz.ydzc1.top/gtckhnuphm.html

[Q73] 查看表状态
来源：http://hz.shuidangran.top/gtpeeewnon.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.52xcode.cn/gtxzqiwkiy.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtclbfbyqv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtcvaihklt.html

[Q75] 日期格式化
来源：http://hz.svipenyu.cn/gtycdiqnyx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yonumen.top/gtotkclkzy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtuqtonabf.html

[Q76] 按天统计
来源：http://hz.yonumen.top/gthiztqdsj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pycfn.com/gtvrjgavji.html

[Q77] 时间加减
来源：http://hz.pengpengdd.cyou/gtpicympda.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.aizwys.cn/gtriwkdozk.html

[Q78] 当前时间
来源：http://hz.jinyuanbaomall.cn/gttwbdfldt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.haohaochexian.top/gtrmvltbhq.html

[Q79] 字符串拼接
来源：http://hz.jiagoushi.top/gtaagqxoyf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnqzz.top/gtjxqbdwfh.html

[Q80] 字符串截取
来源：http://hz.52xcode.cn/gtmnhaghqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pengpengdd.cyou/gtqishubic.html

[Q81] 字符串替换
来源：http://hz.zdqjudy.top/gtotshvqtl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhongyouzk.top/gtgfkgwgip.html

[Q82] 字符长度与字节长度
来源：http://hz.hywenlv.cn/gtsvmxrdqb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cucudq.cn/gtkaldaada.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtzfnutuyi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtcggqdetb.html

[Q84] 去除首尾空格
来源：http://hz.shuidangran.top/gttcpvuagc.html

SELECT TRIM(name) FROM users;
来源：http://hz.sweek.top/gtmnmghdrv.html

[Q85] 数值取整
来源：http://hz.bjfxy.top/gtcqclowyk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aizwys.cn/gtjtueznei.html

[Q86] 读取 JSON 字段
来源：http://hz.tian-w.cn/gtqzbykivg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aizwys.cn/gtflbijzhy.html

[Q87] JSON 字段做条件
来源：http://hz.sufxvd.cn/gtnhjjmlsa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jiagoushi.top/gtphdbksmj.html

[Q88] 行转列（条件聚合）
来源：http://hz.zycfv.cn/gtzgsqrbkk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daxiang520.top/gtfsdlcnst.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cdnleiting.top/gtwihjjxep.html

[Q89] 判断表是否存在
来源：http://hz.chenzaomai.com/gtqgeoybgh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daria6918.cn/gtdduompha.html

[Q90] 生成序号列
来源：http://hz.yonumen.top/gtxhqfmlmt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hongshengwenyu.top/gtnozlyxzb.html

================================================================================
来源：http://hz.cdnleiting.top/gtcouodyjw.html

R. Bash 专题
来源：http://hz.chenjidiqi.icu/gtbgvejsry.html

================================================================================
来源：http://hz.hnxiangtu.top/gtpqjwytjq.html

[R01] shebang 与严格模式
来源：http://hz.havefunace.top/gthsmyrqvm.html

#!/usr/bin/env bash
来源：http://hz.zycfv.cn/gtkbbjbqwc.html

set -euo pipefail
来源：http://hz.yuanzhike.top/gtaffxijoo.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtfcsyeigs.html

name="Tom"; echo "$name"
来源：http://hz.ybcxt.top/gtgybrhjib.html

[R03] 只读变量
来源：http://hz.smart0.xyz/gtycnqkoox.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtaueqzrjb.html

[R04] 位置参数
来源：http://hz.feifeiyinyue.top/gtbdkxtrti.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dashuyun.cn/gtpwppbmoe.html

[R05] 参数默认值
来源：http://hz.nanxuanxn.top/gtqijqaaws.html

name="${1:-default}"
来源：http://hz.chenzaomai.com/gtuokzvxmh.html

[R06] 判断命令是否存在
来源：http://hz.xuetiantiany.cn/gtxgomkmmn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gtwajdjnup.html

[R07] if 判断文件
来源：http://hz.yongpay.top/gtucsecaef.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.snrcjt.cn/gthevkrftr.html

[R08] 数值比较
来源：http://hz.nanxinkj.top/gtvsiogjmf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuetiantiany.cn/gtfhntxvep.html

[R09] 字符串比较
来源：http://hz.zhengqikj.top/gtmxcfrcmq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnxiangtu.top/gtvjpqkclr.html

[R10] 正则匹配
来源：http://hz.andypj.xyz/gtyxzrcudi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tian-w.cn/gtqmqkqgsx.html

[R11] case 多分支
来源：http://hz.wangshuangyany.cn/gtrsroiddr.html

case "$1" in
来源：http://hz.nanxuanxn.top/gtferajpad.html

start) echo "启动" ;;
来源：http://hz.sufxvd.cn/gtdtdaamtg.html

stop)  echo "停止" ;;
来源：http://hz.hfpthk.cn/gtrhoyfvtj.html

*)     echo "未知命令" ;;
来源：http://hz.cdnleiting.top/gtawvkhqdl.html

esac
来源：http://hz.jinqigufen.top/gtwvtkbxma.html

[R12] for 遍历文件
来源：http://hz.yuanzhike.top/gtwzvbhvzl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.9152youxi.cn/gtvqepvkrh.html

[R13] for 计数循环
来源：http://hz.shanyushiyangkeji.top/gtojjhhvle.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ehwqpu.com/gtjqslnwvq.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtcjkilqvp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenlongwang.top/gtzgyhyqdm.html

[R15] while 逐行读文件
来源：http://hz.shzxlz.cn/gtrauehwqa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtewlrwdix.html

[R16] until 等待条件
来源：http://hz.shzxlz.cn/gtahhnpvvr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtpccsaejp.html

[R17] 数组定义与取值
来源：http://hz.xinyue.icu/gtiryttoav.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtvcajcdrn.html

[R18] 遍历数组
来源：http://hz.vqdsnc.cn/gtnjriuwla.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gaohongyu789.top/gtnyguyxsv.html

[R19] 数组长度
来源：http://hz.chenzaomai.com/gtcdihqgvv.html

echo "${#arr[@]}"
来源：http://hz.meibo888.top/gtdmmnyext.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gtsrkdzabu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtxoboynym.html

[R21] 字符串长度
来源：http://hz.ywan-chungtsiang.top/gtfcveyion.html

echo "${#s}"
来源：http://hz.316326.xyz/gtgzddqxuz.html

[R22] 截取子串
来源：http://hz.sysykeji.top/gtqhpdndka.html

echo "${s:0:5}"
来源：http://hz.tanke756.top/gtpfiispgm.html

[R23] 字符串替换
来源：http://hz.smart0.xyz/gtzvedksee.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuxming.cn/gtfrcjtmyf.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gtiqckpstj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhoulong.xyz/gtfjseiujx.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtvqesibau.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenjidiqi.icu/gtsbqiesdb.html

[R26] 命令替换
来源：http://hz.shanyushiyangtech.top/gtegpdffpa.html

now=$(date +%F); echo "$now"
来源：http://hz.nwbrower.top/gtftfpkxey.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtuyqfwcvf.html

echo $((1 + 2 * 3))
来源：http://hz.jinyuanbaomall.cn/gtwnbslrci.html

[R28] 浮点运算
来源：http://hz.bjfxy.top/gtqylktswx.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gtrxswfliz.html

[R29] 定义函数
来源：http://hz.cashguo.top/gtdnaxnidj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xinyue.icu/gtdquwhqja.html

[R30] 函数返回状态码
来源：http://hz.zycfv.cn/gtrvhjjnnc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtsdwrrmwt.html

[R31] 局部变量
来源：http://hz.ivvv.top/gtuhsfocyt.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuetiantiany.cn/gtfyzsbafp.html

[R32] 参数个数校验
来源：http://hz.shzxlz.cn/gtbsoafmzt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.0kj1m.cn/gtoemjxhbq.html

[R33] 捕获错误并提示行号
来源：http://hz.ydzc1.top/gtnajxcwds.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtjjtqmspu.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtzpdztnam.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gthmdpjpqu.html

[R35] 后台执行并等待
来源：http://hz.jyoumei.cn/gtmzghunis.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fzhhl.top/gtyhmmhbcl.html

[R36] 并发执行多个任务
来源：http://hz.zhongyouzk.top/gtrwvtrwmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gaohongyu789.top/gthqectumy.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtiscdnjdz.html


<!-- 参考信息 -->