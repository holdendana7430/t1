代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxinkj.top/gtryszqlie.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daxiang520.top/gtwisspqzb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhoulong.xyz/gtlnegbohq.html

[P04] 求长度
来源：http://hz.xuanzx.com/gtmjwfisis.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxuanxn.top/gtefichrtj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtwvccehkt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtgezkfhuz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtydxftftj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cashguo.top/gtdskuvvpg.html

Go:   len(arr);  len(m)
来源：http://hz.jinqigfzy.top/gtnuzcakqf.html

Ruby: x.length;  x.size
来源：http://hz.zdqjudy.top/gttpukyvyp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ppjwa.cn/gtzffblzlx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.meibo888.top/gtzzssqvuh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gtvfnjyvsx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ybcxt.top/gtseyklhig.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gtzaormnyk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gtfoucdykx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gtvzhfpmzi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jianghu66.top/gthwntekyi.html

Ruby: a == b
来源：http://hz.ydzc1.top/gtjtbxxxak.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinyuanbaomall.cn/gthzibjema.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sweek.top/gtjzwflzbz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dianchejie.cn/gtatfitqqn.html

PHP:  if (empty($x)) {}
来源：http://hz.ywan-chungtsiang.top/gtxpejierr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gogol.net.cn/gtfycmpvrn.html

TS:   if (x == null) {}
来源：http://hz.birdmap.top/gtqfdabohc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuxming.cn/gtvslkshma.html

Go:   if x == nil {}
来源：http://hz.cucudq.cn/gtkmlcizyf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtfcdmxycf.html

C#:   if (x is null) {}
来源：http://hz.guannengcc.top/gtoxxvmabl.html

[P07] 防抖与节流
来源：http://hz.hysaishi.cn/gtrfqgqjxr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pengpengdd.cyou/gtpweavjjv.html

PHP:  // 手写时间戳比较
来源：http://hz.tanke756.top/gtlbgtjvwr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtvzrlyvtw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtqjlidthl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.birdmap.top/gthaomacar.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuanzx.com/gtpnrakjbu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hfpthk.cn/gtfhngkvtr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuanzhike.top/gtcyoapfxh.html

[P08] 处理浮点精度问题
来源：http://hz.jiagoushi.top/gtgdzjnmkc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258.top/gtnelsqrao.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.haohaochexian.top/gthpcrrfou.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnxiangtu.top/gtmtvtbtfw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xinyue.icu/gtqscwtgbk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shangyingyoupin.top/gtphahrotl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yuanzhike.top/gtcpaivwgz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258.top/gtphvlvdex.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hongshengwenyu.top/gtzrstyjpi.html

================================================================================
来源：http://hz.9152youxi.cn/gtarsscnwl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jqgufenzy.top/gtxtrgsdvb.html

================================================================================
来源：http://hz.hfpthk.cn/gtyvzkhgwb.html

[Q01] 创建表
来源：http://hz.shangyingyoupin.top/gtwznivgpl.html

CREATE TABLE users (
来源：http://hz.0kj1m.cn/gtdlgusjrf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtuabyewjd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daxiang520.top/gtjdlhmgbi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ehwqpu.com/gtuhzcsoda.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.c1oappe.top/gtwgqxsalx.html

);
来源：http://hz.wangdashe.top/gtvopezout.html

[Q02] 创建带外键的表
来源：http://hz.hammf.cn/gtgdoxgszo.html

CREATE TABLE orders (
来源：http://hz.chenzaomai.com/gtranjjqbp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtslbjnydo.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gthsqjyqfk.html

amount DECIMAL(10, 2),
来源：http://hz.birdmap.top/gtvdctyoif.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.daxiang520.top/gtuufkxwcg.html

);
来源：http://hz.xuetiantiany.cn/gtrqfpixcp.html

[Q03] 增加列
来源：http://hz.jiagoushi.top/gtyakuzdwl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.9152youxi.cn/gtgskdetsk.html

