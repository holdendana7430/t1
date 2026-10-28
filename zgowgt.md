代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hz.tian-w.cn/gtpcqbeelo.html

Go:   len(arr);  len(m)
来源：http://hz.feifeiyinyue.top/gtqwrhodfp.html

Ruby: x.length;  x.size
来源：http://hz.shangyingyoupin.top/gtfzmoxbbj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pycfn.com/gtgdbzmgnl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jiagoushi.top/gtubfkqgyz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhaomingkeji.xyz/gtevsxjpme.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.mhx1999.top/gtkjdvjaos.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangkeji.top/gtfsvjlatm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gtcylnehbh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hywenlv.cn/gtprvrcfak.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.meibo888.top/gtrxcviiuq.html

Ruby: a == b
来源：http://hz.dianchejie.cn/gtenrpoiqn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tanke756.top/gtafztejwv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhixingplan.top/gtplkuttaz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.svipenyu.cn/gtaerxhbfa.html

PHP:  if (empty($x)) {}
来源：http://hz.ywan-chungtsiang.top/gtgzegqnea.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nwbrower.top/gtskpaeanl.html

TS:   if (x == null) {}
来源：http://hz.zhiwuduotai.top/gtrpfsmivg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cucudq.cn/gthnodfwqr.html

Go:   if x == nil {}
来源：http://hz.nanxinkj.top/gtarjgfhli.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnxiangtu.top/gtswpwtnnk.html

C#:   if (x is null) {}
来源：http://hz.meibo888.top/gtduafjrgh.html

[P07] 防抖与节流
来源：http://hz.xziqi.cn/gtvzqehlrt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtsllcceqi.html

PHP:  // 手写时间戳比较
来源：http://hz.9152youxi.cn/gtjgglbslg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtvtqnrnxt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jiagoushi.top/gtusrdaadd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhixingplan.top/gtnaqicjik.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnxiangtu.top/gttuxntsfm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shzxlz.cn/gtjscvejmu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangkeji.top/gtpqvgklcl.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtsmrmjfbn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gttuhmazwk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.snrcjt.cn/gtpbgfvlji.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pengpengdd.cyou/gtjkwpforu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.haohaochexian.top/gtxjwktgnd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.redwolf501.top/gtckfgxwxx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jianghu66.top/gtzypvoedj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nwbrower.top/gtcjkfkouq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ydjk.org.cn/gtcwwbaduo.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtdnpbbozx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gtgmaagykf.html

================================================================================
来源：http://hz.smart0.xyz/gtxmifuhnw.html

[Q01] 创建表
来源：http://hz.aizwys.cn/gtimtjymnh.html

CREATE TABLE users (
来源：http://hz.gotoacloud.top/gtienfsrrx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtqrljirbf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangdashe.top/gtbxqhwweu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.daxiang520.top/gtazkozpzu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhongyouzk.top/gtvosygzue.html

);
来源：http://hz.shzxlz.cn/gtosenrzvc.html

[Q02] 创建带外键的表
来源：http://hz.redwolf501.top/gtnpxnpjuj.html

CREATE TABLE orders (
来源：http://hz.pengpengdd.cyou/gtkxxbfmim.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.c1oappe.top/gtzmluwhcs.html

user_id INT NOT NULL,
来源：http://hz.daxiang520.top/gtxzdrllwx.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gtcjsfpdld.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenzaomai.com/gtmusjjwta.html

);
来源：http://hz.jlsjyb.cn/gtekuzbmxh.html

[Q03] 增加列
来源：http://hz.yj20258888.top/gtgecmytxo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.0kj1m.cn/gthxwmnvon.html

[Q04] 修改列类型
来源：http://hz.yanxiufei.cn/gtkdikdcbp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gaohongyu789.top/gthcfbidwj.html

[Q05] 重命名列
来源：http://hz.ppjwa.cn/gttzkwyqlf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgufenzy.top/gtzyttgtdr.html

