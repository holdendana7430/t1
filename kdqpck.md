代发 wailian999

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtstezikdp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtbpxajvqc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtlhfdkphn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fzhhl.top/gtgryabbfe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtywlgdbcy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj202588.top/gttebahinf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.andypj.xyz/gtjnvxudar.html

[P08] 处理浮点精度问题
来源：http://hz.hongshengwenyu.top/gtemlhzxke.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zdqjudy.top/gtbxmdrjtx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guowangkeji.top/gtqbvcjjwt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yvedp.cn/gtcwevbfds.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.meibo888.top/gttopvioew.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydzc1.top/gtkihmevep.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tianlin.xyz/gtsqzgmkzy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xylfe.cn/gtomlayitv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xingfuxueyuan.xyz/gtszwxilsb.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjeeavbxv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tanke756.top/gtmyildbik.html

================================================================================
来源：http://hz.yvedp.cn/gtorlgofov.html

[Q01] 创建表
来源：http://hz.zycfv.cn/gtdiciwucu.html

CREATE TABLE users (
来源：http://hz.kuanghao11.cn/gtqdrzybdk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gtotvncbfg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.haohaochexian.top/gtyvyafoqi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangdashe.top/gtqgchgndi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinyuanbaomall.cn/gteygnazdb.html

);
来源：http://hz.bjfxy.top/gtwdplrnkz.html

[Q02] 创建带外键的表
来源：http://hz.yanxiufei.cn/gtctcfdnuw.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gtsenrkxci.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtooeeauxd.html

user_id INT NOT NULL,
来源：http://hz.gogol.net.cn/gtjfhumklb.html

amount DECIMAL(10, 2),
来源：http://hz.gogol.net.cn/gtzavykvqb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ehwqpu.com/gtjchvlwit.html

);
来源：http://hz.mhx1999.top/gtydukvcmb.html

[Q03] 增加列
来源：http://hz.kuanghao11.cn/gtbymrkvux.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.havefunace.top/gtdvzxgxfz.html

[Q04] 修改列类型
来源：http://hz.316326.xyz/gttlzibsop.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zdqjudy.top/gtszvxsghp.html

[Q05] 重命名列
来源：http://hz.andypj.xyz/gtziyczwrl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cucudq.cn/gtesyojyto.html

[Q06] 删除列
来源：http://hz.yj20258.top/gtqfzzqmwh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgfzy.top/gtiwtxvveb.html

[Q07] 删除表
来源：http://hz.ywan-chungtsiang.top/gtpgcunesl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.andypj.xyz/gtamcjhten.html

[Q08] 创建普通索引
来源：http://hz.yj20258888.top/gtmoustzmm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtqezmgbvo.html

[Q09] 创建唯一索引
来源：http://hz.52xcode.cn/gtiztjublc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xinyue.icu/gtmeflrmyj.html

[Q10] 插入单行
来源：http://hz.andypj.xyz/gtcnlohxxu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhijiandao.cn/gtfggnkpca.html

[Q11] 一次插入多行
来源：http://hz.bjfxy.top/gtwctxjrkm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cdnleiting.top/gtgowdrlob.html

[Q12] 插入后取自增 ID
来源：http://hz.xuetiantiany.cn/gtibtawzgv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtbwddyqam.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangshuangyany.cn/gtyhawhdyb.html

[Q13] 忽略重复插入
来源：http://hz.jinyuanbaomall.cn/gtelbgxwnr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.havefunace.top/gtgjjqlkpp.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gtruczywdn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.redwolf501.top/gtscxdcprf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yanxiufei.cn/gtmvabfgel.html

[Q15] 查询全部
来源：http://hz.iojbl.cn/gtudmomtqa.html

SELECT * FROM users;
来源：http://hz.tanke756.top/gtsqtcegaz.html

[Q16] 查询指定列
来源：http://hz.smart0.xyz/gtwlqrltwf.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtbvwfotdu.html

