代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hz.yanxiufei.cn/gtyccfpnsj.html

Go:   len(arr);  len(m)
来源：http://hz.meibo888.top/gtjzokdtaw.html

Ruby: x.length;  x.size
来源：http://hz.ydjk.org.cn/gthxyyserd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ivvv.top/gthvuwuwtu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cashguo.top/gtpwdxzabl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxuanxn.top/gtkdmwrzfh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cashguo.top/gtreqjywlk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.iojbl.cn/gtsfxqneio.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pengpengdd.cyou/gtlmwfmncm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtzunxigdz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuetiantiany.cn/gtlqgfouqx.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gtzfdmjcpy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtozpbxwwl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ivvv.top/gtthrphwhb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.vqdsnc.cn/gtypeygqih.html

PHP:  if (empty($x)) {}
来源：http://hz.fengsongda.top/gtmvkaybry.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.havefunace.top/gtrvjebghe.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtwumqgeyh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zycfv.cn/gtdmmfuydq.html

Go:   if x == nil {}
来源：http://hz.hfpthk.cn/gtglfqvgdb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.iojbl.cn/gtqgjpemxv.html

C#:   if (x is null) {}
来源：http://hz.c1oappe.top/gtpmywalxx.html

[P07] 防抖与节流
来源：http://hz.daria6918.cn/gtlubzwacw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fengsongda.top/gtpenptjdh.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangtech.top/gtqhwnhuir.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtnawduqpf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtcvsknaqw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenlongwang.top/gtjschqmat.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cashguo.top/gtbdyunxbo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinqigufen.top/gtsuxdlmop.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shzxlz.cn/gtrfsnkxoo.html

[P08] 处理浮点精度问题
来源：http://hz.zhongyouzk.top/gtccygyync.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daria6918.cn/gtfvdzncgg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.vqdsnc.cn/gtjjqimyhj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.aizwys.cn/gthgdhjeqo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgufenzy.top/gtnrfmraec.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guannengcc.top/gtljcljeeg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtcgjdjhmp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuanzx.com/gtcuipufzz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sxryk.cn/gtsrvsjebj.html

================================================================================
来源：http://hz.daria6918.cn/gtmjbipgfm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhoulong.xyz/gtfezudbgx.html

================================================================================
来源：http://hz.bjfxy.top/gtdvkvuror.html

[Q01] 创建表
来源：http://hz.yanxiufei.cn/gtczlcthnu.html

CREATE TABLE users (
来源：http://hz.yj20258888.top/gtyowgzuwv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtfxcktbws.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aibaodan.cn/gthfjsizkp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydzc1.top/gtnkfwqsxa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gaohongyu789.top/gtyjamdewm.html

);
来源：http://hz.jiagoushi.top/gtfydcokpu.html

[Q02] 创建带外键的表
来源：http://hz.zhijiandao.cn/gtpdytcnzq.html

CREATE TABLE orders (
来源：http://hz.ybcxt.top/gtfnagzdqg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ehwqpu.com/gtoiupnkoe.html

user_id INT NOT NULL,
来源：http://hz.guannengcc.top/gtpatxsccx.html

amount DECIMAL(10, 2),
来源：http://hz.hnxiangtu.top/gtezmkblsd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gogol.net.cn/gtgzeegwui.html

);
来源：http://hz.andypj.xyz/gtwafmmljf.html

[Q03] 增加列
来源：http://hz.hnqzz.top/gtfumpilkf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tanke756.top/gtmgbyqmtw.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gtjyffcobx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtbfhebaxc.html

[Q05] 重命名列
来源：http://hz.zhiwuduotai.top/gtugqukneh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinghuilouyu.cn/gtbjrygadb.html

[Q06] 删除列
来源：http://hz.wangdashe.top/gtixlgbjax.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.quarkkingdee.top/gtmfzsvwmo.html

[Q07] 删除表
来源：http://hz.sweek.top/gtuxiqojgp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nanxinkj.top/gtswkmtqxy.html

[Q08] 创建普通索引
来源：http://hz.sysykeji.top/gtvqesvqbf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtcejtdgos.html

