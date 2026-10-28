代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jiagoushi.top/gtnyeofojx.html

TS:   if (x == null) {}
来源：http://hz.hysaishi.cn/gtzwfccjnz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinghuilouyu.cn/gtbzvzmhrg.html

Go:   if x == nil {}
来源：http://hz.0kj1m.cn/gtlnqvdosa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hfpthk.cn/gtkrecyekr.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gtannrglvh.html

[P07] 防抖与节流
来源：http://hz.zhongyouzk.top/gtdyzxbuue.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.daxiang520.top/gtcaemnrnp.html

PHP:  // 手写时间戳比较
来源：http://hz.cdnleiting.top/gtmejftmpn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtfzdmhsag.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtjskwgcuz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj202588.top/gtyzyltjbk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sweek.top/gtnduwltok.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gtlpdyzipd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ydzc1.top/gtmxfpwczs.html

[P08] 处理浮点精度问题
来源：http://hz.ppjwa.cn/gthinrhdmt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jyoumei.cn/gtgahtxrim.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yangfankeji.com/gtchhbimdm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinqigufen.top/gtktbbaska.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hfpthk.cn/gtzbfjilxd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nanxinkj.top/gtbviyvker.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtjmeccycu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.smart0.xyz/gtxqzrpiec.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtcgamvlvq.html

================================================================================
来源：http://hz.fzhhl.top/gtrmatekum.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnxiangtu.top/gtggzuchrg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtpxfqvhav.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtivwtmqdh.html

CREATE TABLE users (
来源：http://hz.cashguo.top/gtvidxazuu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gtjtcnqvya.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ivvv.top/gtuanvoocd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenlongwang.top/gtrwjvogxl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuxming.cn/gtktbzyejj.html

);
来源：http://hz.andypj.xyz/gtflumimbt.html

[Q02] 创建带外键的表
来源：http://hz.jinqigufen.top/gtultkudra.html

CREATE TABLE orders (
来源：http://hz.ehwqpu.com/gtwfgfssmd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtvejwaqfc.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gtlawbngka.html

amount DECIMAL(10, 2),
来源：http://hz.hammf.cn/gtynlqwdwg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gzhubu.top/gtsabybzyf.html

);
来源：http://hz.xuetiantiany.cn/gtgikhzsol.html

[Q03] 增加列
来源：http://hz.nanxinkj.top/gtogcykkjv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gogol.net.cn/gtaeitttld.html

[Q04] 修改列类型
来源：http://hz.jianghu66.top/gthsjnceku.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aizwys.cn/gtyvkjqsvs.html

[Q05] 重命名列
来源：http://hz.sxryk.cn/gtwaxblsed.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.redwolf501.top/gteclqcqze.html

[Q06] 删除列
来源：http://hz.ydzc1.top/gtfximqoio.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.meibo888.top/gtxbreejhy.html

[Q07] 删除表
来源：http://hz.meibo888.top/gtzmeaycgz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sweek.top/gttcsraeta.html

[Q08] 创建普通索引
来源：http://hz.sweek.top/gtunowpkan.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtydedezeq.html

[Q09] 创建唯一索引
来源：http://hz.xuetiantiany.cn/gtozzbjzdx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtrbcyzvpr.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gtonjthrlp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtvpkspnwl.html

[Q11] 一次插入多行
来源：http://hz.mhx1999.top/gtdcyhljwc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydjk.org.cn/gtkkifrmzm.html

[Q12] 插入后取自增 ID
来源：http://hz.dianchejie.cn/gtuvoxajhj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.bjfxy.top/gtaerrhtyk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gtclsohkrd.html

[Q13] 忽略重复插入
来源：http://hz.yj202588.top/gtrqknaefh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pycfn.com/gthywsmccq.html

[Q14] 存在则更新（upsert）
来源：http://hz.zdqjudy.top/gtgstcmsqc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.vqdsnc.cn/gtbnhbfocc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.havefunace.top/gtrupoktih.html

