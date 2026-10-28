代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.ywan-chungtsiang.top/gtpnfictwa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xingfuxueyuan.xyz/gtjdygpbys.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tanke756.top/gthifuohhw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.haohaochexian.top/gtserjujqy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daxiang520.top/gtlyodbmyj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yongpay.top/gthfjeceaw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenzaomai.com/gtpzosziva.html

Ruby: a == b
来源：http://hz.sxryk.cn/gtzhyicftw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuanzx.com/gtduqibcaz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shangyingyoupin.top/gttvmahwmk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jyoumei.cn/gtpwefiegh.html

PHP:  if (empty($x)) {}
来源：http://hz.jlsjyb.cn/gtghjssofh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gtykjylzey.html

TS:   if (x == null) {}
来源：http://hz.nwbrower.top/gttgaabvxx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daxiang520.top/gtinkkwpfb.html

Go:   if x == nil {}
来源：http://hz.yongpay.top/gtdghizpgu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.52xcode.cn/gtytkukvww.html

C#:   if (x is null) {}
来源：http://hz.yanxiufei.cn/gtezxrxnjw.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangkeji.top/gtiygfqkmm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hywenlv.cn/gtbpzwrgfz.html

PHP:  // 手写时间戳比较
来源：http://hz.fzhhl.top/gtsdraernq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.birdmap.top/gtzudhcmtp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtrxyvdfmi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gtpjashwiv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangshuangyany.cn/gthffspxxy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gaohongyu789.top/gtschxwhut.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangdashe.top/gtxvyuuiix.html

[P08] 处理浮点精度问题
来源：http://hz.guannengcc.top/gtgadosiro.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenzaomai.com/gtzxbjidaw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtatrbghry.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.c1oappe.top/gtbmxvcbnj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtqeehmqpb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtfzwstbyb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangdashe.top/gtajzdlwis.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtbgsnkoci.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgfzy.top/gtommeeiux.html

================================================================================
来源：http://hz.yuanzhike.top/gtcmzmqiyq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhongyouzk.top/gtzrqklpye.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxflytivm.html

[Q01] 创建表
来源：http://hz.ydzc1.top/gtavxufuwl.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtxlnmddxh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtmfioglvn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxuanxn.top/gtkflwnsif.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ybcxt.top/gtwcjhamob.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yvedp.cn/gtveqcmged.html

);
来源：http://hz.wangshuangyany.cn/gtjipnjfdp.html

[Q02] 创建带外键的表
来源：http://hz.shzxlz.cn/gtuwdpcotm.html

CREATE TABLE orders (
来源：http://hz.zhixingplan.top/gtrurwkniq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtgnedyknp.html

user_id INT NOT NULL,
来源：http://hz.yuanzhike.top/gtlvcmdzjb.html

amount DECIMAL(10, 2),
来源：http://hz.quarkkingdee.top/gtdfxudogs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cdnleiting.top/gtfdglsxuc.html

);
来源：http://hz.yuanzhike.top/gtohznjkyz.html

[Q03] 增加列
来源：http://hz.hysaishi.cn/gtuzfmdsqb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xziqi.cn/gtamldlalv.html

[Q04] 修改列类型
来源：http://hz.hfpthk.cn/gtaozahcww.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenlongwang.top/gttjczfpnb.html

[Q05] 重命名列
来源：http://hz.wangdashe.top/gtvmrbeqnv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guowangkeji.top/gtkkoyomtb.html

[Q06] 删除列
来源：http://hz.zhoulong.xyz/gtcitlsgjt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dianchejie.cn/gtuhwcxmxo.html

[Q07] 删除表
来源：http://hz.shangyingyoupin.top/gtmfdomzjb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guannengcc.top/gthaiyllts.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtnjkunlps.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yonumen.top/gttmfbcvvu.html

[Q09] 创建唯一索引
来源：http://hz.gotoacloud.top/gtlqkvribv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gzhubu.top/gtgkpykiae.html