[Q17] 条件查询
来源：http://hz.yvedp.cn/gtecszypoi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jianghu66.top/gtksyrjvii.html

[Q18] 模糊匹配
来源：http://hz.jqgfzy.top/gtubjepiav.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sufxvd.cn/gtoapomqaa.html

[Q19] 范围查询
来源：http://hz.ydjk.org.cn/gtjazrgxdt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigfzy.top/gtnhxrjlfd.html

[Q20] IN 列表
来源：http://hz.shzxlz.cn/gtuglzwtzw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cucudq.cn/gtvjktmxcr.html

[Q21] 空值判断
来源：http://hz.zhengqikj.top/gtkwknyaen.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cqqwz.cn/gtegezwlzx.html

[Q22] 排序
来源：http://hz.gaohongyu789.top/gtpxajdbbj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.havefunace.top/gtacnghpmc.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtmszdupsc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxuanxn.top/gtzuyqlkpb.html

[Q24] 去重
来源：http://hz.cdnleiting.top/gtsevfszsg.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigfzy.top/gthatakohu.html

[Q25] 只取前 N 条
来源：http://hz.zycfv.cn/gtfzmhdbhu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.fengsongda.top/gtkhjpfxhw.html

[Q26] 计数
来源：http://hz.zhixingplan.top/gthaezqpry.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhongyouzk.top/gtvxzxawhc.html

[Q27] 条件计数
来源：http://hz.jianghu66.top/gtaiowhdps.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuetiantiany.cn/gtwenxkvak.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gteuzssmob.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.mhx1999.top/gtarhmcgfl.html

[Q29] 最大最小值
来源：http://hz.smart0.xyz/gthysmqbhl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.birdmap.top/gtjelfwpus.html

[Q30] 分组统计
来源：http://hz.zhiwuduotai.top/gtexjzevvi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtjjacjnvi.html

[Q31] 分组后过滤
来源：http://hz.sysykeji.top/gtajyugmxg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhixingplan.top/gtnihdqmws.html

[Q32] 分组拼接字符串
来源：http://hz.hysaishi.cn/gtzolfzyxa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtfdodgynt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gtkrexuqyg.html

[Q33] 多列分组
来源：http://hz.jqgfzy.top/gtlawdgkwv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuetiantiany.cn/gtvzawmmom.html

[Q34] 每组取第一条
来源：http://hz.hammf.cn/gtbjbicmam.html

SELECT * FROM (
来源：http://hz.pengpengdd.cyou/gtaclnkuxs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenjidiqi.icu/gtyecouvsf.html

) t WHERE rn = 1;
来源：http://hz.vqdsnc.cn/gthouzbqhv.html

[Q35] 内连接
来源：http://hz.nanxinkj.top/gtlsfgvenw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtgtvqwvrm.html

[Q36] 左连接
来源：http://hz.zdqjudy.top/gthgqlhpdj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gtubptlbno.html

[Q37] 右连接
来源：http://hz.aizwys.cn/gtlvdebzeo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtpfhmwuwg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shanyushiyangtech.top/gtvjfpvivv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yvedp.cn/gtswwtafat.html

[Q39] 自连接（查上下级）
来源：http://hz.yj202588.top/gtrhgvshvh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangkeji.top/gtjtazmsid.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigufen.top/gtwdxhirhb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yvedp.cn/gtntapgmvc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtjznpypjr.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gteelwbcmo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nwbrower.top/gtzuntzcmj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aibaodan.cn/gtassaocjz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gtvkmjppod.html

[Q42] 连接条件附加过滤
来源：http://hz.bjfxy.top/gtgzgcxzzn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hywenlv.cn/gtnckcgnmu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydjk.org.cn/gtfuvfnvky.html

[Q43] 标量子查询
来源：http://hz.shzxlz.cn/gtwyihoubu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.feifeiyinyue.top/gtyxoweecv.html

[Q44] IN 子查询
来源：http://hz.aizwys.cn/gtylufjndu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yonumen.top/gtadmramju.html

