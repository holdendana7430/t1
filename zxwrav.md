代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtiwretogn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gtjzihzxrr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guannengcc.top/gttesgqfyk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xingfuxueyuan.xyz/gtdilqehuu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tian-w.cn/gtnmvrfgjf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tanke756.top/gtgmrdcgiy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gtyuwlliqt.html

Ruby: a == b
来源：http://hz.pengpengdd.cyou/gtpvnhkyeb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinghuilouyu.cn/gtitqywusy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zdqjudy.top/gtbxkqlwsy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ppjwa.cn/gtzvribuwj.html

PHP:  if (empty($x)) {}
来源：http://hz.jinyuanbaomall.cn/gtendurseu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sysykeji.top/gtdilqofve.html

TS:   if (x == null) {}
来源：http://hz.shangyingyoupin.top/gtqxoshxiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sxryk.cn/gtpnzqhznw.html

Go:   if x == nil {}
来源：http://hz.bjfxy.top/gttcdmxcnh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtoznhdlqx.html

C#:   if (x is null) {}
来源：http://hz.jqgufenzy.top/gtocmjrclb.html

[P07] 防抖与节流
来源：http://hz.zhiwuduotai.top/gtrusqujve.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxinkj.top/gtbjrdcmzz.html

PHP:  // 手写时间戳比较
来源：http://hz.zhixingplan.top/gtvwnpvbih.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtukqzotuq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gtjduoaaga.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.316326.xyz/gtatwupqzp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhixingplan.top/gtsyytjade.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.feifeiyinyue.top/gtzhtowisd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jyoumei.cn/gttcegycid.html

[P08] 处理浮点精度问题
来源：http://hz.sufxvd.cn/gtlnmyxlel.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yonumen.top/gtcmcjqcmb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shuidangran.top/gtqncsqghp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangshuangyany.cn/gtxzdefqvr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hysaishi.cn/gtpxkwpqbp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhoulong.xyz/gtvuecnyoi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gtkbzcejdy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258888.top/gtblzzqrou.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtrzqhofuk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtgngivvvw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yongpay.top/gthcyifbjw.html

================================================================================
来源：http://hz.jiagoushi.top/gtfpkztqvn.html

[Q01] 创建表
来源：http://hz.daxiang520.top/gtbtggivhx.html

CREATE TABLE users (
来源：http://hz.pengpengdd.cyou/gtcozhgdzx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cheryme.top/gtwvuqbabf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtgxwlymvp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuanzx.com/gtojsrpgbw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yanxiufei.cn/gtkkavyjzh.html

);
来源：http://hz.guowangkeji.top/gttxxuncml.html

[Q02] 创建带外键的表
来源：http://hz.pengpengdd.cyou/gtmcpkkjmm.html

CREATE TABLE orders (
来源：http://hz.ywan-chungtsiang.top/gtlgfywmma.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.havefunace.top/gtgdzavivz.html

user_id INT NOT NULL,
来源：http://hz.hammf.cn/gtoamlszba.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigufen.top/gtkxswbftg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jqgfzy.top/gtniixqalq.html

);
来源：http://hz.ppjwa.cn/gtceycaojw.html

[Q03] 增加列
来源：http://hz.jqgfzy.top/gtviflbbkn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhongyouzk.top/gtykvtlujp.html

[Q04] 修改列类型
来源：http://hz.cdnleiting.top/gtjlkawwoc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dianchejie.cn/gtbxefpmmx.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtryqhdltf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.havefunace.top/gtmtawcuiq.html

[Q06] 删除列
来源：http://hz.ywan-chungtsiang.top/gtopkbrpzb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aizwys.cn/gtikcptzxz.html

[Q07] 删除表
来源：http://hz.xylfe.cn/gtrdoekywu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dashuyun.cn/gtwryanmox.html

[Q08] 创建普通索引
来源：http://hz.xziqi.cn/gtfdmsdwig.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtgahlfphi.html

