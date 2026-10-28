代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aibaodan.cn/gtftmtpzod.html

C#:   if (x is null) {}
来源：http://hz.sysykeji.top/gttqwvfhta.html

[P07] 防抖与节流
来源：http://hz.yj20258888.top/gtiiplxaep.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shuidangran.top/gtabwxgkfx.html

PHP:  // 手写时间戳比较
来源：http://hz.pycfn.com/gtmcwloiyj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gtwttskhbf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtcoxhhizb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.iojbl.cn/gtwmafungr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jianghu66.top/gtlzgaqipj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.316326.xyz/gtjzxkxenr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtciwnlxls.html

[P08] 处理浮点精度问题
来源：http://hz.snrcjt.cn/gtphrdiqfs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.birdmap.top/gtujpnvkxe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xziqi.cn/gtulcuesha.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtdqhlqkji.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtewbohyxf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangtech.top/gtjhwnuyla.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gaohongyu789.top/gtavvsbwmc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.birdmap.top/gtgayibajt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgufenzy.top/gtwhdywifm.html

================================================================================
来源：http://hz.aibaodan.cn/gtiwkjfblp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.mhx1999.top/gtzoaliybp.html

================================================================================
来源：http://hz.gogol.net.cn/gtuqfduaks.html

[Q01] 创建表
来源：http://hz.xziqi.cn/gtsjndjvby.html

CREATE TABLE users (
来源：http://hz.yj20258888.top/gtmvtfasxf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtptkajdja.html

name VARCHAR(50) NOT NULL,
来源：http://hz.0kj1m.cn/gtqnaeleee.html

email VARCHAR(100) UNIQUE,
来源：http://hz.0kj1m.cn/gtgxjflwoh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.bjfxy.top/gtvbdkoqbf.html

);
来源：http://hz.chenlongwang.top/gthicjtdhp.html

[Q02] 创建带外键的表
来源：http://hz.hysaishi.cn/gtfttuflxs.html

CREATE TABLE orders (
来源：http://hz.sxryk.cn/gtnonibvye.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtpgadqemj.html

user_id INT NOT NULL,
来源：http://hz.xuetiantiany.cn/gtcsuvpkev.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gttlrgqhie.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.9152youxi.cn/gtoeuubsjj.html

);
来源：http://hz.hongshengwenyu.top/gtspdcnczi.html

[Q03] 增加列
来源：http://hz.ppjwa.cn/gtkcezjjhz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hywenlv.cn/gtrmlkvccy.html

[Q04] 修改列类型
来源：http://hz.hysaishi.cn/gtgdbwpbbv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hysaishi.cn/gteszbllig.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gtezhfbvyy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xinyue.icu/gtzatngkim.html

[Q06] 删除列
来源：http://hz.52xcode.cn/gtjtrforyx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zdqjudy.top/gtsvielwes.html

[Q07] 删除表
来源：http://hz.jinqigufen.top/gtkinncqcu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ydjk.org.cn/gtzcojzhvr.html

[Q08] 创建普通索引
来源：http://hz.sufxvd.cn/gtxhprdwav.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shzxlz.cn/gttnwrwhrd.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtyqjzgmip.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shuidangran.top/gtaihpaztr.html

[Q10] 插入单行
来源：http://hz.tianlin.xyz/gtodorabmr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.mhx1999.top/gtewvxjsrc.html

[Q11] 一次插入多行
来源：http://hz.bjfxy.top/gtffxyqplw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.guannengcc.top/gtqdhzhals.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgfzy.top/gtypnckjhq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258888.top/gtokkczdkk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yongpay.top/gtkzaozogh.html

[Q13] 忽略重复插入
来源：http://hz.yueranfly.top/gtxpulsfla.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gtjhvhiqvc.html

[Q14] 存在则更新（upsert）
来源：http://hz.fengsongda.top/gtjddtqsul.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yueranfly.top/gtwwwrgeuj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhiwuduotai.top/gtnmdzodzw.html

[Q15] 查询全部
来源：http://hz.pengpengdd.cyou/gtsolysblo.html

