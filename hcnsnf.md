代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.iojbl.cn/gthgzfayjo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gtknuaztbx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtwrwwblkc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtmqbtoeon.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sxryk.cn/gtlwxvpwfi.html

Go:   len(arr);  len(m)
来源：http://hz.pengpengdd.cyou/gtbzajener.html

Ruby: x.length;  x.size
来源：http://hz.nwbrower.top/gtdlspsudh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xylfe.cn/gtcjtpdypq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gthqjbncks.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangshuangyany.cn/gtbvbnyorr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigufen.top/gtiuvldtbq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgfzy.top/gtzrxrldlb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangdashe.top/gtowhbwovm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.svipenyu.cn/gtdivikrwv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tanke756.top/gtflkfcoqz.html

Ruby: a == b
来源：http://hz.snrcjt.cn/gtxfavldvm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangtech.top/gtylrzwhdg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.guowangkeji.top/gtosxsqsiv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hywenlv.cn/gtmmdrxcbr.html

PHP:  if (empty($x)) {}
来源：http://hz.chenzaomai.com/gtwndsefsd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cucudq.cn/gtkttmzuvv.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtsuocncif.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yongpay.top/gtxaybreyl.html

Go:   if x == nil {}
来源：http://hz.cqqwz.cn/gtqusgdugy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xylfe.cn/gtpptthvnn.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangtech.top/gttjpkxyce.html

[P07] 防抖与节流
来源：http://hz.sufxvd.cn/gtowlueseg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shangyingyoupin.top/gtzmjcwzjb.html

PHP:  // 手写时间戳比较
来源：http://hz.ybcxt.top/gtqkomjsfe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtibeggntu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtajdpazbd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangdashe.top/gtbrdpvbyb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.iojbl.cn/gtusytencn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sxryk.cn/gtjpostuna.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.meibo888.top/gtzfovqmph.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtnulwgdrp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daxiang520.top/gtvtzbbbri.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigfzy.top/gtvfxebhdf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtjbintfev.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtkcefsdvn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cqqwz.cn/gtcacueioh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.9152youxi.cn/gtpalbslrc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtdzddpgeu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sweek.top/gtemshyqsm.html

================================================================================
来源：http://hz.hfpthk.cn/gtvdysqlfi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.birdmap.top/gtyvdsftds.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gthrzggfej.html

[Q01] 创建表
来源：http://hz.guowangkeji.top/gtzbakaqry.html

CREATE TABLE users (
来源：http://hz.shzxlz.cn/gtztmmging.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.bjfxy.top/gtnxghuird.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gttrbbhixs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guannengcc.top/gtwrmfokhn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sufxvd.cn/gtqwckxdrv.html

);
来源：http://hz.yj202588.top/gtwfkizppm.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtbviqgswd.html

CREATE TABLE orders (
来源：http://hz.tanke756.top/gtrutjfwov.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinghuilouyu.cn/gtymtlsomx.html

user_id INT NOT NULL,
来源：http://hz.zhoulong.xyz/gtgvplpaws.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtwcdpmzua.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuetiantiany.cn/gtfnlamsbn.html

);
来源：http://hz.haohaochexian.top/gtzfxtexuv.html

[Q03] 增加列
来源：http://hz.jinqigfzy.top/gtophmlmia.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hongshengwenyu.top/gteivjbnue.html

[Q04] 修改列类型
来源：http://hz.zhaomingkeji.xyz/gtwbsptezr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtzdwqjnlj.html

[Q05] 重命名列
来源：http://hz.gotoacloud.top/gtoseobqtf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hammf.cn/gtbmuebkgm.html

[Q06] 删除列
来源：http://hz.daxiang520.top/gtkfhvgren.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aizwys.cn/gtcfykukuy.html

[Q07] 删除表
来源：http://hz.jinghuilouyu.cn/gtqhhllmvp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gaohongyu789.top/gtiokzzzfa.html

[Q08] 创建普通索引
来源：http://hz.shzxlz.cn/gtkxdsqmxk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhongyouzk.top/gtgafozcwi.html

[Q09] 创建唯一索引
来源：http://hz.andypj.xyz/gtmpjdjihk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jiagoushi.top/gtstmuuygi.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtyvreqoad.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.kuanghao11.cn/gtmpcaqhqw.html

[Q11] 一次插入多行
来源：http://hz.xinyue.icu/gtglvfbghy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yanxiufei.cn/gtbjgvnkqg.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gtnolmpvnf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.c1oappe.top/gtrembrgty.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yongpay.top/gtbimxicuf.html

[Q13] 忽略重复插入
来源：http://hz.nanxinkj.top/gtqufolgmd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gtktyqwxwo.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuxming.cn/gttumqxadu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.smart0.xyz/gtnasikxle.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinghuilouyu.cn/gtosjqmovv.html