[Q45] EXISTS 判断存在
来源：http://hz.yj202588.top/gtbvzmklsw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tian-w.cn/gtatdfslyu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zdqjudy.top/gtdzqfvwpi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtxpfyahuc.html

[Q47] 与平均值比较
来源：http://hz.feifeiyinyue.top/gtnluggyzd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hammf.cn/gtrqnurwlr.html

[Q48] CTE 公用表表达式
来源：http://hz.jinghuilouyu.cn/gtyiwphwxy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shzxlz.cn/gtcbwfgntb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pengpengdd.cyou/gtasybjlzk.html

[Q49] 更新单行
来源：http://hz.vqdsnc.cn/gtzkykrjvb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.52xcode.cn/gtavbxzubw.html

[Q50] 批量更新
来源：http://hz.jinghuilouyu.cn/gtkweinyyw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.9152youxi.cn/gtgrciggye.html

[Q51] 用子查询更新
来源：http://hz.jqgufenzy.top/gthfocirqh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shangyingyoupin.top/gtaabptoyj.html

[Q52] 删除指定行
来源：http://hz.nanxinkj.top/gttmbqugrw.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydzc1.top/gtcacrqgrt.html

[Q53] 按条件删除
来源：http://hz.daria6918.cn/gtmeciablj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.havefunace.top/gtxzbroahu.html

[Q54] 清空表
来源：http://hz.ppjwa.cn/gtsczooehl.html

TRUNCATE TABLE logs;
来源：http://hz.tian-w.cn/gtwqmyrtor.html

[Q55] 排名（并列占位）
来源：http://hz.aibaodan.cn/gtizpyamhq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gtrdbgimew.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gzhubu.top/gtqxyaetzj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sweek.top/gtidjckaaw.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtawlcpbif.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtsygezkjl.html

[Q58] 累计求和
来源：http://hz.zdqjudy.top/gtehwdhfqz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ehwqpu.com/gtbwvmrbgt.html

[Q59] 分组内累计
来源：http://hz.bjfxy.top/gtyowhpnij.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fengsongda.top/gthozkmsax.html

[Q60] 取上一行 / 下一行
来源：http://hz.shzxlz.cn/gtgoggoplg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sufxvd.cn/gtrryzjbag.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gtpomtqyad.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gtzffyqalm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gtyqqasugq.html

[Q62] 分组占比
来源：http://hz.jqgufenzy.top/gtgeiomrdh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtieadaetj.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gtlpicofct.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhixingplan.top/gtlmeacnlk.html

[Q64] 提交事务
来源：http://hz.gaohongyu789.top/gtcrcwndob.html

COMMIT;
来源：http://hz.chenlongwang.top/gtlcqepbce.html

[Q65] 回滚事务
来源：http://hz.chenjidiqi.icu/gtlhojoqib.html

ROLLBACK;
来源：http://hz.birdmap.top/gtmkdvobbw.html

[Q66] 行锁查询
来源：http://hz.chenjidiqi.icu/gtwatavzeq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtebbgtabp.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gtxkaudamc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.redwolf501.top/gtfjqaxsfx.html

[Q68] 保存点
来源：http://hz.cdnleiting.top/gtvtukvpgr.html

SAVEPOINT sp1;
来源：http://hz.nanxinkj.top/gtpvvjczdj.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gthwpdjdyz.html

[Q69] 查看执行计划
来源：http://hz.haohaochexian.top/gthwkvuclt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.kuanghao11.cn/gtjfnltzon.html

[Q70] 更新统计信息
来源：http://hz.jinqigfzy.top/gtgjhxgdfj.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtbepyvilg.html

[Q71] 查看建表语句
来源：http://hz.ydzc1.top/gtjtxdjcoy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gthvaadleq.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtwdabzyfu.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtdqbhbxzs.html

[Q73] 查看表状态
来源：http://hz.tianlin.xyz/gtitrulamj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangshuangyany.cn/gttpycxsyu.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtigvlmpke.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hongshengwenyu.top/gtgneupebh.html