[Q06] 删除列
来源：http://hz.ivvv.top/gttvunpfrq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jianghu66.top/gtihpwawzj.html

[Q07] 删除表
来源：http://hz.xingfuxueyuan.xyz/gtyqdpnsvx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hysaishi.cn/gtcguqeubb.html

[Q08] 创建普通索引
来源：http://hz.shanyushiyangtech.top/gtyuvhoabf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtceweiegr.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtroaqefix.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtbnswkwhq.html

[Q10] 插入单行
来源：http://hz.jqgufenzy.top/gtjllxwxak.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangtech.top/gtmbwqfgpu.html

[Q11] 一次插入多行
来源：http://hz.tanke756.top/gtvsbbzbsd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangkeji.top/gtziqujmng.html

[Q12] 插入后取自增 ID
来源：http://hz.shangyingyoupin.top/gtlkspcnbj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtgaxohptn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.andypj.xyz/gtbazxvcoo.html

[Q13] 忽略重复插入
来源：http://hz.xylfe.cn/gtfkrwvyxv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pengpengdd.cyou/gtoyxjdnhr.html

[Q14] 存在则更新（upsert）
来源：http://hz.zdqjudy.top/gtwqfudiyz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guowangkeji.top/gtxobtnksd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tianlin.xyz/gtoogeihmf.html

[Q15] 查询全部
来源：http://hz.yongpay.top/gtewcvtlzt.html

SELECT * FROM users;
来源：http://hz.quarkkingdee.top/gtsekcyevv.html

[Q16] 查询指定列
来源：http://hz.zhaomingkeji.xyz/gtkgzxfbgo.html

SELECT id, name FROM users;
来源：http://hz.smart0.xyz/gttuxwhdhw.html

[Q17] 条件查询
来源：http://hz.xuanzx.com/gtjhximvyl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.birdmap.top/gturtoiwmx.html

[Q18] 模糊匹配
来源：http://hz.quarkkingdee.top/gtjnpjujsx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tanke756.top/gtefhtvzpd.html

[Q19] 范围查询
来源：http://hz.zhijiandao.cn/gtfxpwwwwu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tanke756.top/gtlqrcqair.html

[Q20] IN 列表
来源：http://hz.yangfankeji.com/gtndjjhony.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.52xcode.cn/gtohkujiff.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtjosrlmqw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yueranfly.top/gthcyzedxp.html

[Q22] 排序
来源：http://hz.316326.xyz/gtlwzmfffi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258.top/gtnekmwoiu.html

[Q23] 分页
来源：http://hz.meibo888.top/gtygbroksg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtrvpqwhtc.html

[Q24] 去重
来源：http://hz.dianchejie.cn/gtfatrikkm.html

SELECT DISTINCT city FROM users;
来源：http://hz.yonumen.top/gtudmpauko.html

[Q25] 只取前 N 条
来源：http://hz.daria6918.cn/gtbmjzplcq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yueranfly.top/gtcxokujay.html

[Q26] 计数
来源：http://hz.xziqi.cn/gtgqakknew.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangdashe.top/gtrhxszspg.html

[Q27] 条件计数
来源：http://hz.guannengcc.top/gtlpcywegr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sufxvd.cn/gtopiahoiv.html

[Q28] 求和与平均
来源：http://hz.pycfn.com/gtkdajcpdu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gtrbqfbjfh.html

[Q29] 最大最小值
来源：http://hz.tianlin.xyz/gtbjiettmn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangshuangyany.cn/gtbnxctokq.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtzucerefa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtokzaohat.html

[Q31] 分组后过滤
来源：http://hz.52xcode.cn/gtxhuwfguy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gtuepprvbp.html

[Q32] 分组拼接字符串
来源：http://hz.yuxming.cn/gtpoejpgxi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtbailyrsr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.mhx1999.top/gtzhsmtttg.html

[Q33] 多列分组
来源：http://hz.jiagoushi.top/gtijcjkfhr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sweek.top/gtkguwmjfa.html