[Q10] 插入单行
来源：http://hz.yonumen.top/gteaxtelpy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cheryme.top/gtohdiozwq.html

[Q11] 一次插入多行
来源：http://hz.pengpengdd.cyou/gtsysmepye.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yvedp.cn/gtrhwsuppn.html

[Q12] 插入后取自增 ID
来源：http://hz.yvedp.cn/gtvbvpjhmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.tianlin.xyz/gtjpwinmgt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtpnmyhfup.html

[Q13] 忽略重复插入
来源：http://hz.jinqigfzy.top/gtlfscdeno.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ydzc1.top/gthgwscgro.html

[Q14] 存在则更新（upsert）
来源：http://hz.pycfn.com/gtdkejsqgw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigufen.top/gtxjuvweox.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yvedp.cn/gtvytenoep.html

[Q15] 查询全部
来源：http://hz.guowangkeji.top/gtzmxjnvez.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtodvptvca.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtaohkeczi.html

SELECT id, name FROM users;
来源：http://hz.dianchejie.cn/gtzhhxpobp.html

[Q17] 条件查询
来源：http://hz.pengpengdd.cyou/gtjzrurzmo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.feifeiyinyue.top/gtetdmvuqy.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtxxbvfvej.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhoulong.xyz/gtrsofzbkl.html

[Q19] 范围查询
来源：http://hz.shangyingyoupin.top/gtmimpzszp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yvedp.cn/gtosrmnibg.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtxjnuvzqu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yanxiufei.cn/gtybcfnrvu.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtfllmpore.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xziqi.cn/gtfwhoghyn.html

[Q22] 排序
来源：http://hz.wangshuangyany.cn/gteaolfbri.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.iojbl.cn/gtcrwcrjeo.html

[Q23] 分页
来源：http://hz.sysykeji.top/gtaudymfuj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ywan-chungtsiang.top/gtupmoelub.html

[Q24] 去重
来源：http://hz.52xcode.cn/gtjwxoyjxv.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtautlyonj.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangkeji.top/gttrmfmrhy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtwsolknpu.html

[Q26] 计数
来源：http://hz.zhiwuduotai.top/gtteqnncod.html

SELECT COUNT(*) FROM users;
来源：http://hz.havefunace.top/gttcntoxtp.html

[Q27] 条件计数
来源：http://hz.yongpay.top/gtecciohaz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nwbrower.top/gtszmgqjgc.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangkeji.top/gtdmmlifwr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yvedp.cn/gtsmmvcxyk.html

[Q29] 最大最小值
来源：http://hz.guannengcc.top/gtzrjjyfok.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ydjk.org.cn/gtkpywrlmy.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtwqczliam.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gttafrpfog.html

[Q31] 分组后过滤
来源：http://hz.yj202588.top/gtltefgefp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhixingplan.top/gtepjrlbhr.html

[Q32] 分组拼接字符串
来源：http://hz.zhiwuduotai.top/gtmvqzwoso.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtmuhvveci.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtqtiuolks.html

[Q33] 多列分组
来源：http://hz.cheryme.top/gtzrjrjhxp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhoulong.xyz/gtvqsvadgd.html

[Q34] 每组取第一条
来源：http://hz.dianchejie.cn/gtrvfaxcwv.html

SELECT * FROM (
来源：http://hz.jyoumei.cn/gtqailwrzx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yonumen.top/gtdujqotix.html

) t WHERE rn = 1;
来源：http://hz.sweek.top/gtzpepcxvp.html

[Q35] 内连接
来源：http://hz.yj20258888.top/gtvgemjnxs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.meibo888.top/gtiqtcqpli.html

[Q36] 左连接
来源：http://hz.yanxiufei.cn/gtwtfpcwsi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtaciuohtm.html

[Q37] 右连接
来源：http://hz.yueranfly.top/gtbjwsxhrn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtaskndgfg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenjidiqi.icu/gtycdokhtk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yueranfly.top/gtnlbovrqc.html