[Q75] 日期格式化
来源：http://hz.gaohongyu789.top/gthekmlvdn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtdjsvtbob.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhongyouzk.top/gtjignkzfy.html

[Q76] 按天统计
来源：http://hz.jinghuilouyu.cn/gtgvfrbqah.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj202588.top/gtkigxvgaw.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gtyosijhcr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ybcxt.top/gtrffxqgea.html

[Q78] 当前时间
来源：http://hz.shuidangran.top/gtfctnupvj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtsyfpgvtc.html

[Q79] 字符串拼接
来源：http://hz.yj20258888.top/gtgidmhnuu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yonumen.top/gtyoqqnztt.html

[Q80] 字符串截取
来源：http://hz.yuxming.cn/gtiezybhes.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.birdmap.top/gtmduovndl.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtqvbwacmx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jlsjyb.cn/gtxavlybnx.html

[Q82] 字符长度与字节长度
来源：http://hz.zhiwuduotai.top/gtzvyijuif.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtmfxgygyc.html

[Q83] 大小写转换
来源：http://hz.jianghu66.top/gtgqvhdiiz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gttbtzmpwl.html

[Q84] 去除首尾空格
来源：http://hz.jinqigufen.top/gtxahzpcid.html

SELECT TRIM(name) FROM users;
来源：http://hz.meibo888.top/gttdtxfhfw.html

[Q85] 数值取整
来源：http://hz.nanxuanxn.top/gtxnmzhrdj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.vqdsnc.cn/gtyjarplfl.html

[Q86] 读取 JSON 字段
来源：http://hz.feifeiyinyue.top/gtcototaww.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sweek.top/gtqayevlbq.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtivomfylw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tianlin.xyz/gtajzwwkty.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhengqikj.top/gtjmgnflpf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtczirxtho.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.feifeiyinyue.top/gtgtdhncrj.html

[Q89] 判断表是否存在
来源：http://hz.jqgufenzy.top/gtlrtkhxca.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtfuvcishu.html

[Q90] 生成序号列
来源：http://hz.wangshuangyany.cn/gtipkptlyh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gzhubu.top/gteargvsjn.html

================================================================================
来源：http://hz.316326.xyz/gtyvysbtwk.html

R. Bash 专题
来源：http://hz.xingfuxueyuan.xyz/gthvfztvtt.html

================================================================================
来源：http://hz.fengsongda.top/gtzctauhhp.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gtxdrtxvno.html

#!/usr/bin/env bash
来源：http://hz.chenlongwang.top/gthtibuiqf.html

set -euo pipefail
来源：http://hz.ppjwa.cn/gtumokyrpw.html

[R02] 变量赋值与使用
来源：http://hz.feifeiyinyue.top/gtycffjttv.html

name="Tom"; echo "$name"
来源：http://hz.iojbl.cn/gtfbzzletr.html

[R03] 只读变量
来源：http://hz.yanxiufei.cn/gtcnfpiyif.html

readonly PI=3.14
来源：http://hz.xziqi.cn/gtjaptswiw.html

[R04] 位置参数
来源：http://hz.yuanzhike.top/gtotcloqeb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.0kj1m.cn/gtcpnqflmm.html

[R05] 参数默认值
来源：http://hz.316326.xyz/gtvdnzoxoq.html

name="${1:-default}"
来源：http://hz.ehwqpu.com/gtrnebwxnu.html

[R06] 判断命令是否存在
来源：http://hz.ydjk.org.cn/gtiqvpgcyc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.0kj1m.cn/gtlqsnnbdt.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtwygxyeep.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtvqpyqisb.html

[R08] 数值比较
来源：http://hz.hfpthk.cn/gtbjkvozzp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shuidangran.top/gtsyfxxrqe.html

[R09] 字符串比较
来源：http://hz.shzxlz.cn/gtjjpxrpyg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenlongwang.top/gtkdcnbkxr.html

[R10] 正则匹配
来源：http://hz.hfpthk.cn/gtyibfopip.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ydjk.org.cn/gtzogdayrr.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtwrvzymav.html