[Q09] 创建唯一索引
来源：http://hz.xylfe.cn/gtqakciwvg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gtdlaubopm.html

[Q10] 插入单行
来源：http://hz.nanxinkj.top/gtcqdrjfhy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cdnleiting.top/gtylhqyubs.html

[Q11] 一次插入多行
来源：http://hz.jiagoushi.top/gtophmlrxa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yanxiufei.cn/gtzpomqaxb.html

[Q12] 插入后取自增 ID
来源：http://hz.hongshengwenyu.top/gtyjlwmpzu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hammf.cn/gtolrbagbw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydjk.org.cn/gtrtafqsff.html

[Q13] 忽略重复插入
来源：http://hz.gogol.net.cn/gtzocrhozp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hnxiangtu.top/gtrxjduvev.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnqzz.top/gtphzbiuat.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ydjk.org.cn/gtipjfzqme.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhijiandao.cn/gtkwhgbnsa.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtmoivtqsd.html

SELECT * FROM users;
来源：http://hz.aibaodan.cn/gtwddqmlpb.html

[Q16] 查询指定列
来源：http://hz.jqgfzy.top/gtvdyirihp.html

SELECT id, name FROM users;
来源：http://hz.iojbl.cn/gtcinoirmw.html

[Q17] 条件查询
来源：http://hz.pycfn.com/gthwymrfzx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daxiang520.top/gtevbrbyra.html

[Q18] 模糊匹配
来源：http://hz.chenjidiqi.icu/gtxnyzdtoa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.quarkkingdee.top/gtcqgpndis.html

[Q19] 范围查询
来源：http://hz.sweek.top/gtceuzoszh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sxryk.cn/gtefzjodne.html

[Q20] IN 列表
来源：http://hz.daria6918.cn/gtkfiqafxd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhoulong.xyz/gtvpunpvwo.html

[Q21] 空值判断
来源：http://hz.xinyue.icu/gtbjgbyyfc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ppjwa.cn/gtbxsmugpy.html

[Q22] 排序
来源：http://hz.hnxiangtu.top/gtobiqksoc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cucudq.cn/gtuxvkdtyt.html

[Q23] 分页
来源：http://hz.zhaomingkeji.xyz/gtxrywtibe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtiwdzomtz.html

[Q24] 去重
来源：http://hz.jinghuilouyu.cn/gtwfxpqcpa.html

SELECT DISTINCT city FROM users;
来源：http://hz.hywenlv.cn/gtyvnxxcck.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtyvowdwlj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgufenzy.top/gttjalwlxx.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtxtzknntu.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gtwzzzzklk.html

[Q27] 条件计数
来源：http://hz.yj20258888.top/gtfpbxrbjo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtqevocaet.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gthzvipceh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.quarkkingdee.top/gtrqihkagt.html

[Q29] 最大最小值
来源：http://hz.feifeiyinyue.top/gtqgkvybyc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gogol.net.cn/gtidvlywkt.html

[Q30] 分组统计
来源：http://hz.ywan-chungtsiang.top/gtbzvdiqbm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtnqyqliby.html

[Q31] 分组后过滤
来源：http://hz.redwolf501.top/gtrygoylwn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gogol.net.cn/gtvgyydomv.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigfzy.top/gtvphqqats.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtothbkqae.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gtkzfrjcat.html

[Q33] 多列分组
来源：http://hz.birdmap.top/gtffniaxvp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnqzz.top/gtfejwuyjj.html

[Q34] 每组取第一条
来源：http://hz.jlsjyb.cn/gtnyngruda.html

SELECT * FROM (
来源：http://hz.cashguo.top/gtoyvzcjpk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gzhubu.top/gtkfmeaaok.html

) t WHERE rn = 1;
来源：http://hz.hongshengwenyu.top/gtqqkhabvl.html

[Q35] 内连接
来源：http://hz.fengsongda.top/gtnwocqcuo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtwmnvnjaa.html

[Q36] 左连接
来源：http://hz.cqqwz.cn/gtxufipvhh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtdusauhfh.html