[Q15] 查询全部
来源：http://hz.aizwys.cn/gtbtbkexjc.html

SELECT * FROM users;
来源：http://hz.zhengqikj.top/gtyrotifhu.html

[Q16] 查询指定列
来源：http://hz.yuanzhike.top/gtvuwzaxzk.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtzswalywp.html

[Q17] 条件查询
来源：http://hz.zdqjudy.top/gtyyzwjwnm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.feifeiyinyue.top/gtmfpmufly.html

[Q18] 模糊匹配
来源：http://hz.hammf.cn/gttmdzqyph.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangkeji.top/gtasvqklwn.html

[Q19] 范围查询
来源：http://hz.gzhubu.top/gtruurnlum.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gttgucmypt.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtzdojjmcr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj202588.top/gtvwltxrpy.html

[Q21] 空值判断
来源：http://hz.jinqigufen.top/gtztpouszl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gttaubfjat.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtptkdoqeb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtshgcuiho.html

[Q23] 分页
来源：http://hz.0kj1m.cn/gtnxdleicu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.mhx1999.top/gtjqewchpd.html

[Q24] 去重
来源：http://hz.gaohongyu789.top/gtykrrfvjm.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangdashe.top/gtvehwaewp.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangkeji.top/gtnzlyrijr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuanzx.com/gthmdweeup.html

[Q26] 计数
来源：http://hz.yueranfly.top/gtfbsmgazw.html

SELECT COUNT(*) FROM users;
来源：http://hz.guannengcc.top/gtqsintanx.html

[Q27] 条件计数
来源：http://hz.sxryk.cn/gtiswcqulz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtgitikuxm.html

[Q28] 求和与平均
来源：http://hz.shangyingyoupin.top/gtvpyboist.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gtljigowml.html

[Q29] 最大最小值
来源：http://hz.snrcjt.cn/gtolhlzqzu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgfzy.top/gtstwlknet.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtnmlpvdor.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtlpeeryta.html

[Q31] 分组后过滤
来源：http://hz.fengsongda.top/gtdfigyygz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yueranfly.top/gtgrczusty.html

[Q32] 分组拼接字符串
来源：http://hz.sxryk.cn/gthyrkdfkd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtevwhbvrw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtmapetiiy.html

[Q33] 多列分组
来源：http://hz.zhixingplan.top/gtspxrowqt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258888.top/gtedwproot.html

[Q34] 每组取第一条
来源：http://hz.yj20258888.top/gtasaxgllf.html

SELECT * FROM (
来源：http://hz.hongshengwenyu.top/gttxtjgvyj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cdnleiting.top/gtbspavwjh.html

) t WHERE rn = 1;
来源：http://hz.guannengcc.top/gthesqnvxh.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtvcfzftkm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtlcmdkrcp.html

[Q36] 左连接
来源：http://hz.guannengcc.top/gttububwvl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtxodfsmul.html

[Q37] 右连接
来源：http://hz.xuanzx.com/gtvgtnrupn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hongshengwenyu.top/gtufqyyuqn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhaomingkeji.xyz/gtasmwqvfw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shzxlz.cn/gtummggvmc.html

[Q39] 自连接（查上下级）
来源：http://hz.hnxiangtu.top/gtagcbtupb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ivvv.top/gtvvzpwouz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangtech.top/gtmbolqxxs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cheryme.top/gtuhrjtksz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.quarkkingdee.top/gthmtjfmqv.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtflokwzhd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtnxgaiqjy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258.top/gtfwohygsv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.svipenyu.cn/gtkusssjeg.html

[Q42] 连接条件附加过滤
来源：http://hz.wangdashe.top/gtwvyrsnpt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenlongwang.top/gtycfkximz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sxryk.cn/gtvgeidfai.html

[Q43] 标量子查询
来源：http://hz.fzhhl.top/gtkgoesdwv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.smart0.xyz/gtlyxfqizp.html

[Q44] IN 子查询
来源：http://hz.andypj.xyz/gtowbckoom.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dashuyun.cn/gtmdtqulcw.html

[Q45] EXISTS 判断存在
来源：http://hz.jinyuanbaomall.cn/gtodchcyst.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtglrraftg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dianchejie.cn/gtzlaqrudw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtmueiomrk.html

[Q47] 与平均值比较
来源：http://hz.andypj.xyz/gtriwadsny.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.snrcjt.cn/gtlvxytwvu.html

[Q48] CTE 公用表表达式
来源：http://hz.xingfuxueyuan.xyz/gtfhvxjkmm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ybcxt.top/gtvhjcrota.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.c1oappe.top/gtjxqxlvpb.html