[Q15] 查询全部
来源：http://hz.jianghu66.top/gthgjcjftv.html

SELECT * FROM users;
来源：http://hz.gotoacloud.top/gtfffrcocc.html

[Q16] 查询指定列
来源：http://hz.sxryk.cn/gtbnxuupjo.html

SELECT id, name FROM users;
来源：http://hz.jqgfzy.top/gthpmersoe.html

[Q17] 条件查询
来源：http://hz.dianchejie.cn/gtrhcsxqyy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenlongwang.top/gtgrkfxyxz.html

[Q18] 模糊匹配
来源：http://hz.yvedp.cn/gtpmuvtrvo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinqigufen.top/gtchzttout.html

[Q19] 范围查询
来源：http://hz.hnxiangtu.top/gtetskdjhs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yangfankeji.com/gtyhjgavnx.html

[Q20] IN 列表
来源：http://hz.hammf.cn/gtgllpaipj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fzhhl.top/gtktsxijxi.html

[Q21] 空值判断
来源：http://hz.xuetiantiany.cn/gtqocosrgc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtwbpdgheb.html

[Q22] 排序
来源：http://hz.haohaochexian.top/gtuscipvax.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenzaomai.com/gtuqjysvri.html

[Q23] 分页
来源：http://hz.birdmap.top/gtqlwyxeuj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hysaishi.cn/gttbegvidz.html

[Q24] 去重
来源：http://hz.feifeiyinyue.top/gttaadwbkw.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtwgiprdib.html

[Q25] 只取前 N 条
来源：http://hz.52xcode.cn/gtlqknygqu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.pengpengdd.cyou/gtboaqluxu.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtivfgspwg.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenzaomai.com/gtsdzgsqqc.html

[Q27] 条件计数
来源：http://hz.smart0.xyz/gtrtojsbxf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.52xcode.cn/gtqcsluhoy.html

[Q28] 求和与平均
来源：http://hz.smart0.xyz/gtqufycfls.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.redwolf501.top/gtjcnyxsny.html

[Q29] 最大最小值
来源：http://hz.yangfankeji.com/gtiuwqnvlc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.feifeiyinyue.top/gtexuluvfk.html

[Q30] 分组统计
来源：http://hz.mhx1999.top/gtvgyvnohk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtburrttki.html

[Q31] 分组后过滤
来源：http://hz.bjfxy.top/gtntrpwwnh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnxiangtu.top/gtpprnnejv.html

[Q32] 分组拼接字符串
来源：http://hz.316326.xyz/gttqktlabi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtefppjwok.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aizwys.cn/gtwzfpwykp.html

[Q33] 多列分组
来源：http://hz.yj202588.top/gtkdyzypqt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yvedp.cn/gtmyxsdvim.html

[Q34] 每组取第一条
来源：http://hz.nwbrower.top/gtdkmdbywp.html

SELECT * FROM (
来源：http://hz.sweek.top/gtlcwwtwby.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnxiangtu.top/gtkerthngd.html

) t WHERE rn = 1;
来源：http://hz.yj20258888.top/gtjxxleekd.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gtzfbwauui.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtlbjzsnix.html

[Q36] 左连接
来源：http://hz.jiagoushi.top/gtsxlpikwh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtwtjericw.html

[Q37] 右连接
来源：http://hz.sysykeji.top/gtckgieihf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xziqi.cn/gtckwijtfj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yongpay.top/gtogtccsds.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuxming.cn/gtxwkfwehw.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtklrvvvug.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtxispxtox.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sysykeji.top/gtosaxfijl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.9152youxi.cn/gtclixbaph.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtldmznzcg.html

[Q41] 多表连接
来源：http://hz.xuetiantiany.cn/gtkganqlcc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ppjwa.cn/gtxcnrrozy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.vqdsnc.cn/gtpyjofonc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnqzz.top/gtmxdxevnj.html

[Q42] 连接条件附加过滤
来源：http://hz.ivvv.top/gtplcirsoz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtgqnwvpen.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yanxiufei.cn/gtcmhpuhde.html