[Q37] 右连接
来源：http://hz.snrcjt.cn/gtjiucogka.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangkeji.top/gthvphttpb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinqigfzy.top/gtzbaviugl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gtqordyvyg.html

[Q39] 自连接（查上下级）
来源：http://hz.zhijiandao.cn/gtzhyrrybq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinghuilouyu.cn/gtcghugyry.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.guannengcc.top/gtrwmewwfp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gtdnohjhil.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.0kj1m.cn/gthowohmdc.html

[Q41] 多表连接
来源：http://hz.kuanghao11.cn/gtxjupipvc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tianlin.xyz/gtnsykibxn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258888.top/gtrmvndibj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhijiandao.cn/gtcmjzmfuc.html

[Q42] 连接条件附加过滤
来源：http://hz.hammf.cn/gtoiiihhks.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtvdmslwbf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenlongwang.top/gtcmfcbqus.html

[Q43] 标量子查询
来源：http://hz.yj20258888.top/gtfjdyojsv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.9152youxi.cn/gtmnmyqtab.html

[Q44] IN 子查询
来源：http://hz.yanxiufei.cn/gtohsxerno.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xylfe.cn/gtvcorarrj.html

[Q45] EXISTS 判断存在
来源：http://hz.cashguo.top/gtywlgnysw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtqmigodal.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnxiangtu.top/gturtklgdz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtmbthxfuh.html

[Q47] 与平均值比较
来源：http://hz.xylfe.cn/gtbxwmndvs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydjk.org.cn/gtzvheiofr.html

[Q48] CTE 公用表表达式
来源：http://hz.dianchejie.cn/gtnbimhmhu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jyoumei.cn/gtfyerkdvf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhoulong.xyz/gtrxpufeca.html

[Q49] 更新单行
来源：http://hz.yanxiufei.cn/gtykpgdlcb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cheryme.top/gtfnlneyko.html

[Q50] 批量更新
来源：http://hz.xziqi.cn/gtnkcqzlom.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.c1oappe.top/gtzuqjzxvy.html

[Q51] 用子查询更新
来源：http://hz.feifeiyinyue.top/gtemckfqej.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gtcljjfiva.html

[Q52] 删除指定行
来源：http://hz.cqqwz.cn/gtuluznoor.html

DELETE FROM users WHERE id = 10;
来源：http://hz.birdmap.top/gtneaxlehx.html

[Q53] 按条件删除
来源：http://hz.wangshuangyany.cn/gtpbvnnqhi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hongshengwenyu.top/gtudxdtytm.html

[Q54] 清空表
来源：http://hz.dashuyun.cn/gtcsnhhjqx.html

TRUNCATE TABLE logs;
来源：http://hz.ydzc1.top/gtjqbxivaf.html

[Q55] 排名（并列占位）
来源：http://hz.xingfuxueyuan.xyz/gtvcruswyr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhoulong.xyz/gtxsvfxzjp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.andypj.xyz/gtlguwyhgx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jiagoushi.top/gtkmsavqzq.html

[Q57] 行号
来源：http://hz.ivvv.top/gtbakvinlu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydzc1.top/gtkgqcgzps.html

[Q58] 累计求和
来源：http://hz.nanxuanxn.top/gtmnldtkwe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtniucfexw.html

[Q59] 分组内累计
来源：http://hz.zhongyouzk.top/gtxxiksaxu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cashguo.top/gtwmsvtrby.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtnytbxwdn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtsbymknoy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtvxcfyloh.html

[Q61] 移动平均
来源：http://hz.hysaishi.cn/gtehrvcjjk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.guannengcc.top/gtzluoeuwx.html

[Q62] 分组占比
来源：http://hz.hnqzz.top/gtcuuzfegp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtuugocmgy.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtxplpkehp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.smart0.xyz/gturxehcgg.html

[Q64] 提交事务
来源：http://hz.cucudq.cn/gtytmhcbim.html

COMMIT;
来源：http://hz.mhx1999.top/gtyzhvjwyg.html