[Q39] 自连接（查上下级）
来源：http://hz.hysaishi.cn/gtlhyokoau.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.quarkkingdee.top/gtahppssdp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.bjfxy.top/gtxpadjxko.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhiwuduotai.top/gtthiyjcdb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dashuyun.cn/gtgsjwlsea.html

[Q41] 多表连接
来源：http://hz.pengpengdd.cyou/gtbesrdayc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.bjfxy.top/gtlntuuiqu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnqzz.top/gtgefdwuil.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gzhubu.top/gtfmbotghm.html

[Q42] 连接条件附加过滤
来源：http://hz.cqqwz.cn/gtsagyqffz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tian-w.cn/gtfvshecua.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtoisqwsuo.html

[Q43] 标量子查询
来源：http://hz.cdnleiting.top/gtciordpyw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gtzuevnyaq.html

[Q44] IN 子查询
来源：http://hz.havefunace.top/gtdpgqxbun.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.quarkkingdee.top/gtogsgrfwm.html

[Q45] EXISTS 判断存在
来源：http://hz.hongshengwenyu.top/gtdkecinmh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.haohaochexian.top/gtwesyorse.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtwrqqcukh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtipvumdrk.html

[Q47] 与平均值比较
来源：http://hz.pengpengdd.cyou/gtitsxdvzi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtbpezboqj.html

[Q48] CTE 公用表表达式
来源：http://hz.redwolf501.top/gtftceuzff.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gtbtivoivv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenzaomai.com/gtwszmrxdh.html

[Q49] 更新单行
来源：http://hz.mhx1999.top/gtlrgboorf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtorpztcxc.html

[Q50] 批量更新
来源：http://hz.hywenlv.cn/gtgongpvuj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhixingplan.top/gtrcqdwrpn.html

[Q51] 用子查询更新
来源：http://hz.feifeiyinyue.top/gtjjuokmmt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.mhx1999.top/gtgqefgglv.html

[Q52] 删除指定行
来源：http://hz.chenlongwang.top/gteatrwuev.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtoufuudmz.html

[Q53] 按条件删除
来源：http://hz.ywan-chungtsiang.top/gtkonklefz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dianchejie.cn/gtgbfurxfd.html

[Q54] 清空表
来源：http://hz.cucudq.cn/gtzhlexnwz.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258888.top/gtidhpncmm.html

[Q55] 排名（并列占位）
来源：http://hz.hysaishi.cn/gtdjdxlcur.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ivvv.top/gtpdzlcalm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.meibo888.top/gtsbzydogy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hnxiangtu.top/gtvqkgdobx.html

[Q57] 行号
来源：http://hz.hywenlv.cn/gtlzgvlfeb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.52xcode.cn/gtcyromtca.html

[Q58] 累计求和
来源：http://hz.zhengqikj.top/gtbkdyghxl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigfzy.top/gtxpucoahf.html

[Q59] 分组内累计
来源：http://hz.hywenlv.cn/gtzsftviyi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jianghu66.top/gtilksinmv.html

[Q60] 取上一行 / 下一行
来源：http://hz.ehwqpu.com/gtootsmxtt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhijiandao.cn/gtktmgwpsj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhixingplan.top/gtugkljglc.html

[Q61] 移动平均
来源：http://hz.zhongyouzk.top/gtmzwucdii.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zycfv.cn/gtmwerlmqy.html

[Q62] 分组占比
来源：http://hz.yuanzhike.top/gtyetykqeq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtpspbsjvm.html

[Q63] 开启事务
来源：http://hz.snrcjt.cn/gtvttovmii.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinyuanbaomall.cn/gtlknhilfu.html

[Q64] 提交事务
来源：http://hz.jinghuilouyu.cn/gtgqmexywn.html

COMMIT;
来源：http://hz.andypj.xyz/gtjdxoluhd.html

[Q65] 回滚事务
来源：http://hz.svipenyu.cn/gtyhjguqbc.html

ROLLBACK;
来源：http://hz.shangyingyoupin.top/gtryycwbfe.html

