代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zdqjudy.top/gtmmrldieh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xinyue.icu/gttgqmfiij.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dianchejie.cn/gtwjpnqnim.html

PHP:  if (empty($x)) {}
来源：http://hz.dianchejie.cn/gtlvhfuhjq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.0kj1m.cn/gtgalhsufj.html

TS:   if (x == null) {}
来源：http://hz.ydzc1.top/gtfxclsnle.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtwcrbnsdf.html

Go:   if x == nil {}
来源：http://hz.hongshengwenyu.top/gtdkrjicfq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sweek.top/gtjxlbyboc.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gtaerzjxcb.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gttnzlpxaa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtwxfchozk.html

PHP:  // 手写时间戳比较
来源：http://hz.yj202588.top/gtttnqqzfs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtrrvphbtz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtqemwkhly.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yanxiufei.cn/gtdpsaftnx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenjidiqi.icu/gtriyaremu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gtdjaghioc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nanxinkj.top/gtokxbjvjf.html

[P08] 处理浮点精度问题
来源：http://hz.pengpengdd.cyou/gtthwshiho.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hnxiangtu.top/gtyusbekrt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.316326.xyz/gtztjsbnav.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ehwqpu.com/gtricwqoka.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtegbbjibf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hfpthk.cn/gtfgqayssc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yangfankeji.com/gtiuzvrxve.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangdashe.top/gtpssqcpgi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangshuangyany.cn/gtyroqgmvk.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqbntiktx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.birdmap.top/gtozsfcrua.html

================================================================================
来源：http://hz.shzxlz.cn/gtqxwepsjb.html

[Q01] 创建表
来源：http://hz.zhiwuduotai.top/gttcmsutcc.html

CREATE TABLE users (
来源：http://hz.aibaodan.cn/gtnheuqjul.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtmifkurin.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ppjwa.cn/gtcnxssioq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.9152youxi.cn/gtlavvwimh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.316326.xyz/gtsfzayhuk.html

);
来源：http://hz.kuanghao11.cn/gtfxlaqvmb.html

[Q02] 创建带外键的表
来源：http://hz.shangyingyoupin.top/gtjuofhpoz.html

CREATE TABLE orders (
来源：http://hz.snrcjt.cn/gtdyvotbnh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtihivnlqp.html

user_id INT NOT NULL,
来源：http://hz.yj20258888.top/gtdqaiaiij.html

amount DECIMAL(10, 2),
来源：http://hz.zhaomingkeji.xyz/gtbovploya.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtzqvqdbfe.html

);
来源：http://hz.sysykeji.top/gtndejuzay.html

[Q03] 增加列
来源：http://hz.ivvv.top/gtjdzxdeco.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yongpay.top/gtgymafmpb.html

[Q04] 修改列类型
来源：http://hz.shzxlz.cn/gtyrlfisof.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jyoumei.cn/gtdnlnbwso.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtclbznnjs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.316326.xyz/gtryixxnzs.html

[Q06] 删除列
来源：http://hz.zhixingplan.top/gtppvciuuj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gaohongyu789.top/gtwhsanezx.html

[Q07] 删除表
来源：http://hz.yj202588.top/gttfgzxhyx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinghuilouyu.cn/gtrdpozook.html

[Q08] 创建普通索引
来源：http://hz.ppjwa.cn/gtvgvmrrkv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydzc1.top/gtxtrdxvbl.html

[Q09] 创建唯一索引
来源：http://hz.sysykeji.top/gtlgnzcdzf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sysykeji.top/gtpphfktcp.html

[Q10] 插入单行
来源：http://hz.xziqi.cn/gtuhyrepfi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cdnleiting.top/gtvmcesrgq.html

[Q11] 一次插入多行
来源：http://hz.yanxiufei.cn/gtxprsdbhl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hysaishi.cn/gtikgruffz.html

[Q12] 插入后取自增 ID
来源：http://hz.sweek.top/gtlbekxjtj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhongyouzk.top/gtnqyhwimx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtfpzvmspl.html

[Q13] 忽略重复插入
来源：http://hz.nanxinkj.top/gtpikoeqod.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.316326.xyz/gtbltyooom.html

