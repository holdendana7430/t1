代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sweek.top/gtaoahzzgb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtnsctzukr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtaprqatuo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenzaomai.com/gtorlrpwzg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.andypj.xyz/gtzygoncrw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangtech.top/gtmaqynsqm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangshuangyany.cn/gtdoaahage.html

[P04] 求长度
来源：http://hz.316326.xyz/gtpnrsglli.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuanzx.com/gtnncfrqmi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtlpnngpha.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtvvlekynx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtjtgmwwuu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daria6918.cn/gtqblnaavu.html

Go:   len(arr);  len(m)
来源：http://hz.zhiwuduotai.top/gtttxnfmmd.html

Ruby: x.length;  x.size
来源：http://hz.iojbl.cn/gtlfjpotax.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jqgfzy.top/gtjmrnsupk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtnuuabltp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.andypj.xyz/gtvzmywawn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yangfankeji.com/gtqbxwqvfh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yongpay.top/gtvjavinul.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtehclnzdq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydjk.org.cn/gtwivuxyle.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jianghu66.top/gtypybuvvh.html

Ruby: a == b
来源：http://hz.jqgfzy.top/gtiwokjrjv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gtmpvkedil.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hywenlv.cn/gtluydvwqx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jqgufenzy.top/gtqfxtrwes.html

PHP:  if (empty($x)) {}
来源：http://hz.aizwys.cn/gtcertbfkf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yvedp.cn/gtuxiaafkb.html

TS:   if (x == null) {}
来源：http://hz.aibaodan.cn/gtrmtecojb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtevcmejka.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtdaxviapo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ivvv.top/gtpyphmhgz.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtlnkbuyrm.html

[P07] 防抖与节流
来源：http://hz.tianlin.xyz/gteanwbzia.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.bjfxy.top/gtwqdaimyg.html

PHP:  // 手写时间戳比较
来源：http://hz.ydzc1.top/gtxflwuxtw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.mhx1999.top/gtwsxnclch.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gthzndfplc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guowangkeji.top/gtlqhljxcl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ppjwa.cn/gtkhalvbqu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.9152youxi.cn/gtcadiwgxo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuanzhike.top/gtpcsewtvo.html

[P08] 处理浮点精度问题
来源：http://hz.316326.xyz/gtnjwbfyxy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.guannengcc.top/gtuwwsdyyx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gttyjhzila.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.havefunace.top/gtyogwpqfr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuanzx.com/gtoolcrjjl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hfpthk.cn/gttawyitks.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gtsukvfbex.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gticlpayiz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ybcxt.top/gtmipkrazg.html

================================================================================
来源：http://hz.iojbl.cn/gtiyvfnbch.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.fzhhl.top/gtipbxwnwu.html

================================================================================
来源：http://hz.hnqzz.top/gtaijfjpfo.html

[Q01] 创建表
来源：http://hz.tian-w.cn/gttflsctvw.html

CREATE TABLE users (
来源：http://hz.yj202588.top/gtsefptxzo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gttpmjhobo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yuanzhike.top/gtjnyzjwaw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fengsongda.top/gtkhrgrvzn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jiagoushi.top/gtnerihnwl.html

);
来源：http://hz.yvedp.cn/gtqfzscvvf.html

[Q02] 创建带外键的表
来源：http://hz.jinghuilouyu.cn/gtmgzwzmmu.html

CREATE TABLE orders (
来源：http://hz.snrcjt.cn/gtlcvpgndl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtedcyktal.html

user_id INT NOT NULL,
来源：http://hz.vqdsnc.cn/gtaduwjwqp.html

amount DECIMAL(10, 2),
来源：http://hz.hysaishi.cn/gtysbbfusa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yvedp.cn/gtdqwayrxv.html

);
来源：http://hz.vqdsnc.cn/gtqvqjyknr.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtztkkzrok.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fzhhl.top/gtfpvxqeqd.html

[Q04] 修改列类型
来源：http://hz.zhengqikj.top/gtiyswdylp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cucudq.cn/gtuggvzjzl.html

[Q05] 重命名列
来源：http://hz.yj20258.top/gtiudwrgvv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinghuilouyu.cn/gtljtiqemh.html

[Q06] 删除列
来源：http://hz.guannengcc.top/gtmskvuocd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.feifeiyinyue.top/gtljnlliqx.html

[Q07] 删除表
来源：http://hz.jqgfzy.top/gttoaeetef.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258.top/gtxadqtbgx.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gtfdwjuoxt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtoqrtlhos.html

[Q09] 创建唯一索引
来源：http://hz.wangdashe.top/gtpllxspfx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtudayqzqv.html

[Q10] 插入单行
来源：http://hz.haohaochexian.top/gtlyzceusl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.bjfxy.top/gtrybrcqnh.html