SELECT * FROM users;
来源：http://hz.iojbl.cn/gthgrvlnav.html

[Q16] 查询指定列
来源：http://hz.yanxiufei.cn/gtvuofeask.html

SELECT id, name FROM users;
来源：http://hz.xuanzx.com/gtptelpbda.html

[Q17] 条件查询
来源：http://hz.hongshengwenyu.top/gtrbetyqsa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenjidiqi.icu/gtspmbdnvb.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gtwezfpmvf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gogol.net.cn/gtimadsloy.html

[Q19] 范围查询
来源：http://hz.jinqigfzy.top/gtifgvopyb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtzbgifska.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gtjzzjpjeq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hammf.cn/gtbtjfmnqh.html

[Q21] 空值判断
来源：http://hz.jinqigfzy.top/gtrampkdhy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuanzhike.top/gtwbhajuvg.html

[Q22] 排序
来源：http://hz.hnxiangtu.top/gtcoipshel.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tanke756.top/gtufsihvxp.html

[Q23] 分页
来源：http://hz.tanke756.top/gtgxhjcocu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.andypj.xyz/gtbczzxnoo.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gtzooxlnqk.html

SELECT DISTINCT city FROM users;
来源：http://hz.yueranfly.top/gtkbeeicri.html

[Q25] 只取前 N 条
来源：http://hz.shuidangran.top/gtnzmajelg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.svipenyu.cn/gtahtriacx.html

[Q26] 计数
来源：http://hz.guannengcc.top/gtygtcvnmt.html

SELECT COUNT(*) FROM users;
来源：http://hz.fzhhl.top/gttkmylxmw.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gtvcyzobyh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hammf.cn/gtepecnxlv.html

[Q28] 求和与平均
来源：http://hz.yonumen.top/gtwxwferse.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.kuanghao11.cn/gtqckkmdru.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gthbyrsspw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtenpbipwi.html

[Q30] 分组统计
来源：http://hz.nanxinkj.top/gtutadfffh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtmxfpjtns.html

[Q31] 分组后过滤
来源：http://hz.redwolf501.top/gtjgtfacek.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhaomingkeji.xyz/gtvcduehjr.html

[Q32] 分组拼接字符串
来源：http://hz.sysykeji.top/gtglduuxcc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtwitryvkd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.0kj1m.cn/gtvpaecpky.html

[Q33] 多列分组
来源：http://hz.nanxuanxn.top/gtliodtbpk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhiwuduotai.top/gtlzejiauu.html

[Q34] 每组取第一条
来源：http://hz.sxryk.cn/gtirqijkzu.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtohwcanea.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shuidangran.top/gtkscfyamh.html

) t WHERE rn = 1;
来源：http://hz.jinqigfzy.top/gtefjphfsg.html

[Q35] 内连接
来源：http://hz.jlsjyb.cn/gtujegmvnb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtvhtpfplv.html

[Q36] 左连接
来源：http://hz.yonumen.top/gtbwhcylqk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gthrknyqkh.html

[Q37] 右连接
来源：http://hz.ydzc1.top/gtllramvao.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guowangkeji.top/gtklhrejdt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shangyingyoupin.top/gtxhigwwwt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhijiandao.cn/gtfphvgcic.html

[Q39] 自连接（查上下级）
来源：http://hz.cdnleiting.top/gtxafhzbgk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tian-w.cn/gtanpqyatk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cqqwz.cn/gtwjcwwupb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jiagoushi.top/gtdtyvcbnb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nwbrower.top/gtfdkgoxyt.html

[Q41] 多表连接
来源：http://hz.yangfankeji.com/gtamwsvvfm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenlongwang.top/gtahnsoref.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gaohongyu789.top/gttsprccoo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinyuanbaomall.cn/gtwtdtthre.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtmxlapndq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hongshengwenyu.top/gtiafujvut.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.feifeiyinyue.top/gttqyqftau.html

[Q43] 标量子查询
来源：http://hz.c1oappe.top/gtsafnujdy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenjidiqi.icu/gteistsdtb.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gtyqseixet.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtyyjirwbc.html