[Q14] 存在则更新（upsert）
来源：http://hz.gaohongyu789.top/gtyigsvdix.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhixingplan.top/gtxzahdjgb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangdashe.top/gtklbgchwl.html

[Q15] 查询全部
来源：http://hz.xingfuxueyuan.xyz/gtprtwoumu.html

SELECT * FROM users;
来源：http://hz.yuanzhike.top/gtbepxnawp.html

[Q16] 查询指定列
来源：http://hz.jianghu66.top/gtobayarpj.html

SELECT id, name FROM users;
来源：http://hz.gogol.net.cn/gtzrtvkggx.html

[Q17] 条件查询
来源：http://hz.cqqwz.cn/gtasnqldtm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xingfuxueyuan.xyz/gtorcodrmr.html

[Q18] 模糊匹配
来源：http://hz.gogol.net.cn/gtfdpqlwxw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aizwys.cn/gtudzzfdyh.html

[Q19] 范围查询
来源：http://hz.xuanzx.com/gtgscsynks.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinghuilouyu.cn/gtbcvefncc.html

[Q20] IN 列表
来源：http://hz.yj20258888.top/gttllcumey.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pengpengdd.cyou/gtgbklkstr.html

[Q21] 空值判断
来源：http://hz.dashuyun.cn/gtugjjfifw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tianlin.xyz/gtyzlemckr.html

[Q22] 排序
来源：http://hz.yanxiufei.cn/gtrvuucpga.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.feifeiyinyue.top/gtmsqeqgsr.html

[Q23] 分页
来源：http://hz.yongpay.top/gtjtmckoie.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.svipenyu.cn/gtbvogjpdu.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gthgjkzruv.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnxiangtu.top/gtfxxklega.html

[Q25] 只取前 N 条
来源：http://hz.chenlongwang.top/gtthjcdvhm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yanxiufei.cn/gtyqvszwfw.html

[Q26] 计数
来源：http://hz.xuanzx.com/gtolyogcme.html

SELECT COUNT(*) FROM users;
来源：http://hz.xuanzx.com/gtzhvzasqm.html

[Q27] 条件计数
来源：http://hz.ehwqpu.com/gtuxkqwjrh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sysykeji.top/gtdtskwusq.html

[Q28] 求和与平均
来源：http://hz.jqgufenzy.top/gtcuzlkwvw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xziqi.cn/gtzksqobqp.html

[Q29] 最大最小值
来源：http://hz.dashuyun.cn/gthxscjtkt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.meibo888.top/gthylkyxlw.html

[Q30] 分组统计
来源：http://hz.sufxvd.cn/gtjrodwlss.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.c1oappe.top/gtmdqqsxoh.html

[Q31] 分组后过滤
来源：http://hz.nwbrower.top/gtnqgltbzp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenzaomai.com/gtpddqkjdw.html

[Q32] 分组拼接字符串
来源：http://hz.ydjk.org.cn/gtotlnukxv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gthwvsoibr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhaomingkeji.xyz/gtlagcqwyf.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gtijakvszr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuanzx.com/gtarhiiict.html

[Q34] 每组取第一条
来源：http://hz.jyoumei.cn/gtvebsgnze.html