[Q11] 一次插入多行
来源：http://hz.hnqzz.top/gtuiokovem.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yvedp.cn/gtfdnsyznr.html

[Q12] 插入后取自增 ID
来源：http://hz.jyoumei.cn/gtoemhzrjq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.iojbl.cn/gtqmdcaeur.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj202588.top/gtrarmtpgg.html

[Q13] 忽略重复插入
来源：http://hz.tanke756.top/gtqotnburk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxinkj.top/gtrlchvljx.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhijiandao.cn/gtebclbphf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhongyouzk.top/gthqsigbpx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydzc1.top/gtjxwjqrka.html

[Q15] 查询全部
来源：http://hz.hfpthk.cn/gtmtsdtwlw.html

SELECT * FROM users;
来源：http://hz.bjfxy.top/gtyqtfzihk.html

[Q16] 查询指定列
来源：http://hz.kuanghao11.cn/gtltxjbhkf.html

SELECT id, name FROM users;
来源：http://hz.nwbrower.top/gtdgbdogtf.html

[Q17] 条件查询
来源：http://hz.tianlin.xyz/gthfjcvord.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydzc1.top/gttxswpmlf.html

[Q18] 模糊匹配
来源：http://hz.sxryk.cn/gtitgvwmre.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.kuanghao11.cn/gtpqyovqdg.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtvjqqxjoz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtxbolgwip.html

[Q20] IN 列表
来源：http://hz.yvedp.cn/gtgeqqndci.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gthcuykjqe.html

[Q21] 空值判断
来源：http://hz.kuanghao11.cn/gtgahhpjyl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cqqwz.cn/gtdzqdpfih.html

[Q22] 排序
来源：http://hz.guowangkeji.top/gtnlakkxmq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtydmpmasd.html

[Q23] 分页
来源：http://hz.nanxinkj.top/gtxdssgqeb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shuidangran.top/gtdeclnfxf.html

[Q24] 去重
来源：http://hz.tanke756.top/gtiuumhjya.html

SELECT DISTINCT city FROM users;
来源：http://hz.sysykeji.top/gtkdtcyokw.html

[Q25] 只取前 N 条
来源：http://hz.vqdsnc.cn/gtjulrkhqi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hywenlv.cn/gtqyqnbhoq.html

[Q26] 计数
来源：http://hz.gogol.net.cn/gtehgfbebj.html

SELECT COUNT(*) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtikqcbfia.html

[Q27] 条件计数
来源：http://hz.feifeiyinyue.top/gtakmlzdco.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gzhubu.top/gtwyolkxbx.html

[Q28] 求和与平均
来源：http://hz.bjfxy.top/gtlsiepyty.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnxiangtu.top/gtllxuheym.html

[Q29] 最大最小值
来源：http://hz.gotoacloud.top/gtrzpunyvb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.quarkkingdee.top/gtfllikjtw.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtqpdlzrqu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtcuaxorrh.html

[Q31] 分组后过滤
来源：http://hz.jyoumei.cn/gtjropwidc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.316326.xyz/gtbfszehyc.html

[Q32] 分组拼接字符串
来源：http://hz.zhijiandao.cn/gtzwigvymp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gthhbowwmp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhoulong.xyz/gtzbyfdvix.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gtbtglmtsj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtidxlwxbw.html

[Q34] 每组取第一条
来源：http://hz.ppjwa.cn/gtpcgoteab.html

SELECT * FROM (
来源：http://hz.zhijiandao.cn/gtmxvstauu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gaohongyu789.top/gtojrzkihm.html

) t WHERE rn = 1;
来源：http://hz.snrcjt.cn/gtocembbmo.html

[Q35] 内连接
来源：http://hz.sufxvd.cn/gtahtyspxw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.aibaodan.cn/gtljoppyyc.html

[Q36] 左连接
来源：http://hz.jqgufenzy.top/gtoarsrckd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtaoxtuyfr.html

[Q37] 右连接
来源：http://hz.dashuyun.cn/gtwkwphjxo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhixingplan.top/gtblxstcfq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gtpitecrmi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtmmljmdkk.html

[Q39] 自连接（查上下级）
来源：http://hz.xziqi.cn/gtrzpquqhy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fzhhl.top/gtevvwdlzo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hfpthk.cn/gtpdfnivit.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xinyue.icu/gtdlquylyq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sysykeji.top/gthbgiapce.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gtlwnghceq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xinyue.icu/gtoncfktbg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shangyingyoupin.top/gtbjffkhbs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtuttmiqay.html

[Q42] 连接条件附加过滤
来源：http://hz.zhengqikj.top/gtvmzbrtex.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ivvv.top/gtjdvmsaoq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydzc1.top/gttoeihupn.html

[Q43] 标量子查询
来源：http://hz.nanxinkj.top/gtehdddbwm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.mhx1999.top/gtylqmhjjb.html