[Q04] 修改列类型
来源：http://hz.nwbrower.top/gtgnlyxxdo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jianghu66.top/gtvfseemzk.html

[Q05] 重命名列
来源：http://hz.chenlongwang.top/gtevsprjli.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhoulong.xyz/gtybrpazfm.html

[Q06] 删除列
来源：http://hz.cqqwz.cn/gtrarmwjyg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.quarkkingdee.top/gtefyrvcqr.html

[Q07] 删除表
来源：http://hz.daria6918.cn/gteogmvybz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xylfe.cn/gtnhktcyyd.html

[Q08] 创建普通索引
来源：http://hz.yj20258888.top/gtuafzqrgo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sweek.top/gtihiemxvw.html

[Q09] 创建唯一索引
来源：http://hz.fengsongda.top/gtcmzpseqz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtriyouajh.html

[Q10] 插入单行
来源：http://hz.hammf.cn/gtqgaejupm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tanke756.top/gtermugxkj.html

[Q11] 一次插入多行
来源：http://hz.dashuyun.cn/gtyvcvdgdn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.daria6918.cn/gtinfzuxyx.html

[Q12] 插入后取自增 ID
来源：http://hz.ydzc1.top/gtlguosoil.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258888.top/gtjkwtsfgq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gtznmqaesx.html

[Q13] 忽略重复插入
来源：http://hz.hammf.cn/gtxbdnjlnj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yonumen.top/gtvwahhnge.html

[Q14] 存在则更新（upsert）
来源：http://hz.hammf.cn/gtfeukaefg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtfvrdajdd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxuanxn.top/gtjdlpztym.html

[Q15] 查询全部
来源：http://hz.meibo888.top/gtujrvvxfi.html

SELECT * FROM users;
来源：http://hz.jinyuanbaomall.cn/gtpotoycnj.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtvqehjisn.html

SELECT id, name FROM users;
来源：http://hz.9152youxi.cn/gtjliamryr.html

[Q17] 条件查询
来源：http://hz.hnqzz.top/gtbwqjqwfg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daxiang520.top/gtuwrwhybr.html

[Q18] 模糊匹配
来源：http://hz.vqdsnc.cn/gtnqnwhhhe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydzc1.top/gttmrpvogi.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gthxobfnqc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zycfv.cn/gtrsxlpild.html

[Q20] IN 列表
来源：http://hz.xinyue.icu/gttnwavotg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yangfankeji.com/gtwnshjzrd.html

[Q21] 空值判断
来源：http://hz.hongshengwenyu.top/gtvzpzobyn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cucudq.cn/gtulhjdutr.html

[Q22] 排序
来源：http://hz.havefunace.top/gtvbfrvpbf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shanyushiyangkeji.top/gtirgemtjy.html

[Q23] 分页
来源：http://hz.havefunace.top/gtcuipykzl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenjidiqi.icu/gtonherazr.html

[Q24] 去重
来源：http://hz.chenzaomai.com/gtydglpeyy.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinyuanbaomall.cn/gteripdtpl.html

[Q25] 只取前 N 条
来源：http://hz.yj202588.top/gtabseoysz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.andypj.xyz/gtrekomypc.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtupyngwmb.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtbpulvxhx.html

[Q27] 条件计数
来源：http://hz.shanyushiyangkeji.top/gtwexajrgc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cqqwz.cn/gtwplpevtu.html

[Q28] 求和与平均
来源：http://hz.chenzaomai.com/gtgwemeqqg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.birdmap.top/gthehdbyvr.html

[Q29] 最大最小值
来源：http://hz.svipenyu.cn/gtmytktlan.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gtfbtcpwvm.html

[Q30] 分组统计
来源：http://hz.pengpengdd.cyou/gtkbadvshg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtqytkqfvg.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtftxghjgd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangtech.top/gtbneewvrf.html