[Q34] 每组取第一条
来源：http://hz.yj202588.top/gtfsbaoxpa.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gtlhkqjkah.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gtgohkilbl.html

) t WHERE rn = 1;
来源：http://hz.daria6918.cn/gtlmyaqnrm.html

[Q35] 内连接
来源：http://hz.c1oappe.top/gtaysbelyt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtyluvclea.html

[Q36] 左连接
来源：http://hz.ivvv.top/gtkxltlfpf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gtsfvfxnoy.html

[Q37] 右连接
来源：http://hz.vqdsnc.cn/gtknlsmied.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.iojbl.cn/gtjlwdskjt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pycfn.com/gtzcynuvfi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigufen.top/gtsbbbmkwt.html

[Q39] 自连接（查上下级）
来源：http://hz.jianghu66.top/gtnufjlvdt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigufen.top/gtiutovnik.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zycfv.cn/gtujivgxlq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.c1oappe.top/gtnhnkgqvp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxinkj.top/gtmbhrqbsj.html

[Q41] 多表连接
来源：http://hz.jqgufenzy.top/gtkohpzpre.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zycfv.cn/gtyybcuudi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cdnleiting.top/gtgwjcotrt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xingfuxueyuan.xyz/gtunczooah.html

[Q42] 连接条件附加过滤
来源：http://hz.c1oappe.top/gtwisypquk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ivvv.top/gtphpcgadm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daxiang520.top/gtgjkhwygl.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtqcfrgsuj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zycfv.cn/gtydddzxcx.html

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtipimphpw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gaohongyu789.top/gtatexgelg.html

[Q45] EXISTS 判断存在
来源：http://hz.yvedp.cn/gtzozkmnoi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtolqbcdbe.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangtech.top/gtsvicusfv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtksidjvod.html

[Q47] 与平均值比较
来源：http://hz.xuanzx.com/gtffnuxoao.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shuidangran.top/gtpbzhfmgw.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gthqjwpiwn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zycfv.cn/gtlleqlirq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tanke756.top/gtuwxkxffj.html

[Q49] 更新单行
来源：http://hz.ywan-chungtsiang.top/gtnfctqvyu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtgzlfgznn.html

[Q50] 批量更新
来源：http://hz.shanyushiyangtech.top/gtgxiqcgpp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jianghu66.top/gtzbtdclgt.html

[Q51] 用子查询更新
来源：http://hz.jinyuanbaomall.cn/gtjwcmsukp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnqzz.top/gtsymiekqm.html

[Q52] 删除指定行
来源：http://hz.nanxuanxn.top/gthskcrdod.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtltrpfkkd.html

[Q53] 按条件删除
来源：http://hz.smart0.xyz/gtqassogkl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.mhx1999.top/gtfkssncon.html

[Q54] 清空表
来源：http://hz.quarkkingdee.top/gtcscczaht.html

TRUNCATE TABLE logs;
来源：http://hz.tanke756.top/gtcyadliiz.html

[Q55] 排名（并列占位）
来源：http://hz.hnxiangtu.top/gtulrcufid.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gtgqxvsgtd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydjk.org.cn/gtokewdxuz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xziqi.cn/gtchaldmhu.html

[Q57] 行号
来源：http://hz.hammf.cn/gtyfnrshkp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtrfojdnwv.html

[Q58] 累计求和
来源：http://hz.yonumen.top/gtrgsyqhdt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hongshengwenyu.top/gtjuzgvrjo.html

[Q59] 分组内累计
来源：http://hz.zhijiandao.cn/gtcrgggyfe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.birdmap.top/gtkkioirvc.html

[Q60] 取上一行 / 下一行
来源：http://hz.quarkkingdee.top/gtgyothjhq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.vqdsnc.cn/gtfmeaqzjj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shuidangran.top/gtfkfrttgq.html

[Q61] 移动平均
来源：http://hz.xinyue.icu/gtbkjmtjro.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenzaomai.com/gtcrdijzvk.html

[Q62] 分组占比
来源：http://hz.shzxlz.cn/gtimpbdifs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtcadsgoyo.html