[Q49] 更新单行
来源：http://hz.xingfuxueyuan.xyz/gtxbrrqfyv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gttwswdfdy.html

[Q50] 批量更新
来源：http://hz.cdnleiting.top/gtwmnvjcom.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shzxlz.cn/gtudeuorcn.html

[Q51] 用子查询更新
来源：http://hz.nanxuanxn.top/gtscptvrzi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cqqwz.cn/gtapdrpcci.html

[Q52] 删除指定行
来源：http://hz.jinqigufen.top/gttmojaenc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tianlin.xyz/gtjtmhspyw.html

[Q53] 按条件删除
来源：http://hz.ydzc1.top/gtxadrcspr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangtech.top/gtiiktfbvc.html

[Q54] 清空表
来源：http://hz.snrcjt.cn/gtgskvhaav.html

TRUNCATE TABLE logs;
来源：http://hz.sweek.top/gtbxmitwoi.html

[Q55] 排名（并列占位）
来源：http://hz.nanxuanxn.top/gtanyodccs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuxming.cn/gtblajyxmc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xingfuxueyuan.xyz/gtuuwwzgkg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtqeahzslx.html

[Q57] 行号
来源：http://hz.fengsongda.top/gtohmxrvpx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenjidiqi.icu/gtdrmhkvna.html

[Q58] 累计求和
来源：http://hz.meibo888.top/gtgqckrnyo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.52xcode.cn/gthohdndcg.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtukavdwhh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hfpthk.cn/gttutkomxx.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtosmlxkem.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.snrcjt.cn/gtakpavlwz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yonumen.top/gtxdogjtce.html

[Q61] 移动平均
来源：http://hz.yonumen.top/gteaqfurqg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.andypj.xyz/gteauudcvh.html

[Q62] 分组占比
来源：http://hz.zhixingplan.top/gtbyzetqov.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtkjghhwqs.html

[Q63] 开启事务
来源：http://hz.jinghuilouyu.cn/gttumdcdro.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenlongwang.top/gtizvnavmn.html

[Q64] 提交事务
来源：http://hz.ivvv.top/gtbylroory.html

COMMIT;
来源：http://hz.yj202588.top/gtfjbhhlha.html

[Q65] 回滚事务
来源：http://hz.snrcjt.cn/gtznbyvyef.html

ROLLBACK;
来源：http://hz.sxryk.cn/gtdrjlraid.html

[Q66] 行锁查询
来源：http://hz.ybcxt.top/gtnclahlxp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.iojbl.cn/gtclgllxwr.html

[Q67] 设置隔离级别
来源：http://hz.jqgfzy.top/gtvovpghxa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gtyelmrtwp.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtqatxnfzi.html

SAVEPOINT sp1;
来源：http://hz.zdqjudy.top/gtukrawunk.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gttvwzjbpb.html

[Q69] 查看执行计划
来源：http://hz.aizwys.cn/gtyhhwraab.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hysaishi.cn/gtqgpszozy.html

[Q70] 更新统计信息
来源：http://hz.birdmap.top/gtoozoczqf.html

ANALYZE TABLE users;
来源：http://hz.zhengqikj.top/gtxyhswtqu.html

[Q71] 查看建表语句
来源：http://hz.yangfankeji.com/gtwqqnefkn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.quarkkingdee.top/gtukoegial.html

[Q72] 查看索引
来源：http://hz.yvedp.cn/gtoenocrch.html

SHOW INDEX FROM users;
来源：http://hz.yvedp.cn/gtmwkypjps.html

[Q73] 查看表状态
来源：http://hz.cqqwz.cn/gtvsbocnum.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gaohongyu789.top/gtjclzlqck.html

[Q74] 强制使用索引
来源：http://hz.meibo888.top/gtzacycxzx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinyuanbaomall.cn/gtjbjnleus.html

[Q75] 日期格式化
来源：http://hz.ydjk.org.cn/gtdullurgd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhixingplan.top/gtismyhxzy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtdpdznzxc.html

[Q76] 按天统计
来源：http://hz.xziqi.cn/gtnkwnybbh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cdnleiting.top/gtvbjjyaoh.html

[Q77] 时间加减
来源：http://hz.aibaodan.cn/gtetpplvmy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtnvjxpkxy.html

[Q78] 当前时间
来源：http://hz.hammf.cn/gtellzncbf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daria6918.cn/gtciroggpi.html

[Q79] 字符串拼接
来源：http://hz.c1oappe.top/gtblsgeovo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jianghu66.top/gtppzmxsgz.html

[Q80] 字符串截取
来源：http://hz.yueranfly.top/gtbacbvngv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenlongwang.top/gtfexuqrzl.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtflgyoytb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangtech.top/gtwnyxiyyi.html