[Q32] 分组拼接字符串
来源：http://hz.birdmap.top/gtuwjukemm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gthentspcb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenzaomai.com/gtuhbaqcal.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtsphcwzje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.haohaochexian.top/gtxblwzrrt.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtbxjruefl.html

SELECT * FROM (
来源：http://hz.dashuyun.cn/gtybkqyogb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yueranfly.top/gtqeyovhur.html

) t WHERE rn = 1;
来源：http://hz.daria6918.cn/gtoxinspzs.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtlyalktic.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtybjywfsj.html

[Q36] 左连接
来源：http://hz.zhongyouzk.top/gtxummmvbi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.52xcode.cn/gtshxpsgph.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtgpaolicb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtwlsasibc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.dianchejie.cn/gtftusrahf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.aizwys.cn/gtunlyontj.html

[Q39] 自连接（查上下级）
来源：http://hz.kuanghao11.cn/gtixqrmqhg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jlsjyb.cn/gtquxkpvbg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj202588.top/gtlyqrrnho.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gtjkfrhplc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.aizwys.cn/gteffuagqw.html

[Q41] 多表连接
来源：http://hz.jinghuilouyu.cn/gthrimmses.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jianghu66.top/gtpnivxstu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sysykeji.top/gtmnchtnwn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydjk.org.cn/gtnxyfinhw.html

[Q42] 连接条件附加过滤
来源：http://hz.jlsjyb.cn/gtpkqxbfxf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.haohaochexian.top/gtslhcrdpp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhengqikj.top/gtlfayftju.html

[Q43] 标量子查询
来源：http://hz.hammf.cn/gtuvplhtpn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xylfe.cn/gtackmkkju.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangkeji.top/gthdyymhbn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yonumen.top/gtdedgdhas.html

[Q45] EXISTS 判断存在
来源：http://hz.sxryk.cn/gtbrjcnlll.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtwzopnlri.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jianghu66.top/gtdeeuvhhd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtebuwwwkl.html

[Q47] 与平均值比较
来源：http://hz.chenjidiqi.icu/gtxvkdyagi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hywenlv.cn/gtdawacpgc.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigufen.top/gtewrixqnl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigufen.top/gtldztfmqf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pengpengdd.cyou/gtmnerravb.html

[Q49] 更新单行
来源：http://hz.hfpthk.cn/gtkpompvbg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj202588.top/gtmjatzuox.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtyhrlnbrv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangkeji.top/gtklrhrbvr.html

[Q51] 用子查询更新
来源：http://hz.c1oappe.top/gtwnxztsqk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yvedp.cn/gtsejkecah.html

[Q52] 删除指定行
来源：http://hz.yangfankeji.com/gttxcrmnov.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gzhubu.top/gtlfelirtp.html

[Q53] 按条件删除
来源：http://hz.nanxinkj.top/gtnjackxjb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtxgamykpq.html

[Q54] 清空表
来源：http://hz.guowangkeji.top/gtxzypsvvs.html

TRUNCATE TABLE logs;
来源：http://hz.shangyingyoupin.top/gtiwoqeetd.html

[Q55] 排名（并列占位）
来源：http://hz.mhx1999.top/gtjrhdugdv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.birdmap.top/gtpjsjblgv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhiwuduotai.top/gtqjuadktr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtintpaado.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gtrftpjbpm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhoulong.xyz/gtmmqxwrbm.html

[Q58] 累计求和
来源：http://hz.xziqi.cn/gtlgzmfjed.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jlsjyb.cn/gtwbxulvix.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gtboifqdnj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gotoacloud.top/gtpljfhmzl.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gtwzjosfwb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cheryme.top/gtglddoqoe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangshuangyany.cn/gtbkjlqcfu.html

[Q61] 移动平均
来源：http://hz.ybcxt.top/gthmvlierp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gtukdpukjo.html

[Q62] 分组占比
来源：http://hz.zhijiandao.cn/gtykgnhaqr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtkfdreish.html