SELECT * FROM (
来源：http://hz.zhaomingkeji.xyz/gtxjeegjqr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gogol.net.cn/gtfobrlykv.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtpatrxeea.html

[Q35] 内连接
来源：http://hz.mhx1999.top/gtzfjpbpfr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangkeji.top/gtgpvgjjzs.html

[Q36] 左连接
来源：http://hz.ehwqpu.com/gtzibbcgys.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtarnhpfhw.html

[Q37] 右连接
来源：http://hz.kuanghao11.cn/gtuydrlzsm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sweek.top/gtqtbjzrkx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jiagoushi.top/gtnwvmhssr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tian-w.cn/gtyhctugei.html

[Q39] 自连接（查上下级）
来源：http://hz.jiagoushi.top/gtxmcjqehf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.redwolf501.top/gtshwkajrg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gtwwjaljxa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhoulong.xyz/gtpnwqubfd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pengpengdd.cyou/gtxmrxqbkf.html

[Q41] 多表连接
来源：http://hz.jinqigufen.top/gtciusthbq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgfzy.top/gtvpdtjzvn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gogol.net.cn/gtggnekquw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.52xcode.cn/gtjotdkbkk.html

[Q42] 连接条件附加过滤
来源：http://hz.hysaishi.cn/gtpkehdnni.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gotoacloud.top/gthqwzyxlr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yonumen.top/gttrfuanwy.html

[Q43] 标量子查询
来源：http://hz.meibo888.top/gtxcwptqny.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.mhx1999.top/gttvtbrvjj.html

[Q44] IN 子查询
来源：http://hz.zhijiandao.cn/gthzqyoxdp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.haohaochexian.top/gtcsoupagg.html

[Q45] EXISTS 判断存在
来源：http://hz.tanke756.top/gtqbtawmil.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtcftyvmfk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xziqi.cn/gthekxzolf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtiblipukg.html

[Q47] 与平均值比较
来源：http://hz.sweek.top/gthvktjhqh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhaomingkeji.xyz/gtlfbghihz.html

[Q48] CTE 公用表表达式
来源：http://hz.daxiang520.top/gtyygptkud.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gaohongyu789.top/gtfqmvpkbl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aizwys.cn/gtciqtqcbx.html

[Q49] 更新单行
来源：http://hz.gogol.net.cn/gtkbmpvrur.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.52xcode.cn/gtcnrtquvo.html

[Q50] 批量更新
来源：http://hz.andypj.xyz/gtfgbhtfum.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cheryme.top/gtymxdhapp.html

[Q51] 用子查询更新
来源：http://hz.jinqigufen.top/gtoqqpbvxd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.fengsongda.top/gtnmrdfbtb.html

[Q52] 删除指定行
来源：http://hz.pengpengdd.cyou/gtpzdnkvcu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fzhhl.top/gtrmukbmsz.html

[Q53] 按条件删除
来源：http://hz.pycfn.com/gtyzwlvaku.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nwbrower.top/gtdvpjzvgq.html

[Q54] 清空表
来源：http://hz.ywan-chungtsiang.top/gthyzqwklu.html

TRUNCATE TABLE logs;
来源：http://hz.mhx1999.top/gthnsqtgmt.html

[Q55] 排名（并列占位）
来源：http://hz.andypj.xyz/gtvqnlqnwp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.andypj.xyz/gtqvdtyhuo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.316326.xyz/gtxqedzjai.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuanzhike.top/gtqkecihqa.html

[Q57] 行号
来源：http://hz.jqgufenzy.top/gtptcicgto.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtzrtczvpp.html

[Q58] 累计求和
来源：http://hz.xuanzx.com/gthanyohsz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gtvhjzajex.html

[Q59] 分组内累计
来源：http://hz.9152youxi.cn/gthdvxeclj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.quarkkingdee.top/gtdbxrbjcc.html

[Q60] 取上一行 / 下一行
来源：http://hz.gaohongyu789.top/gtfhdukhvx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtalaxdwoc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yanxiufei.cn/gtpadhsmwx.html

[Q61] 移动平均
来源：http://hz.kuanghao11.cn/gtgezsesvq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ydzc1.top/gtygtnguzv.html

[Q62] 分组占比
来源：http://hz.gotoacloud.top/gtwlloplgl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtgznwjkvj.html

[Q63] 开启事务
来源：http://hz.yangfankeji.com/gtduopnnoz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenjidiqi.icu/gtcfbexqyb.html

[Q64] 提交事务
来源：http://hz.ppjwa.cn/gttglyqrqo.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gtqtynbffp.html

[Q65] 回滚事务
来源：http://hz.sufxvd.cn/gtcjcokxuc.html

ROLLBACK;
来源：http://hz.fengsongda.top/gtihwjeetq.html

[Q66] 行锁查询
来源：http://hz.yanxiufei.cn/gtyfjvnycn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hnqzz.top/gtkqtrxzrq.html

[Q67] 设置隔离级别
来源：http://hz.andypj.xyz/gtonfbtxpy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinqigfzy.top/gttxhzutqu.html

[Q68] 保存点
来源：http://hz.ydzc1.top/gtiijwefje.html

SAVEPOINT sp1;
来源：http://hz.dianchejie.cn/gtnmknwzel.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtbwhzmolu.html

[Q69] 查看执行计划
来源：http://hz.ehwqpu.com/gtzevebcus.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.andypj.xyz/gtvvjmuqfk.html

[Q70] 更新统计信息
来源：http://hz.sufxvd.cn/gtckfqvron.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtiebssixu.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtnnkgawsd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinqigufen.top/gtmiwonzvz.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gtqygidtsy.html

SHOW INDEX FROM users;
来源：http://hz.52xcode.cn/gtjucrnmzh.html

[Q73] 查看表状态
来源：http://hz.hnqzz.top/gtbjphbmuh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.0kj1m.cn/gtxtymztmn.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtnpaugqdy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gtkcsbscqf.html

[Q75] 日期格式化
来源：http://hz.snrcjt.cn/gttkxsvysc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuanzx.com/gtdvdukobm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gtfyvcousm.html

[Q76] 按天统计
来源：http://hz.sweek.top/gtdemvfahs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jqgfzy.top/gtvqgoezhz.html

[Q77] 时间加减
来源：http://hz.nanxinkj.top/gtdyjwctuc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenlongwang.top/gtbpfjptxw.html

[Q78] 当前时间
来源：http://hz.hywenlv.cn/gtkpoquijm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhijiandao.cn/gtwrbqrbfb.html

[Q79] 字符串拼接
来源：http://hz.fengsongda.top/gtdjgxugwa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yangfankeji.com/gtlfikngtw.html

[Q80] 字符串截取
来源：http://hz.pycfn.com/gtzytpanpf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.52xcode.cn/gtekvmrgoh.html

[Q81] 字符串替换
来源：http://hz.sysykeji.top/gtuftyqhow.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuanzhike.top/gtxciwdxxd.html

[Q82] 字符长度与字节长度
来源：http://hz.c1oappe.top/gtaaoeucup.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtinnbzqgc.html

[Q83] 大小写转换
来源：http://hz.chenjidiqi.icu/gtxzclcftt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sweek.top/gtwxitilnj.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtgbelrygr.html

SELECT TRIM(name) FROM users;
来源：http://hz.jiagoushi.top/gtocyszyor.html

[Q85] 数值取整
来源：http://hz.daria6918.cn/gtputeytdd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gtyqjoktol.html

[Q86] 读取 JSON 字段
来源：http://hz.xziqi.cn/gtynedvzqv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cucudq.cn/gtsdmnjjgr.html

[Q87] JSON 字段做条件
来源：http://hz.yongpay.top/gtfngtotni.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ehwqpu.com/gtfwgnknjj.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtphgxogac.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gogol.net.cn/gtfyhbhuii.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ppjwa.cn/gtgmyhlifm.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gtxvifczwn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fengsongda.top/gtacboytxg.html

[Q90] 生成序号列
来源：http://hz.iojbl.cn/gtrujsehal.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.bjfxy.top/gtvloajzbe.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtbpqnixrk.html

R. Bash 专题
来源：http://hz.havefunace.top/gtqmfpkcjp.html

================================================================================
来源：http://hz.9152youxi.cn/gtsfixjhjp.html

[R01] shebang 与严格模式
来源：http://hz.kuanghao11.cn/gtnujjixcm.html

#!/usr/bin/env bash
来源：http://hz.hongshengwenyu.top/gtpiablptb.html

set -euo pipefail
来源：http://hz.hfpthk.cn/gtksvqlxms.html

[R02] 变量赋值与使用
来源：http://hz.zycfv.cn/gtjkdvnfsq.html

name="Tom"; echo "$name"
来源：http://hz.vqdsnc.cn/gtjguzyujb.html

[R03] 只读变量
来源：http://hz.hfpthk.cn/gtkqrzcrrj.html

readonly PI=3.14
来源：http://hz.zhiwuduotai.top/gtflnichbd.html

[R04] 位置参数
来源：http://hz.jlsjyb.cn/gttwzaunqw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cashguo.top/gtutmjukbh.html

[R05] 参数默认值
来源：http://hz.yj20258888.top/gtnkpxrrns.html

name="${1:-default}"
来源：http://hz.cashguo.top/gtoaqiyvwf.html

[R06] 判断命令是否存在
来源：http://hz.haohaochexian.top/gtuswiulmv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtidhcolyt.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gtdejcybhe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gaohongyu789.top/gtcwgvyqhq.html

[R08] 数值比较
来源：http://hz.fengsongda.top/gtfkxxvgmz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sweek.top/gtsfnicnqx.html

[R09] 字符串比较
来源：http://hz.mhx1999.top/gtweyxlndp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ybcxt.top/gtxyekxokh.html

[R10] 正则匹配
来源：http://hz.zhixingplan.top/gtbhthojae.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhijiandao.cn/gttyuwfrxo.html

[R11] case 多分支
来源：http://hz.sweek.top/gtrnrifjev.html

case "$1" in
来源：http://hz.redwolf501.top/gtzsjxwssf.html

start) echo "启动" ;;
来源：http://hz.yvedp.cn/gtkhrvluqg.html