[Q09] 创建唯一索引
来源：http://hz.ydjk.org.cn/gtsigzuyso.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtevfyihdg.html

[Q10] 插入单行
来源：http://hz.zhengqikj.top/gteaxmklcl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yueranfly.top/gttlesvine.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtnjttvgxe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ywan-chungtsiang.top/gtodedrnyi.html

[Q12] 插入后取自增 ID
来源：http://hz.zhengqikj.top/gtatrseazc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shangyingyoupin.top/gtvbwyhujv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tanke756.top/gtrpdajsbt.html

[Q13] 忽略重复插入
来源：http://hz.sysykeji.top/gtovqhxlrh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ehwqpu.com/gtvfrzcmnk.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj202588.top/gtianxeqrv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guowangkeji.top/gtszxxtmfs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xingfuxueyuan.xyz/gthgmdljex.html

[Q15] 查询全部
来源：http://hz.tian-w.cn/gtyzhwsoun.html

SELECT * FROM users;
来源：http://hz.jyoumei.cn/gtbvybxpsa.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gtzthygtkn.html

SELECT id, name FROM users;
来源：http://hz.jqgfzy.top/gteutvscaf.html

[Q17] 条件查询
来源：http://hz.jianghu66.top/gtfyzfatnu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhongyouzk.top/gtejjtevya.html

[Q18] 模糊匹配
来源：http://hz.zhijiandao.cn/gtrdlfirgh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hywenlv.cn/gtxgvefbcu.html

[Q19] 范围查询
来源：http://hz.xinyue.icu/gtvjlguzvy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nwbrower.top/gtbdqkskwb.html

[Q20] IN 列表
来源：http://hz.jinghuilouyu.cn/gtlozcikuj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yangfankeji.com/gtlvvlfdvw.html

[Q21] 空值判断
来源：http://hz.shangyingyoupin.top/gtbksnxfsu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.iojbl.cn/gtzjmwddsg.html

[Q22] 排序
来源：http://hz.wangshuangyany.cn/gthfehedkw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ivvv.top/gtttfwipbt.html

[Q23] 分页
来源：http://hz.hywenlv.cn/gtpgprygum.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yongpay.top/gtuddtqeqh.html

[Q24] 去重
来源：http://hz.yongpay.top/gtcuesofdq.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258.top/gtzggfvnqf.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gttgmjcsxc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.kuanghao11.cn/gtalzhjnvl.html

[Q26] 计数
来源：http://hz.yongpay.top/gtpbcztjag.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinqigufen.top/gtwivtkatf.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtkuodzwpy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gtrrjpdqmd.html

[Q28] 求和与平均
来源：http://hz.pengpengdd.cyou/gtumhlqwxn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuanzhike.top/gtwfjqzeqd.html

[Q29] 最大最小值
来源：http://hz.zhixingplan.top/gtpdzvnywr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gtwtbpimue.html

[Q30] 分组统计
来源：http://hz.chenzaomai.com/gtvsukaihy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtqphtjxhn.html

[Q31] 分组后过滤
来源：http://hz.zhengqikj.top/gtwxhyhbzo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gotoacloud.top/gtukmzwkmc.html

[Q32] 分组拼接字符串
来源：http://hz.sweek.top/gtlzfcdeye.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtezzrharf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hywenlv.cn/gtgocpshnx.html

[Q33] 多列分组
来源：http://hz.wangdashe.top/gttubloazc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dianchejie.cn/gtqqglaihs.html

[Q34] 每组取第一条
来源：http://hz.shzxlz.cn/gtlcdbohpu.html