[Q43] 标量子查询
来源：http://hz.zhijiandao.cn/gtqtmyfbdc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinghuilouyu.cn/gtgagrfsqr.html

[Q44] IN 子查询
来源：http://hz.dianchejie.cn/gtjzzrfrae.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangshuangyany.cn/gtockxevxz.html

[Q45] EXISTS 判断存在
来源：http://hz.hammf.cn/gtlbtddrgk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daxiang520.top/gtjfjzmewh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.birdmap.top/gtznyyspjj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gttneazvps.html

[Q47] 与平均值比较
来源：http://hz.dianchejie.cn/gtejwtnrmn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgfzy.top/gtebjroqiy.html

[Q48] CTE 公用表表达式
来源：http://hz.pengpengdd.cyou/gtvvlylccu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigfzy.top/gtvdxdwyvw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtwkhrmfzn.html

[Q49] 更新单行
来源：http://hz.gaohongyu789.top/gtkcljktzl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jiagoushi.top/gtwacdgeoo.html

[Q50] 批量更新
来源：http://hz.ybcxt.top/gtnlvbspsq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.mhx1999.top/gtegjvnxwx.html

[Q51] 用子查询更新
来源：http://hz.pycfn.com/gtssneford.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ywan-chungtsiang.top/gtlyyyntau.html

[Q52] 删除指定行
来源：http://hz.nanxinkj.top/gtetgtuvsv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtsqamgxha.html

[Q53] 按条件删除
来源：http://hz.ywan-chungtsiang.top/gtkvwlusjn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.316326.xyz/gtmtdklpdi.html

[Q54] 清空表
来源：http://hz.shangyingyoupin.top/gtuxuxutpu.html

TRUNCATE TABLE logs;
来源：http://hz.gogol.net.cn/gtmyaljjwa.html

[Q55] 排名（并列占位）
来源：http://hz.ybcxt.top/gteglvvkyf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gzhubu.top/gtadhglfbg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinyuanbaomall.cn/gtnsipnfhc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.snrcjt.cn/gtbtnwjqif.html

[Q57] 行号
来源：http://hz.cucudq.cn/gtpppjogmf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinyuanbaomall.cn/gtxnnlzohx.html

[Q58] 累计求和
来源：http://hz.shanyushiyangtech.top/gthkntfmda.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydzc1.top/gtogjnkmlh.html

[Q59] 分组内累计
来源：http://hz.gogol.net.cn/gthragpxas.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cashguo.top/gtcjsiysyg.html

[Q60] 取上一行 / 下一行
来源：http://hz.birdmap.top/gtdbnjlkqd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cashguo.top/gtiqwfurwr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cashguo.top/gtwmibhvid.html

[Q61] 移动平均
来源：http://hz.cheryme.top/gtsuuelflv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gtogdayswv.html

[Q62] 分组占比
来源：http://hz.xingfuxueyuan.xyz/gtmdydzbyh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gteisvlslm.html

[Q63] 开启事务
来源：http://hz.cheryme.top/gtphxlbtph.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangdashe.top/gthqvqtvoh.html

[Q64] 提交事务
来源：http://hz.yongpay.top/gtmhesztoz.html

COMMIT;
来源：http://hz.shangyingyoupin.top/gtxusfseeb.html

[Q65] 回滚事务
来源：http://hz.yanxiufei.cn/gtzovjkbbo.html

ROLLBACK;
来源：http://hz.pycfn.com/gtlbhmseod.html

[Q66] 行锁查询
来源：http://hz.cqqwz.cn/gtsuglrcsm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhaomingkeji.xyz/gtuarlztqk.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtyzgrwozd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangtech.top/gttmnksioo.html

[Q68] 保存点
来源：http://hz.quarkkingdee.top/gtourokiki.html

SAVEPOINT sp1;
来源：http://hz.jiagoushi.top/gtsbcdnhqa.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtzdcpwuit.html