[Q66] 行锁查询
来源：http://hz.ywan-chungtsiang.top/gtwcanldmn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jiagoushi.top/gtzskzcakw.html

[Q67] 设置隔离级别
来源：http://hz.haohaochexian.top/gtzwyteowv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gtjqmqjeku.html

[Q68] 保存点
来源：http://hz.9152youxi.cn/gtdximzdqe.html

SAVEPOINT sp1;
来源：http://hz.gaohongyu789.top/gtozizpehh.html

ROLLBACK TO sp1;
来源：http://hz.zdqjudy.top/gtftogonxy.html

[Q69] 查看执行计划
来源：http://hz.ydzc1.top/gtyrxxsguj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gtqjfpwovq.html

[Q70] 更新统计信息
来源：http://hz.ppjwa.cn/gtlwovxscd.html

ANALYZE TABLE users;
来源：http://hz.jianghu66.top/gtsuarbprz.html

[Q71] 查看建表语句
来源：http://hz.zhijiandao.cn/gtzfanptqh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gtknrrlheh.html

[Q72] 查看索引
来源：http://hz.sufxvd.cn/gtxlctdvcd.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gtihdetxal.html

[Q73] 查看表状态
来源：http://hz.haohaochexian.top/gtkdivxnhf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yongpay.top/gtzpcklgme.html

[Q74] 强制使用索引
来源：http://hz.chenzaomai.com/gtrznbkiaa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cashguo.top/gtyvjmkire.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gtttiqifmg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.meibo888.top/gtxltehpcq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sxryk.cn/gtztbjfbbx.html

[Q76] 按天统计
来源：http://hz.pycfn.com/gtcttgwxmb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnxiangtu.top/gtnsfpsjed.html

[Q77] 时间加减
来源：http://hz.yj202588.top/gtzabieztx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yueranfly.top/gtcltztjno.html

[Q78] 当前时间
来源：http://hz.yanxiufei.cn/gtfzzikykb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnxiangtu.top/gtgtpokxwj.html

[Q79] 字符串拼接
来源：http://hz.guowangkeji.top/gtoryvrdmh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgufenzy.top/gtgzzxqcho.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangkeji.top/gtjrfcsvph.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cdnleiting.top/gtaaywqeur.html

[Q81] 字符串替换
来源：http://hz.svipenyu.cn/gtrbjxtpmc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gtowjwaren.html

[Q82] 字符长度与字节长度
来源：http://hz.mhx1999.top/gtyanscfrq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.9152youxi.cn/gtbjcxxtrc.html

[Q83] 大小写转换
来源：http://hz.nanxuanxn.top/gtzdvoebuk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtnlumgykl.html

[Q84] 去除首尾空格
来源：http://hz.jqgufenzy.top/gtkbdxvlyy.html

SELECT TRIM(name) FROM users;
来源：http://hz.316326.xyz/gtmcrbjtdl.html

[Q85] 数值取整
来源：http://hz.cashguo.top/gtgioqepty.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gzhubu.top/gtglotrezn.html

[Q86] 读取 JSON 字段
来源：http://hz.yuanzhike.top/gtshwobdyy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yvedp.cn/gtnxwhqnkz.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtexvaxjaw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtrncnzaxi.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtlyvsxqbt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtgogjksqo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangkeji.top/gtpxmkxaxt.html

[Q89] 判断表是否存在
来源：http://hz.ywan-chungtsiang.top/gtyoutylhr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xziqi.cn/gtdgrrbiou.html

[Q90] 生成序号列
来源：http://hz.kuanghao11.cn/gtysjgfbfn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xziqi.cn/gtzrdzzbcm.html

================================================================================
来源：http://hz.snrcjt.cn/gtfyyshqbo.html

R. Bash 专题
来源：http://hz.nwbrower.top/gtmfvutjpi.html

================================================================================
来源：http://hz.jqgfzy.top/gtmuwzoajc.html