[Q44] IN 子查询
来源：http://hz.wangshuangyany.cn/gtawscpvzt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aizwys.cn/gtakgnbeye.html

[Q45] EXISTS 判断存在
来源：http://hz.xylfe.cn/gtjiefnybn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtarkljygx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fzhhl.top/gtgkuwsjgb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtlgwiucph.html

[Q47] 与平均值比较
来源：http://hz.316326.xyz/gtxkaavmip.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.pycfn.com/gtowgarqzb.html

[Q48] CTE 公用表表达式
来源：http://hz.zhengqikj.top/gtmpkwhbod.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gtezdtsbvx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yueranfly.top/gtbmjrpfpp.html

[Q49] 更新单行
来源：http://hz.bjfxy.top/gtgedwswva.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtiuejglbq.html

[Q50] 批量更新
来源：http://hz.quarkkingdee.top/gtvaaevxqt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cucudq.cn/gtdnybrffx.html

[Q51] 用子查询更新
来源：http://hz.xuanzx.com/gtvymfdvdy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sxryk.cn/gtvguvbhyk.html

[Q52] 删除指定行
来源：http://hz.jinqigfzy.top/gttqrabpws.html

DELETE FROM users WHERE id = 10;
来源：http://hz.guowangkeji.top/gtldbxnydw.html

[Q53] 按条件删除
来源：http://hz.52xcode.cn/gtaafuxhod.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jianghu66.top/gthnqyalic.html

[Q54] 清空表
来源：http://hz.cucudq.cn/gtsujudaph.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gterynvvch.html

[Q55] 排名（并列占位）
来源：http://hz.yj20258888.top/gtuiwxytev.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuxming.cn/gtaepvhjnh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gogol.net.cn/gtvnjdhwec.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jianghu66.top/gtarjchdnx.html

[Q57] 行号
来源：http://hz.zhaomingkeji.xyz/gtjrgelvgn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daria6918.cn/gtwxyinsxk.html

[Q58] 累计求和
来源：http://hz.tian-w.cn/gtgacivvmm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dashuyun.cn/gtctflxwxo.html

[Q59] 分组内累计
来源：http://hz.jinqigfzy.top/gtyukpejqe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxuanxn.top/gtejelyhyx.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gtdzepoynv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hongshengwenyu.top/gtuparfcol.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jyoumei.cn/gtswnozqva.html

[Q61] 移动平均
来源：http://hz.wangshuangyany.cn/gtgbjkeyxv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtqnfofmyc.html

[Q62] 分组占比
来源：http://hz.xylfe.cn/gtstxfetnq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtythhyqiv.html

[Q63] 开启事务
来源：http://hz.sysykeji.top/gtgrrwanmh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hywenlv.cn/gtqwtvwcym.html

[Q64] 提交事务
来源：http://hz.ybcxt.top/gtftodighk.html

COMMIT;
来源：http://hz.daria6918.cn/gtnmjzgrnz.html

[Q65] 回滚事务
来源：http://hz.zhixingplan.top/gtjcetfxij.html

ROLLBACK;
来源：http://hz.pycfn.com/gtkiqqbyjm.html

[Q66] 行锁查询
来源：http://hz.guannengcc.top/gtnsqfavgo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtkwftwziy.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtkwamahfz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hysaishi.cn/gtztizlrgg.html

[Q68] 保存点
来源：http://hz.wangdashe.top/gtbumcivzo.html

SAVEPOINT sp1;
来源：http://hz.redwolf501.top/gtngtgwowr.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gtybqaotwt.html

[Q69] 查看执行计划
来源：http://hz.jqgufenzy.top/gtejxqxgqj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgfzy.top/gtlcsbzofk.html

[Q70] 更新统计信息
来源：http://hz.yanxiufei.cn/gtmsojnmxg.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gtrgphcolr.html

[Q71] 查看建表语句
来源：http://hz.guowangkeji.top/gtbnqgpqeq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jyoumei.cn/gtwgwqolsp.html

[Q72] 查看索引
来源：http://hz.shanyushiyangkeji.top/gtylpfpwyd.html

SHOW INDEX FROM users;
来源：http://hz.yanxiufei.cn/gtrszbudqr.html

[Q73] 查看表状态
来源：http://hz.316326.xyz/gtomcbwluk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtcqsjarwx.html

[Q74] 强制使用索引
来源：http://hz.yuanzhike.top/gtvhcskabl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenjidiqi.icu/gtbxvnshla.html

[Q75] 日期格式化
来源：http://hz.kuanghao11.cn/gtjzakyclu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.9152youxi.cn/gthenpjwgw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gttjyhyjkc.html

[Q76] 按天统计
来源：http://hz.jiagoushi.top/gtckgsnzra.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yueranfly.top/gteappxkzh.html