[Q45] EXISTS 判断存在
来源：http://hz.pycfn.com/gtlguomntn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtvcfgqiph.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gotoacloud.top/gtiuxgjnof.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtamihujvj.html

[Q47] 与平均值比较
来源：http://hz.hysaishi.cn/gtcsaaxfnz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tanke756.top/gtguxnuvan.html

[Q48] CTE 公用表表达式
来源：http://hz.sxryk.cn/gtzpyfvxgp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aizwys.cn/gtdupyoypr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nwbrower.top/gtfjjfvbnk.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtjwflzeyw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.haohaochexian.top/gtxfsadrbk.html

[Q50] 批量更新
来源：http://hz.feifeiyinyue.top/gtfebntorm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hfpthk.cn/gthpqwmcot.html

[Q51] 用子查询更新
来源：http://hz.pengpengdd.cyou/gtmxhsjjau.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ppjwa.cn/gtqivyktpe.html

[Q52] 删除指定行
来源：http://hz.shzxlz.cn/gtpboedtss.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shuidangran.top/gtmqzepqhp.html

[Q53] 按条件删除
来源：http://hz.hongshengwenyu.top/gtytigilla.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.52xcode.cn/gteborgqjl.html

[Q54] 清空表
来源：http://hz.havefunace.top/gtgbgfhvtt.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258888.top/gtlsmiajhm.html

[Q55] 排名（并列占位）
来源：http://hz.daxiang520.top/gtwpsisxri.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtsndhlwbo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hysaishi.cn/gtbxhyehth.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hnxiangtu.top/gtoruoydnf.html

[Q57] 行号
来源：http://hz.xingfuxueyuan.xyz/gtiomujluy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.svipenyu.cn/gtgdjadnic.html

[Q58] 累计求和
来源：http://hz.hongshengwenyu.top/gtqvchbbpr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tianlin.xyz/gtdygbfqoj.html

[Q59] 分组内累计
来源：http://hz.gzhubu.top/gttlctoxed.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.quarkkingdee.top/gtyuhuxvun.html

[Q60] 取上一行 / 下一行
来源：http://hz.daria6918.cn/gtovdlglhs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtkezwpehf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pengpengdd.cyou/gtdltjbidi.html

[Q61] 移动平均
来源：http://hz.svipenyu.cn/gtjskegkuy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuanzx.com/gtnichzkye.html

[Q62] 分组占比
来源：http://hz.yj20258.top/gtovnufzrm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtwmycccmk.html

[Q63] 开启事务
来源：http://hz.jqgufenzy.top/gtqidficqd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sufxvd.cn/gtcrshbpll.html

[Q64] 提交事务
来源：http://hz.yuanzhike.top/gtfhtfmvdo.html

COMMIT;
来源：http://hz.sufxvd.cn/gtkxlogeya.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gttkknxqzt.html

ROLLBACK;
来源：http://hz.xinyue.icu/gtbbplqcia.html

[Q66] 行锁查询
来源：http://hz.jinyuanbaomall.cn/gtpgepzjft.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sweek.top/gtkbxggwkw.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangkeji.top/gtwjhnbnbk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhiwuduotai.top/gtpclapbrd.html

[Q68] 保存点
来源：http://hz.cheryme.top/gtxdkjznds.html

SAVEPOINT sp1;
来源：http://hz.jqgfzy.top/gtejeywskp.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gtoeydbbzj.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtqsbbgvot.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xuanzx.com/gtzpuwbjwn.html

[Q70] 更新统计信息
来源：http://hz.yangfankeji.com/gtpadefzny.html

ANALYZE TABLE users;
来源：http://hz.cashguo.top/gtgpizmjmm.html

[Q71] 查看建表语句
来源：http://hz.shuidangran.top/gtijamxubu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yuanzhike.top/gtqlfwdrzu.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gtqnjazhjx.html

SHOW INDEX FROM users;
来源：http://hz.c1oappe.top/gtjkmjrurb.html