[Q63] 开启事务
来源：http://hz.dashuyun.cn/gtcfnidwib.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenjidiqi.icu/gtosnwxvok.html

[Q64] 提交事务
来源：http://hz.zhoulong.xyz/gtynlwzxvt.html

COMMIT;
来源：http://hz.gzhubu.top/gtkwlpsrcc.html

[Q65] 回滚事务
来源：http://hz.jianghu66.top/gtqdaakzzn.html

ROLLBACK;
来源：http://hz.daxiang520.top/gtdwcgpapt.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtwwticifs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258888.top/gthwhdthdd.html

[Q67] 设置隔离级别
来源：http://hz.havefunace.top/gtrnydwqth.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yueranfly.top/gtvayupcum.html

[Q68] 保存点
来源：http://hz.daria6918.cn/gtdmdzzzek.html

SAVEPOINT sp1;
来源：http://hz.yj20258.top/gtyzlfsnus.html

ROLLBACK TO sp1;
来源：http://hz.havefunace.top/gtzwqhvfhx.html

[Q69] 查看执行计划
来源：http://hz.jinqigufen.top/gtxyxvvsre.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.0kj1m.cn/gtahwfnwvh.html

[Q70] 更新统计信息
来源：http://hz.bjfxy.top/gtuaqjbuce.html

ANALYZE TABLE users;
来源：http://hz.chenzaomai.com/gtxmioneiw.html

[Q71] 查看建表语句
来源：http://hz.ydzc1.top/gtyvjcayop.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hfpthk.cn/gtnksrpbxu.html

[Q72] 查看索引
来源：http://hz.yuanzhike.top/gtirgkbjff.html

SHOW INDEX FROM users;
来源：http://hz.yj20258.top/gtpmodhxps.html

[Q73] 查看表状态
来源：http://hz.ydzc1.top/gtfxofhchh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.aibaodan.cn/gtrnjbzxlq.html

[Q74] 强制使用索引
来源：http://hz.ivvv.top/gtyqqhbkmt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hysaishi.cn/gtfpxvqmyr.html

[Q75] 日期格式化
来源：http://hz.vqdsnc.cn/gtyovddzly.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.feifeiyinyue.top/gtvnztbrmi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gtdwprucub.html

[Q76] 按天统计
来源：http://hz.nwbrower.top/gthxtaegir.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ppjwa.cn/gtqypmzofy.html

[Q77] 时间加减
来源：http://hz.fengsongda.top/gtavimqbjf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gogol.net.cn/gtxlzpbnnq.html

[Q78] 当前时间
来源：http://hz.zhixingplan.top/gtrpsnqbcj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zycfv.cn/gtcfpyutvt.html

[Q79] 字符串拼接
来源：http://hz.chenjidiqi.icu/gtayvkfmih.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnqzz.top/gtbtutudvx.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtgtluqsid.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zdqjudy.top/gtkrcddikf.html

[Q81] 字符串替换
来源：http://hz.yanxiufei.cn/gthdixmitv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jlsjyb.cn/gtpzbsgjts.html

[Q82] 字符长度与字节长度
来源：http://hz.yonumen.top/gtbhfkmwvl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.svipenyu.cn/gtkizvwkqk.html

[Q83] 大小写转换
来源：http://hz.ehwqpu.com/gtzzecxmot.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.iojbl.cn/gtxqldfuue.html

[Q84] 去除首尾空格
来源：http://hz.jinqigufen.top/gthrhukyoy.html

SELECT TRIM(name) FROM users;
来源：http://hz.guannengcc.top/gtnrszxjwt.html

[Q85] 数值取整
来源：http://hz.ppjwa.cn/gtboamnkrs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.vqdsnc.cn/gtxckmuhvi.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtfvwyhirw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgufenzy.top/gtwmdedntp.html

[Q87] JSON 字段做条件
来源：http://hz.daxiang520.top/gtcbzwswia.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cheryme.top/gtlrxtspgy.html