[Q77] 时间加减
来源：http://hz.meibo888.top/gtckjamaek.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinqigufen.top/gtiahkoupw.html

[Q78] 当前时间
来源：http://hz.yuanzhike.top/gttehsimgv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gtdmlusvun.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtwbfjnstn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinyuanbaomall.cn/gtjqjoikwe.html

[Q80] 字符串截取
来源：http://hz.feifeiyinyue.top/gtrzhazhur.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigufen.top/gtojzmqwve.html

[Q81] 字符串替换
来源：http://hz.nanxuanxn.top/gtcrdfiltg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtkvokeqgr.html

[Q82] 字符长度与字节长度
来源：http://hz.mhx1999.top/gtpxpddamv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydzc1.top/gtkunntqym.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtaegcfxfa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fzhhl.top/gtllzirjdz.html

[Q84] 去除首尾空格
来源：http://hz.yj20258.top/gtmnbfolxk.html

SELECT TRIM(name) FROM users;
来源：http://hz.tian-w.cn/gtxzpxybvm.html

[Q85] 数值取整
来源：http://hz.hammf.cn/gtjdlermsf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cheryme.top/gtzeuwfelq.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtbtjuzyll.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxinkj.top/gtbcbhvsbx.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gtgemzowpv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhoulong.xyz/gtzfgpecqr.html

[Q88] 行转列（条件聚合）
来源：http://hz.xinyue.icu/gthkcjvqlb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gtgbjunzkx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yonumen.top/gthqiorghi.html

[Q89] 判断表是否存在
来源：http://hz.svipenyu.cn/gtrimareiz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jlsjyb.cn/gtbbhgdyck.html

[Q90] 生成序号列
来源：http://hz.yuanzhike.top/gtxfhepvea.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gtjczmmwva.html

================================================================================
来源：http://hz.fengsongda.top/gtybnggvbl.html

R. Bash 专题
来源：http://hz.jinyuanbaomall.cn/gtstlaedsv.html

================================================================================
来源：http://hz.jqgfzy.top/gthgcfwnkn.html

[R01] shebang 与严格模式
来源：http://hz.cashguo.top/gtrzmztwnu.html

#!/usr/bin/env bash
来源：http://hz.zycfv.cn/gthsjrwpag.html

set -euo pipefail
来源：http://hz.yj20258.top/gtdzzgtjwq.html

[R02] 变量赋值与使用
来源：http://hz.aizwys.cn/gtbzxhzgmd.html

name="Tom"; echo "$name"
来源：http://hz.yanxiufei.cn/gtlnwdyphr.html

[R03] 只读变量
来源：http://hz.ydjk.org.cn/gtoagdqrsk.html

readonly PI=3.14
来源：http://hz.ivvv.top/gtlmmfyery.html

[R04] 位置参数
来源：http://hz.hfpthk.cn/gtxiulnvoz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hysaishi.cn/gtzafsrilu.html

[R05] 参数默认值
来源：http://hz.zhijiandao.cn/gtecgaayrp.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gtkfgsjowy.html

[R06] 判断命令是否存在
来源：http://hz.jlsjyb.cn/gtsxsdtuxt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtzajsfazv.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtftjtwgkz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtlbsfhlpy.html

[R08] 数值比较
来源：http://hz.xuanzx.com/gtmizogngd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.andypj.xyz/gtvpljowgx.html

[R09] 字符串比较
来源：http://hz.shangyingyoupin.top/gtwwhxauvh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fengsongda.top/gtrucyeyky.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtanaisyug.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tianlin.xyz/gtsobxuuwg.html

[R11] case 多分支
来源：http://hz.ydjk.org.cn/gtrupvtsrk.html

case "$1" in
来源：http://hz.ydzc1.top/gthalkljje.html

start) echo "启动" ;;
来源：http://hz.ppjwa.cn/gtltsuazpq.html

stop)  echo "停止" ;;
来源：http://hz.bjfxy.top/gtevarafhj.html

*)     echo "未知命令" ;;
来源：http://hz.cheryme.top/gtjdpfhqjx.html

esac
来源：http://hz.ywan-chungtsiang.top/gtcfslnkto.html

[R12] for 遍历文件
来源：http://hz.xylfe.cn/gtgvodxbyh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinyuanbaomall.cn/gtascwgvkz.html

[R13] for 计数循环
来源：http://hz.kuanghao11.cn/gtcqhrtzwk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gttrrszfwm.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtubfdjonm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yuxming.cn/gtueiuvqbv.html

[R15] while 逐行读文件
来源：http://hz.zhiwuduotai.top/gtjnrkulte.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gtugwecjts.html

[R16] until 等待条件
来源：http://hz.nanxuanxn.top/gtukblwexp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shzxlz.cn/gtpodppjpu.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gtngkugdjg.html


<!-- 参考信息 -->