stop)  echo "停止" ;;
来源：http://hz.xuetiantiany.cn/gtiwfmgyru.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigfzy.top/gtxxkovmgp.html

esac
来源：http://hz.sysykeji.top/gtzhbhtuzc.html

[R12] for 遍历文件
来源：http://hz.guowangkeji.top/gtnumcixwp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.feifeiyinyue.top/gtqgqkxtie.html

[R13] for 计数循环
来源：http://hz.ywan-chungtsiang.top/gtirixxvuw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.redwolf501.top/gtmwggvmfv.html

[R14] C 风格 for
来源：http://hz.nanxinkj.top/gthpkjvwfr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.bjfxy.top/gtvcdpotdp.html

[R15] while 逐行读文件
来源：http://hz.yongpay.top/gtlqckgaza.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigufen.top/gtrayimelj.html

[R16] until 等待条件
来源：http://hz.sweek.top/gtxlqtbxgv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtmyezeuuu.html

[R17] 数组定义与取值
来源：http://hz.yonumen.top/gtfjfpmpby.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ybcxt.top/gtgdazirhy.html

[R18] 遍历数组
来源：http://hz.jqgufenzy.top/gtiypqtthh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.andypj.xyz/gtyrwjrama.html

[R19] 数组长度
来源：http://hz.cheryme.top/gtnrwyvegf.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtgruxzinz.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtbdhjjzas.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnxiangtu.top/gtrygnbbtw.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gtfsydycxm.html