[Q63] 开启事务
来源：http://hz.shuidangran.top/gttswwwhrw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.birdmap.top/gtdsbpwtgw.html

[Q64] 提交事务
来源：http://hz.hywenlv.cn/gtolevofnf.html

COMMIT;
来源：http://hz.yongpay.top/gtkcmxxqpd.html

[Q65] 回滚事务
来源：http://hz.pengpengdd.cyou/gtdvnhzevh.html

ROLLBACK;
来源：http://hz.birdmap.top/gtkladoutz.html

[Q66] 行锁查询
来源：http://hz.kuanghao11.cn/gtzoifqkag.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ywan-chungtsiang.top/gtekuicxwj.html

[Q67] 设置隔离级别
来源：http://hz.wangshuangyany.cn/gtnfkhuhfb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gtafqppnvf.html

[Q68] 保存点
来源：http://hz.hnqzz.top/gtvufomphj.html

SAVEPOINT sp1;
来源：http://hz.zhiwuduotai.top/gtfchhuies.html

ROLLBACK TO sp1;
来源：http://hz.jianghu66.top/gtltmmlnaz.html

[Q69] 查看执行计划
来源：http://hz.zhixingplan.top/gtisamiirc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zycfv.cn/gtwhufceaz.html

[Q70] 更新统计信息
来源：http://hz.shuidangran.top/gtzidjfeat.html

ANALYZE TABLE users;
来源：http://hz.ivvv.top/gtnkmurahu.html

[Q71] 查看建表语句
来源：http://hz.zycfv.cn/gtjjjymtto.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gtonphirvr.html

[Q72] 查看索引
来源：http://hz.gaohongyu789.top/gtooxiczoc.html

SHOW INDEX FROM users;
来源：http://hz.yanxiufei.cn/gtylehvqmn.html

[Q73] 查看表状态
来源：http://hz.svipenyu.cn/gtyqmwdjwu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.feifeiyinyue.top/gtavaieeqo.html

[Q74] 强制使用索引
来源：http://hz.jqgfzy.top/gtsdvepqvu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.wangdashe.top/gtfaqajynt.html

[Q75] 日期格式化
来源：http://hz.nwbrower.top/gtuqvwopvo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nwbrower.top/gtmdgmvcuq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhiwuduotai.top/gtldwqfyip.html

[Q76] 按天统计
来源：http://hz.shanyushiyangkeji.top/gtwtogmavk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnqzz.top/gtukpuelbg.html

[Q77] 时间加减
来源：http://hz.yueranfly.top/gtctocduna.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.birdmap.top/gtjytmxmff.html

[Q78] 当前时间
来源：http://hz.gogol.net.cn/gtqdrwxeyg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangshuangyany.cn/gtbxvoztnj.html

[Q79] 字符串拼接
来源：http://hz.xuetiantiany.cn/gtbaqwzdnn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ywan-chungtsiang.top/gtwecxwbcn.html

[Q80] 字符串截取
来源：http://hz.tianlin.xyz/gtblcwhkxk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gogol.net.cn/gtfpijfpnz.html

[Q81] 字符串替换
来源：http://hz.ivvv.top/gtsitrdfgb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hongshengwenyu.top/gtvpuiipoo.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgufenzy.top/gtnrougyfm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.smart0.xyz/gttauercba.html

[Q83] 大小写转换
来源：http://hz.gotoacloud.top/gtbxnmtxgk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.316326.xyz/gtbbahhfzc.html

[Q84] 去除首尾空格
来源：http://hz.0kj1m.cn/gtzjhqnznk.html

SELECT TRIM(name) FROM users;
来源：http://hz.zycfv.cn/gtqawrhtct.html

[Q85] 数值取整
来源：http://hz.ydzc1.top/gtyhuikcay.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xingfuxueyuan.xyz/gtlkrxmksa.html