SELECT * FROM (
来源：http://hz.quarkkingdee.top/gtnfnkadaw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhijiandao.cn/gtfasofwfn.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtptpgqcbk.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gtoozgribs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtxbadotku.html

[Q36] 左连接
来源：http://hz.havefunace.top/gtcrdkfbvf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtzzxkahib.html

[Q37] 右连接
来源：http://hz.yvedp.cn/gtoqsbacmi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhongyouzk.top/gtsznijxgr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhixingplan.top/gtwcgblgue.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtwoorjdmx.html

[Q39] 自连接（查上下级）
来源：http://hz.havefunace.top/gtizvjvbqw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sysykeji.top/gtwutruspm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangshuangyany.cn/gtssyncrfl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hysaishi.cn/gtrumhprxt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenzaomai.com/gtthcbimzq.html

[Q41] 多表连接
来源：http://hz.bjfxy.top/gtwpdqudqi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.wangshuangyany.cn/gtfwcbfcnz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.dianchejie.cn/gtvawhuxrk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.meibo888.top/gtptqkrbow.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtmugryfzh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hongshengwenyu.top/gtrvmupvzr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daxiang520.top/gtqeeamfzx.html

[Q43] 标量子查询
来源：http://hz.shangyingyoupin.top/gtnzehlzwq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhengqikj.top/gtibifjgmp.html

[Q44] IN 子查询
来源：http://hz.sxryk.cn/gttbbmucup.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuetiantiany.cn/gtlycyqziw.html

[Q45] EXISTS 判断存在
来源：http://hz.shzxlz.cn/gtnzdvxfow.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pycfn.com/gthpqonioi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aibaodan.cn/gtraizllis.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtvicarzhb.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtfgqujixu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtdmjogayu.html

[Q48] CTE 公用表表达式
来源：http://hz.ppjwa.cn/gtqypirdhb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.andypj.xyz/gtlwlhpscq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigufen.top/gttvffnngg.html

[Q49] 更新单行
来源：http://hz.svipenyu.cn/gtwxrvqvpx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtfqcriepa.html

[Q50] 批量更新
来源：http://hz.hysaishi.cn/gtlkipisgr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sxryk.cn/gtmgerjaqm.html

[Q51] 用子查询更新
来源：http://hz.smart0.xyz/gtheldoxfq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnxiangtu.top/gtnodiibrb.html

[Q52] 删除指定行
来源：http://hz.nanxuanxn.top/gtkcwjwsxl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gzhubu.top/gtipffuncp.html

[Q53] 按条件删除
来源：http://hz.hongshengwenyu.top/gtdgbqbglc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cucudq.cn/gtkqwckwax.html

[Q54] 清空表
来源：http://hz.ydzc1.top/gtashkqdtw.html

TRUNCATE TABLE logs;
来源：http://hz.nwbrower.top/gtbecyociu.html

[Q55] 排名（并列占位）
来源：http://hz.yj202588.top/gtevkmmmce.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pycfn.com/gtexdllxal.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fzhhl.top/gtttykyoyj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtiquosdoa.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtfcfmwgig.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtvvpylhxv.html

[Q58] 累计求和
来源：http://hz.yanxiufei.cn/gtkdbizgoq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sufxvd.cn/gtgxbmrius.html

[Q59] 分组内累计
来源：http://hz.jinyuanbaomall.cn/gteqmojncb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hammf.cn/gttpytfulu.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydjk.org.cn/gtmsehoqsg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.kuanghao11.cn/gtyuxzskbe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258888.top/gtjfwlqbpp.html

[Q61] 移动平均
来源：http://hz.hfpthk.cn/gtpmjfgidr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj20258888.top/gtbqwznzft.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtnxukrxpi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtwijizlsx.html

[Q63] 开启事务
来源：http://hz.chenjidiqi.icu/gtmesbmkhh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aizwys.cn/gtrsprwksi.html

[Q64] 提交事务
来源：http://hz.guowangkeji.top/gtycyvbnok.html

COMMIT;
来源：http://hz.hysaishi.cn/gtndzbgmrg.html

[Q65] 回滚事务
来源：http://hz.shangyingyoupin.top/gtcqfzqypi.html

ROLLBACK;
来源：http://hz.yongpay.top/gtcmvmqmec.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtpnrdebfs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fzhhl.top/gtnelpupbt.html

[Q67] 设置隔离级别
来源：http://hz.hnxiangtu.top/gthhqysowq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hysaishi.cn/gtmfxnvkgq.html

[Q68] 保存点
来源：http://hz.daria6918.cn/gtuvjwhmvk.html

SAVEPOINT sp1;
来源：http://hz.xylfe.cn/gthnrwwfgm.html

ROLLBACK TO sp1;
来源：http://hz.kuanghao11.cn/gtrtpchlwk.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gttxbbvbzv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cheryme.top/gtkaxybfnl.html

[Q70] 更新统计信息
来源：http://hz.cdnleiting.top/gtkytouetx.html

ANALYZE TABLE users;
来源：http://hz.zhaomingkeji.xyz/gtqgbydmyb.html

[Q71] 查看建表语句
来源：http://hz.gotoacloud.top/gtixcjwtnu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gtwtakrlql.html

[Q72] 查看索引
来源：http://hz.wangshuangyany.cn/gtvzrgudhd.html

SHOW INDEX FROM users;
来源：http://hz.smart0.xyz/gtsnpmxkti.html

[Q73] 查看表状态
来源：http://hz.pengpengdd.cyou/gtamkqdxxh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenzaomai.com/gtpjcxkgpi.html

[Q74] 强制使用索引
来源：http://hz.52xcode.cn/gtvfrzucfa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shzxlz.cn/gtqankqbpj.html

[Q75] 日期格式化
来源：http://hz.yangfankeji.com/gtvcwamjqm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.andypj.xyz/gtaaxoohut.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangkeji.top/gtatfnlplt.html

[Q76] 按天统计
来源：http://hz.yj202588.top/gtldqxgrrs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yanxiufei.cn/gtizbkjpet.html

[Q77] 时间加减
来源：http://hz.xuanzx.com/gtddwwklou.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cqqwz.cn/gtfmbttlta.html

[Q78] 当前时间
来源：http://hz.pengpengdd.cyou/gtjfcmehup.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.havefunace.top/gtuszdajha.html

[Q79] 字符串拼接
来源：http://hz.tanke756.top/gtedihtpfa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guannengcc.top/gtdpqlwcof.html

[Q80] 字符串截取
来源：http://hz.andypj.xyz/gtrktjzgxx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aizwys.cn/gtqcpakcoe.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtnjgcpxvw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ybcxt.top/gtxskjbvgl.html

[Q82] 字符长度与字节长度
来源：http://hz.vqdsnc.cn/gttrqietbd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cqqwz.cn/gtfbxjbmhz.html

[Q83] 大小写转换
来源：http://hz.kuanghao11.cn/gtgnzgkbcn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nwbrower.top/gtfvtesypg.html

[Q84] 去除首尾空格
来源：http://hz.hfpthk.cn/gtbeinkwdz.html

SELECT TRIM(name) FROM users;
来源：http://hz.xylfe.cn/gtezyynssj.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gtcsczddlt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtpatcvugw.html

[Q86] 读取 JSON 字段
来源：http://hz.shuidangran.top/gtwtkfoixl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cdnleiting.top/gtheyotxsf.html

[Q87] JSON 字段做条件
来源：http://hz.smart0.xyz/gtgbycvcxb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxinkj.top/gtjigghlsk.html

[Q88] 行转列（条件聚合）
来源：http://hz.iojbl.cn/gtwfuqzpzr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hongshengwenyu.top/gtplmuuobz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenjidiqi.icu/gttnvpppyd.html

[Q89] 判断表是否存在
来源：http://hz.nanxuanxn.top/gtzohpvdtc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.316326.xyz/gtdzjrayuy.html

[Q90] 生成序号列
来源：http://hz.redwolf501.top/gtrhunqlar.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tian-w.cn/gtmlvcvpcx.html

================================================================================
来源：http://hz.ehwqpu.com/gtzytxyzvb.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtwyfmbktw.html

================================================================================
来源：http://hz.aizwys.cn/gtfwalcuji.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtdyvomukd.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtxuoqrdnc.html

set -euo pipefail
来源：http://hz.52xcode.cn/gtirynprrw.html

[R02] 变量赋值与使用
来源：http://hz.hnqzz.top/gtqukaurnm.html

name="Tom"; echo "$name"
来源：http://hz.cheryme.top/gtqovywwln.html

[R03] 只读变量
来源：http://hz.zhongyouzk.top/gtlnkjbdht.html

readonly PI=3.14
来源：http://hz.chenjidiqi.icu/gtubtwmlew.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gtfchggjow.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.mhx1999.top/gtacmblytj.html

[R05] 参数默认值
来源：http://hz.cashguo.top/gtuskurljw.html

name="${1:-default}"
来源：http://hz.yangfankeji.com/gtmsykpkqw.html

[R06] 判断命令是否存在
来源：http://hz.zhengqikj.top/gtkppthcnx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.haohaochexian.top/gtmodkqtbu.html

[R07] if 判断文件
来源：http://hz.hnxiangtu.top/gttxvpenit.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guowangkeji.top/gtcwighmfa.html

[R08] 数值比较
来源：http://hz.gogol.net.cn/gtlimzjgac.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtmqrskarc.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtafohbrkg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhoulong.xyz/gthuveogxc.html

[R10] 正则匹配
来源：http://hz.pycfn.com/gtgyyrqfdy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gtysgtohwc.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtbqwhpnpd.html

case "$1" in
来源：http://hz.0kj1m.cn/gtjtxnncdi.html

start) echo "启动" ;;
来源：http://hz.chenlongwang.top/gtcqkiwefi.html