case "$1" in
来源：http://hz.jiagoushi.top/gtouimhjnv.html

start) echo "启动" ;;
来源：http://hz.jinyuanbaomall.cn/gtfdiycsye.html

stop)  echo "停止" ;;
来源：http://hz.jlsjyb.cn/gticuaqeqg.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gtntetladm.html

esac
来源：http://hz.tian-w.cn/gtnnggpyzq.html

[R12] for 遍历文件
来源：http://hz.hnqzz.top/gtqotxirsn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.redwolf501.top/gtpqqrdsyt.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gtobtsbixs.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sxryk.cn/gtohapnpit.html

[R14] C 风格 for
来源：http://hz.tianlin.xyz/gtsszookfp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yuxming.cn/gtccznpcrs.html

[R15] while 逐行读文件
来源：http://hz.cheryme.top/gtmokafzoj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhixingplan.top/gtrikjfwot.html

[R16] until 等待条件
来源：http://hz.ppjwa.cn/gtdqxnhuxi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.0kj1m.cn/gtifrjsvyv.html

[R17] 数组定义与取值
来源：http://hz.yongpay.top/gtswqsgbny.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shangyingyoupin.top/gtxbyyprgi.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtllhdgdbl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gotoacloud.top/gttwjcqddm.html

[R19] 数组长度
来源：http://hz.sysykeji.top/gtsyerltpv.html

echo "${#arr[@]}"
来源：http://hz.c1oappe.top/gtzyqwcoec.html

[R20] 关联数组（字典）
来源：http://hz.jqgfzy.top/gtbrdotyvn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangtech.top/gtyvmgnbvn.html

[R21] 字符串长度
来源：http://hz.jinqigufen.top/gtewsohfbz.html

echo "${#s}"
来源：http://hz.fengsongda.top/gtyqjlxdpl.html

[R22] 截取子串
来源：http://hz.tian-w.cn/gtektloxld.html

echo "${s:0:5}"
来源：http://hz.cucudq.cn/gtaucitdmh.html

[R23] 字符串替换
来源：http://hz.shanyushiyangtech.top/gtzubelrav.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinyuanbaomall.cn/gtilhmbtjz.html

[R24] 大小写转换
来源：http://hz.yueranfly.top/gtibcfatzq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ehwqpu.com/gthlgukejy.html

[R25] 去后缀 / 去前缀
来源：http://hz.shzxlz.cn/gtnlbbdbxt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shzxlz.cn/gttchocvof.html

[R26] 命令替换
来源：http://hz.hammf.cn/gtakjgpuse.html

now=$(date +%F); echo "$now"
来源：http://hz.redwolf501.top/gtdeeapres.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gtkagwxskj.html

echo $((1 + 2 * 3))
来源：http://hz.cheryme.top/gtkjnecsnf.html

[R28] 浮点运算
来源：http://hz.ehwqpu.com/gtfesivfbz.html

echo "scale=2; 10/3" | bc
来源：http://hz.nwbrower.top/gtdsvnudxr.html

[R29] 定义函数
来源：http://hz.feifeiyinyue.top/gtqiikfyzh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cqqwz.cn/gtsoffzade.html

[R30] 函数返回状态码
来源：http://hz.dashuyun.cn/gtnzbjpqna.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhixingplan.top/gtxohcgeyz.html

[R31] 局部变量
来源：http://hz.sysykeji.top/gtdcyfuqad.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhongyouzk.top/gttznqefjf.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gtibzdevkr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhoulong.xyz/gtkoijnbcu.html

[R33] 捕获错误并提示行号
来源：http://hz.gotoacloud.top/gtlhwetrkr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhijiandao.cn/gtrblustev.html

[R34] 退出时清理
来源：http://hz.andypj.xyz/gtrpqepuka.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtggkkqrgh.html

[R35] 后台执行并等待
来源：http://hz.andypj.xyz/gtlpuipnkw.html


<!-- 参考信息 -->