[Q86] 读取 JSON 字段
来源：http://hz.c1oappe.top/gtxoczbmag.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cdnleiting.top/gthxkzskdv.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigufen.top/gtjyqaoxhf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtfpeecwbc.html

[Q88] 行转列（条件聚合）
来源：http://hz.ywan-chungtsiang.top/gtjutqkwdh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.quarkkingdee.top/gtkwoqybha.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guowangkeji.top/gtbdkutqaa.html

[Q89] 判断表是否存在
来源：http://hz.hongshengwenyu.top/gtxeijufvj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.0kj1m.cn/gtqlvjcoim.html

[Q90] 生成序号列
来源：http://hz.sysykeji.top/gtweaxqtlp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ppjwa.cn/gttblfscis.html

================================================================================
来源：http://hz.zhengqikj.top/gtzntujucj.html

R. Bash 专题
来源：http://hz.jinghuilouyu.cn/gtcqrslncv.html

================================================================================
来源：http://hz.ivvv.top/gtygmuibqa.html

[R01] shebang 与严格模式
来源：http://hz.jinyuanbaomall.cn/gtmgxmqqzh.html

#!/usr/bin/env bash
来源：http://hz.jinqigufen.top/gtazbobfbo.html

set -euo pipefail
来源：http://hz.9152youxi.cn/gtzwxekflo.html

[R02] 变量赋值与使用
来源：http://hz.yuanzhike.top/gtprlbnmvw.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtbbrqbrrk.html

[R03] 只读变量
来源：http://hz.ppjwa.cn/gtjmlbwrkd.html

readonly PI=3.14
来源：http://hz.guannengcc.top/gtssqfmobo.html

[R04] 位置参数
来源：http://hz.tanke756.top/gtfshglyzm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangdashe.top/gtwbdbxkrv.html

[R05] 参数默认值
来源：http://hz.0kj1m.cn/gtwuihtksg.html

name="${1:-default}"
来源：http://hz.gotoacloud.top/gtzxleggpx.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtjrlqjvaj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zycfv.cn/gtvihtzxeq.html

[R07] if 判断文件
来源：http://hz.yuanzhike.top/gtjbjnnbys.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangkeji.top/gtvdzkoswy.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtlfcpkafo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.52xcode.cn/gtkjegznlp.html

[R09] 字符串比较
来源：http://hz.0kj1m.cn/gtzcszuapa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.meibo888.top/gtdbdbesnt.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gtffpfdkzq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cashguo.top/gtccnioadp.html

[R11] case 多分支
来源：http://hz.yj202588.top/gtclnapssl.html

case "$1" in
来源：http://hz.yj202588.top/gthkywaxii.html

start) echo "启动" ;;
来源：http://hz.kuanghao11.cn/gtrhzwtbxd.html

stop)  echo "停止" ;;
来源：http://hz.xingfuxueyuan.xyz/gtemhilyqn.html

*)     echo "未知命令" ;;
来源：http://hz.dashuyun.cn/gtkwxybjlm.html

esac
来源：http://hz.chenzaomai.com/gtdwllvrtd.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangtech.top/gtmdulwjqa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.redwolf501.top/gtdhzkrwfi.html

[R13] for 计数循环
来源：http://hz.kuanghao11.cn/gtnqxfrxdh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtblolffpy.html

[R14] C 风格 for
来源：http://hz.cashguo.top/gtzhobnfxe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.iojbl.cn/gtgrfkbmrs.html

[R15] while 逐行读文件
来源：http://hz.cdnleiting.top/gtaykvmqus.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgufenzy.top/gtvrxigzrn.html

[R16] until 等待条件
来源：http://hz.yueranfly.top/gtidkyjxjj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangshuangyany.cn/gtzuijmerx.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gttpplbyeu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jyoumei.cn/gtcitlxqsm.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtpvyofepn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hywenlv.cn/gtjfthjrxy.html

[R19] 数组长度
来源：http://hz.gogol.net.cn/gtoavipliw.html


<!-- 参考信息 -->