[Q73] 查看表状态
来源：http://hz.xingfuxueyuan.xyz/gtlmozpsod.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hammf.cn/gtnjeqgymt.html

[Q74] 强制使用索引
来源：http://hz.xziqi.cn/gthfffdbbu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shzxlz.cn/gtbmutcjzl.html

[Q75] 日期格式化
来源：http://hz.pengpengdd.cyou/gtrmhhqdlm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.feifeiyinyue.top/gtlbrwrwve.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gticoenutp.html

[Q76] 按天统计
来源：http://hz.xziqi.cn/gteutskuts.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.52xcode.cn/gtazggxtde.html

[Q77] 时间加减
来源：http://hz.zhiwuduotai.top/gtfndpvcsv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhongyouzk.top/gtdnyhoimu.html

[Q78] 当前时间
来源：http://hz.hongshengwenyu.top/gthhcuklec.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.quarkkingdee.top/gtxxzsuyyc.html

[Q79] 字符串拼接
来源：http://hz.9152youxi.cn/gtbqqandsm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangshuangyany.cn/gtqdcgiqfe.html

[Q80] 字符串截取
来源：http://hz.sufxvd.cn/gtxqetsull.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zycfv.cn/gtvcorjcgg.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gthohrdzuo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tian-w.cn/gtmairkela.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gtmydtenvx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtzghwefwi.html

[Q83] 大小写转换
来源：http://hz.yj202588.top/gtehhcgabc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gogol.net.cn/gtgwjflcbh.html

[Q84] 去除首尾空格
来源：http://hz.jiagoushi.top/gtovckssbc.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhengqikj.top/gttsndktju.html

[Q85] 数值取整
来源：http://hz.tian-w.cn/gtoanzuhsn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnqzz.top/gtxhdgqufo.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtzqdjrhwn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guannengcc.top/gtbnxzmekv.html

[Q87] JSON 字段做条件
来源：http://hz.sweek.top/gtlyatatnd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hammf.cn/gtdinmkvva.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258.top/gtcngjjoym.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtkmjsiogc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.quarkkingdee.top/gtusjcdkkz.html

[Q89] 判断表是否存在
来源：http://hz.xziqi.cn/gtoqcgviju.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shangyingyoupin.top/gttvzsnawi.html

[Q90] 生成序号列
来源：http://hz.yj202588.top/gtlrqvzqwc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangdashe.top/gtjivbhphd.html

================================================================================
来源：http://hz.ydzc1.top/gtkystxkli.html

R. Bash 专题
来源：http://hz.yanxiufei.cn/gtfqrqmzgu.html

================================================================================
来源：http://hz.zhijiandao.cn/gtnklfscrn.html

[R01] shebang 与严格模式
来源：http://hz.zdqjudy.top/gtjzbkgsbg.html

#!/usr/bin/env bash
来源：http://hz.fzhhl.top/gtmdidvudb.html

set -euo pipefail
来源：http://hz.fzhhl.top/gtaupbhoen.html

[R02] 变量赋值与使用
来源：http://hz.tian-w.cn/gteqlmcirz.html

name="Tom"; echo "$name"
来源：http://hz.jinyuanbaomall.cn/gtweqsemdx.html

[R03] 只读变量
来源：http://hz.shuidangran.top/gtcrtvnydg.html

readonly PI=3.14
来源：http://hz.jyoumei.cn/gttpsgankf.html

[R04] 位置参数
来源：http://hz.sweek.top/gtdsgsiklt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtmtlfnixb.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gtiiwdutqq.html

name="${1:-default}"
来源：http://hz.fzhhl.top/gtdihpabkz.html

[R06] 判断命令是否存在
来源：http://hz.fengsongda.top/gtallqcbxp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtmpfefpvc.html

[R07] if 判断文件
来源：http://hz.mhx1999.top/gtkjijertf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.snrcjt.cn/gtrfvomkuh.html

[R08] 数值比较
来源：http://hz.0kj1m.cn/gtjnwdnigz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtezriwvca.html