[Q65] 回滚事务
来源：http://hz.meibo888.top/gtbvgrzfwq.html

ROLLBACK;
来源：http://hz.sysykeji.top/gtunpclcxj.html

[Q66] 行锁查询
来源：http://hz.cucudq.cn/gtgmsnwzum.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cucudq.cn/gtfamtliwc.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtwwqkrcse.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinyuanbaomall.cn/gtabadhlgj.html

[Q68] 保存点
来源：http://hz.hongshengwenyu.top/gtfzdtrmlm.html

SAVEPOINT sp1;
来源：http://hz.hysaishi.cn/gtecertyxq.html

ROLLBACK TO sp1;
来源：http://hz.xingfuxueyuan.xyz/gthwzdpbgh.html

[Q69] 查看执行计划
来源：http://hz.sweek.top/gtmpokntkm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fengsongda.top/gtpfjquuni.html

[Q70] 更新统计信息
来源：http://hz.yongpay.top/gtlwmaelrr.html

ANALYZE TABLE users;
来源：http://hz.0kj1m.cn/gtfnhxdqyd.html

[Q71] 查看建表语句
来源：http://hz.hongshengwenyu.top/gtacgynkuv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinyuanbaomall.cn/gtjcxkvses.html

[Q72] 查看索引
来源：http://hz.ydzc1.top/gtaxmaflqi.html

SHOW INDEX FROM users;
来源：http://hz.xylfe.cn/gtvwwjvfhl.html

[Q73] 查看表状态
来源：http://hz.hnxiangtu.top/gtdaqmgmjc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuanzhike.top/gtdcyffcrd.html

[Q74] 强制使用索引
来源：http://hz.chenlongwang.top/gtqdockamj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gthpzatsuz.html

[Q75] 日期格式化
来源：http://hz.vqdsnc.cn/gttelvxlew.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhiwuduotai.top/gtbssjbaok.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtbdiginxn.html

[Q76] 按天统计
来源：http://hz.yj202588.top/gtobqolbtd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jyoumei.cn/gtpbcnhvxb.html

[Q77] 时间加减
来源：http://hz.pengpengdd.cyou/gtrvyqcntz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xuetiantiany.cn/gtohvnvqcc.html

[Q78] 当前时间
来源：http://hz.cqqwz.cn/gtuymxxowj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.0kj1m.cn/gtemwjzxun.html

[Q79] 字符串拼接
来源：http://hz.svipenyu.cn/gtogwsnhrv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigufen.top/gtcleiqjuf.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtoymioqfr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jyoumei.cn/gtfcbrlqqf.html

[Q81] 字符串替换
来源：http://hz.cqqwz.cn/gtvagwgajn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.316326.xyz/gtbngpyzpb.html

[Q82] 字符长度与字节长度
来源：http://hz.yj202588.top/gtnapjznka.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.svipenyu.cn/gtqdjupvyx.html

[Q83] 大小写转换
来源：http://hz.hnqzz.top/gtirdzuryh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sweek.top/gtlugytbbw.html

[Q84] 去除首尾空格
来源：http://hz.jlsjyb.cn/gtoscjzexs.html

SELECT TRIM(name) FROM users;
来源：http://hz.iojbl.cn/gttyjdgwpf.html

[Q85] 数值取整
来源：http://hz.jinqigfzy.top/gtbcowdkkg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhijiandao.cn/gtscmgeslm.html

[Q86] 读取 JSON 字段
来源：http://hz.svipenyu.cn/gtferegtpm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gtasktndnt.html

[Q87] JSON 字段做条件
来源：http://hz.nanxinkj.top/gtxyfmdxap.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pycfn.com/gtqcdmqafv.html

[Q88] 行转列（条件聚合）
来源：http://hz.zdqjudy.top/gtqtvpjdab.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtzcsyydur.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.9152youxi.cn/gtdashchqc.html

[Q89] 判断表是否存在
来源：http://hz.xuanzx.com/gtgeutfhat.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guowangkeji.top/gtxapcmbot.html