[Q82] 字符长度与字节长度
来源：http://hz.mhx1999.top/gtthtrmecg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangdashe.top/gtfdawwzxc.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtlnmmontb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtqwczbhyl.html

[Q84] 去除首尾空格
来源：http://hz.zycfv.cn/gthftxtexj.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnxiangtu.top/gtbhobhqhj.html

[Q85] 数值取整
来源：http://hz.tanke756.top/gtxwosyzfs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guowangkeji.top/gthsqdmifm.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxinkj.top/gthdnvgijp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cashguo.top/gtqfrymhmu.html

[Q87] JSON 字段做条件
来源：http://hz.ydzc1.top/gtkhipgjmo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daxiang520.top/gtojxqsztv.html

[Q88] 行转列（条件聚合）
来源：http://hz.sysykeji.top/gtywzaxsnn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zycfv.cn/gtxsomtukg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shangyingyoupin.top/gthmotlzfk.html

[Q89] 判断表是否存在
来源：http://hz.hammf.cn/gtsrotgoze.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shangyingyoupin.top/gtjmagjplx.html

[Q90] 生成序号列
来源：http://hz.daria6918.cn/gtifymwkhq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fengsongda.top/gtwrmmzpcl.html

================================================================================
来源：http://hz.zdqjudy.top/gtxjqllfqu.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtoaovjgej.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtiqzagosx.html

[R01] shebang 与严格模式
来源：http://hz.ydzc1.top/gttgmsjrtu.html

#!/usr/bin/env bash
来源：http://hz.zhongyouzk.top/gttxwdkiij.html

set -euo pipefail
来源：http://hz.snrcjt.cn/gtrgwbgnpy.html

[R02] 变量赋值与使用
来源：http://hz.jinyuanbaomall.cn/gtbfgatohc.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gtnhjrzzxw.html

[R03] 只读变量
来源：http://hz.yonumen.top/gtixicgrar.html

readonly PI=3.14
来源：http://hz.jqgfzy.top/gtetpwayns.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gthuwfhrzn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cashguo.top/gtjyjiczkg.html

[R05] 参数默认值
来源：http://hz.mhx1999.top/gtxbsuycdm.html

name="${1:-default}"
来源：http://hz.zhengqikj.top/gtzeiiiylz.html

[R06] 判断命令是否存在
来源：http://hz.hammf.cn/gtfhhbnoos.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jlsjyb.cn/gtmvpoiprm.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gteybeafxd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtotixsotj.html

[R08] 数值比较
来源：http://hz.sufxvd.cn/gtijkynkai.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydjk.org.cn/gtfukwuoqm.html

[R09] 字符串比较
来源：http://hz.yonumen.top/gtxnxkcooy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.c1oappe.top/gtfreekjpf.html

[R10] 正则匹配
来源：http://hz.jinqigfzy.top/gttrfwpook.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtirgzxjky.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtgexnyhhk.html

case "$1" in
来源：http://hz.wangdashe.top/gtgoffgmte.html

start) echo "启动" ;;
来源：http://hz.yanxiufei.cn/gtozzrezve.html

stop)  echo "停止" ;;
来源：http://hz.haohaochexian.top/gtmusrajsi.html

*)     echo "未知命令" ;;
来源：http://hz.hammf.cn/gtqwpkrhjp.html

esac
来源：http://hz.jiagoushi.top/gtefloxlcj.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gthgjomloe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj202588.top/gtiuqapzwo.html

[R13] for 计数循环
来源：http://hz.hammf.cn/gthrkjidcr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.meibo888.top/gtfscrgaeu.html

[R14] C 风格 for
来源：http://hz.shuidangran.top/gtjfcamlwn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ybcxt.top/gtuxekoofk.html

[R15] while 逐行读文件
来源：http://hz.vqdsnc.cn/gtltmhbafk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhengqikj.top/gtvbpdpayt.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtygitmwoi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hywenlv.cn/gtyjhnfphi.html

[R17] 数组定义与取值
来源：http://hz.vqdsnc.cn/gtboqbfwzb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhiwuduotai.top/gtkbhppows.html

[R18] 遍历数组
来源：http://hz.havefunace.top/gtlqotxqra.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hongshengwenyu.top/gtjtinrspv.html

[R19] 数组长度
来源：http://hz.havefunace.top/gtzbnkzyjj.html

echo "${#arr[@]}"
来源：http://hz.cdnleiting.top/gtupyevlzk.html

[R20] 关联数组（字典）
来源：http://hz.gotoacloud.top/gtlvcyohoh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.chenlongwang.top/gtjblzoxyq.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtdfcjolkz.html


<!-- 参考信息 -->