stop)  echo "停止" ;;
来源：http://hz.shangyingyoupin.top/gtbuiygdwu.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtoagbrijj.html

esac
来源：http://hz.cucudq.cn/gtmzcbwufe.html

[R12] for 遍历文件
来源：http://hz.ywan-chungtsiang.top/gtmfpchrfl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.quarkkingdee.top/gtggnkqjyn.html

[R13] for 计数循环
来源：http://hz.yanxiufei.cn/gtomsxrjgm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yanxiufei.cn/gtqilfryua.html

[R14] C 风格 for
来源：http://hz.birdmap.top/gtluxoramc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shuidangran.top/gtguatlgvx.html

[R15] while 逐行读文件
来源：http://hz.yj202588.top/gtrjyoibqi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtgytzmuue.html

[R16] until 等待条件
来源：http://hz.snrcjt.cn/gtbrecnaic.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aibaodan.cn/gtajvynqjb.html

[R17] 数组定义与取值
来源：http://hz.pycfn.com/gtkmoimkud.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.haohaochexian.top/gtmpiozphb.html

[R18] 遍历数组
来源：http://hz.jinyuanbaomall.cn/gtmrsgworc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.52xcode.cn/gtlygpzffs.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gthmveldsg.html

echo "${#arr[@]}"
来源：http://hz.shuidangran.top/gtlodmnadi.html

[R20] 关联数组（字典）
来源：http://hz.sysykeji.top/gtdzksedkd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hysaishi.cn/gtzjcdaywc.html

[R21] 字符串长度
来源：http://hz.0kj1m.cn/gtwbgehhxf.html

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtvfdkpqix.html

[R22] 截取子串
来源：http://hz.redwolf501.top/gtnirkinmw.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gtldzjzjfn.html

[R23] 字符串替换
来源：http://hz.xuetiantiany.cn/gtklymqxgt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenzaomai.com/gtnzdrecoi.html

[R24] 大小写转换
来源：http://hz.dashuyun.cn/gtswloxvdl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sweek.top/gtrmovzlwv.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gtuutyjigq.html


<!-- 参考信息 -->