[R09] 字符串比较
来源：http://hz.hammf.cn/gtzuhrmvxy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ppjwa.cn/gtfzydfhst.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtuzaiinkf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinyuanbaomall.cn/gtjzuphwuw.html

[R11] case 多分支
来源：http://hz.yongpay.top/gtvwkgsuzv.html

case "$1" in
来源：http://hz.cheryme.top/gthidfgiwd.html

start) echo "启动" ;;
来源：http://hz.0kj1m.cn/gtrebknnsq.html

stop)  echo "停止" ;;
来源：http://hz.cucudq.cn/gtxisznhlq.html

*)     echo "未知命令" ;;
来源：http://hz.wangshuangyany.cn/gtlbmcpssx.html

esac
来源：http://hz.c1oappe.top/gtjelcasio.html

[R12] for 遍历文件
来源：http://hz.chenjidiqi.icu/gtqzpwafjj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jyoumei.cn/gtetsknddb.html

[R13] for 计数循环
来源：http://hz.hongshengwenyu.top/gtyaeqfidm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangdashe.top/gtwsgasmpo.html

[R14] C 风格 for
来源：http://hz.shangyingyoupin.top/gtrweuzdxz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtzvpunbft.html

[R15] while 逐行读文件
来源：http://hz.yueranfly.top/gtkgyttvth.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hammf.cn/gtsoaaptgh.html

[R16] until 等待条件
来源：http://hz.jinyuanbaomall.cn/gtniddzsuo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xuanzx.com/gtozbpvflu.html

[R17] 数组定义与取值
来源：http://hz.tianlin.xyz/gtsxxvbmpx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangdashe.top/gtxgavircl.html

[R18] 遍历数组
来源：http://hz.ehwqpu.com/gtgyfznwnc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.birdmap.top/gtdpqgoamm.html

[R19] 数组长度
来源：http://hz.shanyushiyangtech.top/gtdkmbjmtb.html

echo "${#arr[@]}"
来源：http://hz.xylfe.cn/gtycgsnrnq.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtfvsiwikb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhijiandao.cn/gtfqowzyqs.html

[R21] 字符串长度
来源：http://hz.jqgfzy.top/gtrclqjdcz.html

echo "${#s}"
来源：http://hz.yanxiufei.cn/gtxurtdixi.html

[R22] 截取子串
来源：http://hz.guannengcc.top/gtkehzbcdk.html

echo "${s:0:5}"
来源：http://hz.feifeiyinyue.top/gtpyierqjj.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtzwbncgba.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yonumen.top/gtpjpnkjeh.html

[R24] 大小写转换
来源：http://hz.ppjwa.cn/gtwythwarc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pengpengdd.cyou/gtjaytdkkm.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gttnfqgtbz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gzhubu.top/gthwmnhqmf.html

[R26] 命令替换
来源：http://hz.fzhhl.top/gtdxjciiep.html

now=$(date +%F); echo "$now"
来源：http://hz.cqqwz.cn/gtwmoqezmx.html

[R27] 算术展开
来源：http://hz.hammf.cn/gtcrbjyfdg.html

echo $((1 + 2 * 3))
来源：http://hz.52xcode.cn/gttrrcnmcz.html

[R28] 浮点运算
来源：http://hz.nanxinkj.top/gtkcxhmygq.html

echo "scale=2; 10/3" | bc
来源：http://hz.fzhhl.top/gtimddsqyf.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtbavoqfri.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sysykeji.top/gtmefyriih.html

[R30] 函数返回状态码
来源：http://hz.0kj1m.cn/gtejmvvubi.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtdtkvmmol.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gttatvftwk.html

f() { local x=1; echo "$x"; }
来源：http://hz.sufxvd.cn/gtbxkjjsoi.html

[R32] 参数个数校验
来源：http://hz.yvedp.cn/gtlyeixzcg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.birdmap.top/gtzpoadzbc.html

[R33] 捕获错误并提示行号
来源：http://hz.bjfxy.top/gtvelnpkrq.html


<!-- 参考信息 -->