[Q69] 查看执行计划
来源：http://hz.snrcjt.cn/gtgytcvgke.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhengqikj.top/gttkzsjlcl.html

[Q70] 更新统计信息
来源：http://hz.zhoulong.xyz/gtuonxntgk.html

ANALYZE TABLE users;
来源：http://hz.52xcode.cn/gtqlsfsmmy.html

[Q71] 查看建表语句
来源：http://hz.yvedp.cn/gtmifrvjpj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nanxinkj.top/gtrdnfmlkb.html

[Q72] 查看索引
来源：http://hz.daxiang520.top/gtmykcegur.html

SHOW INDEX FROM users;
来源：http://hz.shzxlz.cn/gtkgclhgsl.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangtech.top/gtrgvvteyd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xinyue.icu/gtkxlcabco.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtncrlvwis.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigufen.top/gtkoklvrzi.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtrthxzxog.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj20258.top/gttqjwssuh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hysaishi.cn/gtyngnpicv.html

[Q76] 按天统计
来源：http://hz.gogol.net.cn/gtruvxndzo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtrhujmxfd.html

[Q77] 时间加减
来源：http://hz.hnqzz.top/gtarmvuasp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtycvuvhba.html

[Q78] 当前时间
来源：http://hz.xuanzx.com/gtivosskpw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hongshengwenyu.top/gtxynoprfa.html

[Q79] 字符串拼接
来源：http://hz.xuanzx.com/gtxsxienyv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zdqjudy.top/gtvrvfpwiu.html

[Q80] 字符串截取
来源：http://hz.gotoacloud.top/gtdctbaovo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigufen.top/gtrtfrajyz.html

[Q81] 字符串替换
来源：http://hz.chenlongwang.top/gtzvjwwqob.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.haohaochexian.top/gtvixnkiad.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtihrnbhjp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.9152youxi.cn/gttepeaujv.html

[Q83] 大小写转换
来源：http://hz.yueranfly.top/gtqdqzirxm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.smart0.xyz/gtztlrlzdk.html

[Q84] 去除首尾空格
来源：http://hz.ybcxt.top/gtkxifosaa.html

SELECT TRIM(name) FROM users;
来源：http://hz.fzhhl.top/gtejqxmilg.html

[Q85] 数值取整
来源：http://hz.svipenyu.cn/gtrhancgpm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhijiandao.cn/gtwuwlhuwr.html

[Q86] 读取 JSON 字段
来源：http://hz.shangyingyoupin.top/gtairuwvie.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuxming.cn/gtoaysjgez.html

[Q87] JSON 字段做条件
来源：http://hz.xuanzx.com/gtfylstuqw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangdashe.top/gtaoaxnirb.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigufen.top/gtjraucwtb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cheryme.top/gtjpzmfreo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuanzx.com/gtmgqmqmzc.html

[Q89] 判断表是否存在
来源：http://hz.mhx1999.top/gttoncqzkk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xuetiantiany.cn/gtypjkicra.html

[Q90] 生成序号列
来源：http://hz.fengsongda.top/gtgtldhytv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.iojbl.cn/gtlmlwdtlw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtchpggihj.html

R. Bash 专题
来源：http://hz.yueranfly.top/gtvelegdax.html

================================================================================
来源：http://hz.wangdashe.top/gtonoiouwg.html

[R01] shebang 与严格模式
来源：http://hz.cdnleiting.top/gtkuboojrk.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtxidythoy.html

set -euo pipefail
来源：http://hz.svipenyu.cn/gtvzujzglv.html

[R02] 变量赋值与使用
来源：http://hz.quarkkingdee.top/gthygeyavr.html

name="Tom"; echo "$name"
来源：http://hz.ivvv.top/gtbmywwknp.html

[R03] 只读变量
来源：http://hz.tianlin.xyz/gtqljsbyzy.html

readonly PI=3.14
来源：http://hz.jqgfzy.top/gtayxsbdcs.html

[R04] 位置参数
来源：http://hz.svipenyu.cn/gtbmxywsie.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtqwiqbeyu.html