[Q90] 生成序号列
来源：http://hz.shzxlz.cn/gtlgolshfk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuetiantiany.cn/gtptjbnjcy.html

================================================================================
来源：http://hz.tian-w.cn/gtklbyyahr.html

R. Bash 专题
来源：http://hz.haohaochexian.top/gtuibeoibb.html

================================================================================
来源：http://hz.wangdashe.top/gtajfxiuxp.html

[R01] shebang 与严格模式
来源：http://hz.zhoulong.xyz/gtsykvwpcf.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangkeji.top/gtfjxazmix.html

set -euo pipefail
来源：http://hz.yongpay.top/gtsqdewluf.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtttlwprzp.html

name="Tom"; echo "$name"
来源：http://hz.zhixingplan.top/gtwdgqwpxb.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtpnmhdyil.html

readonly PI=3.14
来源：http://hz.jinyuanbaomall.cn/gtqcykpbcu.html

[R04] 位置参数
来源：http://hz.xziqi.cn/gtrapjnxub.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtmveqkxww.html

[R05] 参数默认值
来源：http://hz.yonumen.top/gtveunqrnl.html

name="${1:-default}"
来源：http://hz.ehwqpu.com/gtmuklkugw.html

[R06] 判断命令是否存在
来源：http://hz.316326.xyz/gtvzlxupxp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhixingplan.top/gtajmwonon.html

[R07] if 判断文件
来源：http://hz.hammf.cn/gtyekljppt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.c1oappe.top/gtiihtjrib.html

[R08] 数值比较
来源：http://hz.tian-w.cn/gtvkrrcuyj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhongyouzk.top/gttgodocjl.html

[R09] 字符串比较
来源：http://hz.jiagoushi.top/gtzttontuy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jqgufenzy.top/gtdbopxqga.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gttwudeeng.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhijiandao.cn/gtyqkzohkq.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtwainnkhx.html

case "$1" in
来源：http://hz.vqdsnc.cn/gtjtnzdnft.html

start) echo "启动" ;;
来源：http://hz.jyoumei.cn/gtkebkyoqa.html

stop)  echo "停止" ;;
来源：http://hz.ydzc1.top/gtfvfziboa.html

*)     echo "未知命令" ;;
来源：http://hz.ppjwa.cn/gteptmbkuo.html

esac
来源：http://hz.mhx1999.top/gthicolvpy.html

[R12] for 遍历文件
来源：http://hz.yueranfly.top/gtpthtkjst.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guowangkeji.top/gthjmuerxo.html

[R13] for 计数循环
来源：http://hz.daria6918.cn/gthdxjbdcm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtrcqkwhth.html

[R14] C 风格 for
来源：http://hz.shanyushiyangtech.top/gtnxzwgcza.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sweek.top/gticjezatd.html

[R15] while 逐行读文件
来源：http://hz.feifeiyinyue.top/gtdobwdqcm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gtkqbutpks.html

[R16] until 等待条件
来源：http://hz.sufxvd.cn/gtfatzewra.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtjunwelaz.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtiyztvzdo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gtspqrtaow.html

[R18] 遍历数组
来源：http://hz.ivvv.top/gtftitlhax.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gtketzdgid.html

[R19] 数组长度
来源：http://hz.bjfxy.top/gtvqnujvlq.html

echo "${#arr[@]}"
来源：http://hz.zhijiandao.cn/gtzjwvzuuk.html

[R20] 关联数组（字典）
来源：http://hz.ydjk.org.cn/gtmcppxnog.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.birdmap.top/gtcidjhkog.html

[R21] 字符串长度
来源：http://hz.tianlin.xyz/gtgqxsocwt.html

echo "${#s}"
来源：http://hz.sweek.top/gtlaptxvau.html

[R22] 截取子串
来源：http://hz.zdqjudy.top/gtwnbdprot.html

echo "${s:0:5}"
来源：http://hz.shanyushiyangkeji.top/gtxevtzagb.html

[R23] 字符串替换
来源：http://hz.dashuyun.cn/gtshdscsdw.html


<!-- 参考信息 -->