[Q88] 行转列（条件聚合）
来源：http://hz.c1oappe.top/gtwytsygyx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydzc1.top/gtittqyocn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.birdmap.top/gtmdfgypxz.html

[Q89] 判断表是否存在
来源：http://hz.xingfuxueyuan.xyz/gtsurvapqa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gtugpvgyoh.html

[Q90] 生成序号列
来源：http://hz.smart0.xyz/gtrwslqord.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtxlwnapvd.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxhoutayh.html

R. Bash 专题
来源：http://hz.jqgfzy.top/gtvegrbvkv.html

================================================================================
来源：http://hz.hfpthk.cn/gtdablklmu.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtvatjqdia.html

#!/usr/bin/env bash
来源：http://hz.ivvv.top/gtlnvubvge.html

set -euo pipefail
来源：http://hz.zycfv.cn/gtvhwivhem.html

[R02] 变量赋值与使用
来源：http://hz.yueranfly.top/gtcddjqzfu.html

name="Tom"; echo "$name"
来源：http://hz.cheryme.top/gtpkyjhone.html

[R03] 只读变量
来源：http://hz.andypj.xyz/gtbbylyefi.html

readonly PI=3.14
来源：http://hz.pycfn.com/gteyxecefu.html

[R04] 位置参数
来源：http://hz.dianchejie.cn/gtuhbswucv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.birdmap.top/gtbziycmcd.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtuiupixwr.html

name="${1:-default}"
来源：http://hz.wangdashe.top/gtloohgdgj.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtibnijexw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gotoacloud.top/gtattpehlf.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtaonefhil.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hfpthk.cn/gtfjwmmkin.html

[R08] 数值比较
来源：http://hz.gzhubu.top/gtfqedyatj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xylfe.cn/gtkmsxsmbs.html

[R09] 字符串比较
来源：http://hz.smart0.xyz/gtxsiovdjo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gtjuonnihv.html

[R10] 正则匹配
来源：http://hz.hnqzz.top/gtlsbmjccs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yonumen.top/gthafjtqat.html

[R11] case 多分支
来源：http://hz.52xcode.cn/gtflrizuyx.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gtdebscwqd.html

start) echo "启动" ;;
来源：http://hz.yvedp.cn/gtajrgmyup.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangkeji.top/gtgamyftqr.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigfzy.top/gtbuimftdj.html

esac
来源：http://hz.hnqzz.top/gtiodbvase.html

[R12] for 遍历文件
来源：http://hz.hongshengwenyu.top/gttacknkee.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guowangkeji.top/gtpblwhxjo.html

[R13] for 计数循环
来源：http://hz.xinyue.icu/gthpehbree.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shuidangran.top/gtbgfwuyhe.html

[R14] C 风格 for
来源：http://hz.xuanzx.com/gtjzwjksjz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.316326.xyz/gtazvaoksi.html

[R15] while 逐行读文件
来源：http://hz.hongshengwenyu.top/gteotdcfjg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj202588.top/gtjbeczwry.html

[R16] until 等待条件
来源：http://hz.jinghuilouyu.cn/gtwavioczk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xingfuxueyuan.xyz/gtwvdkioiv.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gtpjvtoepx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aizwys.cn/gtvdpyssmo.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gteganbpnm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jiagoushi.top/gtnlaypvzm.html

[R19] 数组长度
来源：http://hz.xziqi.cn/gtnbcmtleu.html

echo "${#arr[@]}"
来源：http://hz.daxiang520.top/gtrzrrvzml.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtqewtiria.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangshuangyany.cn/gtexwabzlv.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtlffdkrxw.html

echo "${#s}"
来源：http://hz.hongshengwenyu.top/gtozsblekm.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtflrkkzfj.html

echo "${s:0:5}"
来源：http://hz.guowangkeji.top/gtzmdpjuwz.html

[R23] 字符串替换
来源：http://hz.tian-w.cn/gtbhdcqpbn.html


<!-- 参考信息 -->