[R05] 参数默认值
来源：http://hz.yj20258888.top/gtuquokabj.html

name="${1:-default}"
来源：http://hz.pycfn.com/gtwnvytlwi.html

[R06] 判断命令是否存在
来源：http://hz.fzhhl.top/gtechurpti.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.c1oappe.top/gttosljboy.html

[R07] if 判断文件
来源：http://hz.zhengqikj.top/gtwdedliuc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtwtguqfwf.html

[R08] 数值比较
来源：http://hz.chenlongwang.top/gtmclaqrga.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.redwolf501.top/gtlurpepsp.html

[R09] 字符串比较
来源：http://hz.316326.xyz/gtavkwsgzp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hammf.cn/gtkzisdbrh.html

[R10] 正则匹配
来源：http://hz.shuidangran.top/gttnwesmnv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtktcszxhg.html

[R11] case 多分支
来源：http://hz.gogol.net.cn/gtzdsssqlx.html

case "$1" in
来源：http://hz.cdnleiting.top/gtufbphffw.html

start) echo "启动" ;;
来源：http://hz.daria6918.cn/gtgaglxrzt.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtusixygyy.html

*)     echo "未知命令" ;;
来源：http://hz.fzhhl.top/gtfktfopki.html

esac
来源：http://hz.haohaochexian.top/gtptgqyjon.html

[R12] for 遍历文件
来源：http://hz.ehwqpu.com/gtzxdfxjfn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinyuanbaomall.cn/gtklhjmlar.html

[R13] for 计数循环
来源：http://hz.gaohongyu789.top/gthyrpbfgr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtdhlrsifq.html

[R14] C 风格 for
来源：http://hz.yj202588.top/gticlofdkz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shangyingyoupin.top/gtbjhgbndx.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtlayqmtzg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangtech.top/gtcrxnlymg.html

[R16] until 等待条件
来源：http://hz.316326.xyz/gtlofgfrah.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yangfankeji.com/gtongquret.html

[R17] 数组定义与取值
来源：http://hz.sxryk.cn/gtulrnqqns.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gtirhdcbbg.html

[R18] 遍历数组
来源：http://hz.chenzaomai.com/gtfdvqjjmz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuetiantiany.cn/gtrlglbtkj.html

[R19] 数组长度
来源：http://hz.cdnleiting.top/gtwzkovxap.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gtnmkiybrp.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gtogwewlbg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.meibo888.top/gthnmlovhw.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtdrzhhscj.html

echo "${#s}"
来源：http://hz.svipenyu.cn/gtlmodgsit.html

[R22] 截取子串
来源：http://hz.jqgfzy.top/gtvgwartwm.html

echo "${s:0:5}"
来源：http://hz.chenlongwang.top/gtjoawblau.html

[R23] 字符串替换
来源：http://hz.tanke756.top/gtqjpegjzw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.bjfxy.top/gtpxijkcou.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gthhffuahr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ybcxt.top/gtpidxtiti.html

[R25] 去后缀 / 去前缀
来源：http://hz.cashguo.top/gtocnqqtew.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gzhubu.top/gtaakmhpqm.html

[R26] 命令替换
来源：http://hz.nanxinkj.top/gtqwvtyaoq.html

now=$(date +%F); echo "$now"
来源：http://hz.zdqjudy.top/gtwfjvwlpx.html

[R27] 算术展开
来源：http://hz.sufxvd.cn/gtzitxhbhw.html

echo $((1 + 2 * 3))
来源：http://hz.iojbl.cn/gttlcgtoet.html

[R28] 浮点运算
来源：http://hz.ydjk.org.cn/gthjvcwtxh.html

echo "scale=2; 10/3" | bc
来源：http://hz.daria6918.cn/gtgjltlamd.html

[R29] 定义函数
来源：http://hz.xinyue.icu/gttiphuzqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yongpay.top/gtjcdosdjn.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtegmsdlfn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aizwys.cn/gtpksbxxah.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtbctyojdb.html


<!-- 参考信息 -->