echo "${#s}"
来源：http://hz.fengsongda.top/gtgjqhjrac.html

[R22] 截取子串
来源：http://hz.vqdsnc.cn/gtqzmyttwv.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gthdrhmfkr.html

[R23] 字符串替换
来源：http://hz.aizwys.cn/gtlgwmyeli.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.iojbl.cn/gtmkfpnivc.html

[R24] 大小写转换
来源：http://hz.bjfxy.top/gtscatnums.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aizwys.cn/gtqvljmszb.html

[R25] 去后缀 / 去前缀
来源：http://hz.nwbrower.top/gtnvpdliml.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuetiantiany.cn/gtpedwevac.html

[R26] 命令替换
来源：http://hz.iojbl.cn/gtixqpjwgi.html

now=$(date +%F); echo "$now"
来源：http://hz.zhijiandao.cn/gtcpwzlkyl.html

[R27] 算术展开
来源：http://hz.ybcxt.top/gticfbipkt.html

echo $((1 + 2 * 3))
来源：http://hz.tianlin.xyz/gtdiagprjw.html

[R28] 浮点运算
来源：http://hz.zhengqikj.top/gtkaplukyc.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangtech.top/gtxqlsuonw.html

[R29] 定义函数
来源：http://hz.yj20258888.top/gtzdsvsscy.html


<!-- 参考信息 -->