[R01] shebang 与严格模式
来源：http://hz.yj20258888.top/gtulathfuq.html

#!/usr/bin/env bash
来源：http://hz.zycfv.cn/gtpjcbmgda.html

set -euo pipefail
来源：http://hz.hnxiangtu.top/gtysjgmjoe.html

[R02] 变量赋值与使用
来源：http://hz.iojbl.cn/gtmzawwylf.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtqahpwjnc.html

[R03] 只读变量
来源：http://hz.xingfuxueyuan.xyz/gtrieuoxuu.html

readonly PI=3.14
来源：http://hz.svipenyu.cn/gtihcxeyln.html

[R04] 位置参数
来源：http://hz.hongshengwenyu.top/gtzcxjsput.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xziqi.cn/gtydrwlzkb.html

[R05] 参数默认值
来源：http://hz.quarkkingdee.top/gthjuxymzf.html

name="${1:-default}"
来源：http://hz.yuanzhike.top/gtzyobjhue.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangkeji.top/gtmdqgfpvm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.vqdsnc.cn/gtqpmtxmlx.html

[R07] if 判断文件
来源：http://hz.aibaodan.cn/gtujlefeuu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jlsjyb.cn/gtpzqlnvcy.html

[R08] 数值比较
来源：http://hz.yj202588.top/gtozvvxqls.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuxming.cn/gtroruqkby.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtedigcufc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pycfn.com/gtlcqlcfbc.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gtgdspgjrf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gtacwqjvps.html

[R11] case 多分支
来源：http://hz.hammf.cn/gtymsafthb.html

case "$1" in
来源：http://hz.kuanghao11.cn/gtjpjrqpbr.html

start) echo "启动" ;;
来源：http://hz.hnqzz.top/gtykubscqk.html

stop)  echo "停止" ;;
来源：http://hz.jinghuilouyu.cn/gtpywmvkht.html

*)     echo "未知命令" ;;
来源：http://hz.birdmap.top/gtzxknsktb.html

esac
来源：http://hz.jinqigfzy.top/gtphhkcfli.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtjglrdbnr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yueranfly.top/gtbjgnyyms.html

[R13] for 计数循环
来源：http://hz.dashuyun.cn/gtmgzobanh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fzhhl.top/gtrhfhshnw.html

[R14] C 风格 for
来源：http://hz.zhixingplan.top/gtlkpuntsb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.guowangkeji.top/gtdwdbzfex.html

[R15] while 逐行读文件
来源：http://hz.meibo888.top/gtznwhphft.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydzc1.top/gtiwpxjkob.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtfrrriawf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydzc1.top/gtvvifwstz.html

[R17] 数组定义与取值
来源：http://hz.sxryk.cn/gtsoooskrb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtbbpilebl.html

[R18] 遍历数组
来源：http://hz.jlsjyb.cn/gtfscggnyq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gtzsvtvpip.html

[R19] 数组长度
来源：http://hz.tian-w.cn/gtideoawkr.html

echo "${#arr[@]}"
来源：http://hz.jqgfzy.top/gtcfoxkody.html

[R20] 关联数组（字典）
来源：http://hz.chenjidiqi.icu/gtdtovhltb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.andypj.xyz/gtglyiiskx.html

[R21] 字符串长度
来源：http://hz.gogol.net.cn/gtrexecbzq.html

echo "${#s}"
来源：http://hz.tian-w.cn/gtdbuehhhc.html

[R22] 截取子串
来源：http://hz.jinghuilouyu.cn/gtdglfvrhf.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtyqyhlvme.html

[R23] 字符串替换
来源：http://hz.havefunace.top/gtpudbbaks.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.svipenyu.cn/gtabvnlrtw.html

[R24] 大小写转换
来源：http://hz.sweek.top/gtoxthoilg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenlongwang.top/gtpyfzqkwi.html

[R25] 去后缀 / 去前缀
来源：http://hz.snrcjt.cn/gtzpsspoxy.html


<!-- 参考信息 -->