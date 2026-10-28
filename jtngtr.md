代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dashuyun.cn/gtroxcaffy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gticggnivi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.birdmap.top/gtximroynm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gteszjoelp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xinyue.icu/gtrhwuupgd.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtnyqsxgmn.html

Ruby: x.length;  x.size
来源：http://hz.wangdashe.top/gttsxsokwh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtplkgijrh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xylfe.cn/gtwnzttdjc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj202588.top/gtigatpdzc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yongpay.top/gtenptpyvi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtrzzjmoia.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shangyingyoupin.top/gtauvfjskf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.52xcode.cn/gtjcspitpd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yvedp.cn/gtuucnssum.html

Ruby: a == b
来源：http://hz.chenlongwang.top/gtbqdylzpa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhaomingkeji.xyz/gtlrpdgjsq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.snrcjt.cn/gtlzarugtf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hywenlv.cn/gttavzlldo.html

PHP:  if (empty($x)) {}
来源：http://hz.fengsongda.top/gtbcdwioqd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinghuilouyu.cn/gtpzuohigp.html

TS:   if (x == null) {}
来源：http://hz.redwolf501.top/gtmpdkpjqc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gtmrusjasr.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gtnqfycqnh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gotoacloud.top/gtecyyeogo.html

C#:   if (x is null) {}
来源：http://hz.xuetiantiany.cn/gtzvsblzvy.html

[P07] 防抖与节流
来源：http://hz.haohaochexian.top/gtbxmdgllo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jlsjyb.cn/gtngglxvsp.html

PHP:  // 手写时间戳比较
来源：http://hz.sxryk.cn/gtbjdeupjh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtuzsuwpiv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gtqwivffss.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sxryk.cn/gtwrsjodwr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.iojbl.cn/gtathfckhg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.quarkkingdee.top/gtpxkfooyg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ywan-chungtsiang.top/gtstpzsenc.html

[P08] 处理浮点精度问题
来源：http://hz.dianchejie.cn/gtulmbqvob.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gtsjhjwfgv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.bjfxy.top/gtoekoqeom.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydjk.org.cn/gthppxdnfl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtrwfntqnl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.andypj.xyz/gtykyagauj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgufenzy.top/gttmwksryl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinghuilouyu.cn/gtcbdiwjow.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zdqjudy.top/gtdteglkja.html

================================================================================
来源：http://hz.nanxinkj.top/gtstxfuvou.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daria6918.cn/gtjshtkhrx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtgyrpoabm.html

[Q01] 创建表
来源：http://hz.hysaishi.cn/gtsupcymvq.html

CREATE TABLE users (
来源：http://hz.sweek.top/gtukjttkve.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gtgfqvlfgd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenlongwang.top/gtykyssior.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigfzy.top/gtdukjkinm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenjidiqi.icu/gtslifxknp.html

);
来源：http://hz.hnxiangtu.top/gtwmmpysxt.html

[Q02] 创建带外键的表
来源：http://hz.xingfuxueyuan.xyz/gtydzehbdk.html

CREATE TABLE orders (
来源：http://hz.tian-w.cn/gtenlqjufv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtboyroskt.html

user_id INT NOT NULL,
来源：http://hz.ybcxt.top/gtpndamnoe.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258888.top/gtdusbbbsl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gzhubu.top/gtrvsoljdv.html

);
来源：http://hz.aizwys.cn/gtbmhsiidk.html

[Q03] 增加列
来源：http://hz.zhoulong.xyz/gtlkfumvwe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nwbrower.top/gtqowoqvsz.html

[Q04] 修改列类型
来源：http://hz.sweek.top/gtlxghfnve.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hnxiangtu.top/gtgkuasgjt.html

[Q05] 重命名列
来源：http://hz.ybcxt.top/gthddbkthq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.feifeiyinyue.top/gtbloyzars.html

[Q06] 删除列
来源：http://hz.cdnleiting.top/gtkymeugci.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cdnleiting.top/gtcttxhejn.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtbaoaxmlb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenlongwang.top/gtkcrbgpww.html

[Q08] 创建普通索引
来源：http://hz.zhixingplan.top/gtstnwcbya.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtrjwvzred.html

[Q09] 创建唯一索引
来源：http://hz.shanyushiyangkeji.top/gtuhtlkrqx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shuidangran.top/gtogmsnykx.html

[Q10] 插入单行
来源：http://hz.xuanzx.com/gtxojchjlh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.9152youxi.cn/gtrmexvlko.html

[Q11] 一次插入多行
来源：http://hz.sufxvd.cn/gttemciudb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jqgufenzy.top/gtmijwmuwv.html

[Q12] 插入后取自增 ID
来源：http://hz.nanxuanxn.top/gtilspneam.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhiwuduotai.top/gtkgsdzwyf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.9152youxi.cn/gtgdmuebgl.html

[Q13] 忽略重复插入
来源：http://hz.chenjidiqi.icu/gtkgyrmujf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangshuangyany.cn/gtmlpgbyux.html

[Q14] 存在则更新（upsert）
来源：http://hz.nanxuanxn.top/gtslhubwyj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnxiangtu.top/gttmfgoszr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.snrcjt.cn/gtserfqjdd.html

[Q15] 查询全部
来源：http://hz.zhiwuduotai.top/gtloibgufy.html

SELECT * FROM users;
来源：http://hz.ybcxt.top/gtbcrjfofh.html

[Q16] 查询指定列
来源：http://hz.chenzaomai.com/gtlhouqwzi.html

SELECT id, name FROM users;
来源：http://hz.ppjwa.cn/gtethulpxs.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtrndcnlub.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cheryme.top/gtczrghlcd.html

[Q18] 模糊匹配
来源：http://hz.vqdsnc.cn/gtmfbsynqj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yonumen.top/gtvecqmpxa.html

[Q19] 范围查询
来源：http://hz.gotoacloud.top/gtfmyplbbs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinghuilouyu.cn/gtkoamahvj.html

[Q20] IN 列表
来源：http://hz.yueranfly.top/gtjmhapafk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cdnleiting.top/gtogawzobg.html

[Q21] 空值判断
来源：http://hz.zhengqikj.top/gtibedzuxj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtrlrgfonl.html

[Q22] 排序
来源：http://hz.ivvv.top/gtdigfcnor.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hammf.cn/gtvwwejoir.html

[Q23] 分页
来源：http://hz.wangshuangyany.cn/gtwktudlsi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jianghu66.top/gtdrxotoxj.html

[Q24] 去重
来源：http://hz.gogol.net.cn/gttdsglfkd.html

SELECT DISTINCT city FROM users;
来源：http://hz.quarkkingdee.top/gtwdrkssjv.html

[Q25] 只取前 N 条
来源：http://hz.smart0.xyz/gtvqdamdvs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gtmdaeboba.html

[Q26] 计数
来源：http://hz.yanxiufei.cn/gtghzlcpzz.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gtepbnvgvd.html

[Q27] 条件计数
来源：http://hz.dashuyun.cn/gtbvvxukhk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zdqjudy.top/gtjsqckbue.html

[Q28] 求和与平均
来源：http://hz.tanke756.top/gtarfuqzms.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenjidiqi.icu/gtabrglfex.html

[Q29] 最大最小值
来源：http://hz.gaohongyu789.top/gtfuqvjqyn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.mhx1999.top/gtiktdhawc.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtpmedcmof.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtburxuobb.html

[Q31] 分组后过滤
来源：http://hz.ydzc1.top/gtqdbtwltu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.vqdsnc.cn/gtzjluhuhv.html

[Q32] 分组拼接字符串
来源：http://hz.nanxinkj.top/gtsyeiyjdv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtwnmmddyw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hongshengwenyu.top/gtygcahklx.html

[Q33] 多列分组
来源：http://hz.xuetiantiany.cn/gtusjnzgvp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gzhubu.top/gtzmuwkvmw.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtwjdtkleh.html

SELECT * FROM (
来源：http://hz.iojbl.cn/gtofmgbxjl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jyoumei.cn/gtcugfhhwa.html

) t WHERE rn = 1;
来源：http://hz.andypj.xyz/gttmoclfyo.html

[Q35] 内连接
来源：http://hz.sysykeji.top/gtxflnfbob.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtawuxnydj.html

[Q36] 左连接
来源：http://hz.yuanzhike.top/gtmesxwnhf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.52xcode.cn/gtsrsjxpam.html

[Q37] 右连接
来源：http://hz.ybcxt.top/gtmuhdpxfm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.9152youxi.cn/gtnefvetes.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.guowangkeji.top/gtlzgyebdt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sufxvd.cn/gtruuvlaxf.html

[Q39] 自连接（查上下级）
来源：http://hz.yuxming.cn/gtwgpfztui.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hywenlv.cn/gtfsomlbij.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.andypj.xyz/gtpodxtuuy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhengqikj.top/gtigtfawod.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tanke756.top/gtnlvqmlgb.html

[Q41] 多表连接
来源：http://hz.jqgfzy.top/gtewzkdlem.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gtuhalogbc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtydwpmtnx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gtkjvashnq.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxinkj.top/gtcubbneig.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jianghu66.top/gtukzgnvlc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.quarkkingdee.top/gtxvoebyav.html

[Q43] 标量子查询
来源：http://hz.pycfn.com/gtqnlfoojn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nanxuanxn.top/gtheemjmcx.html

[Q44] IN 子查询
来源：http://hz.yuxming.cn/gtjzrjkxyp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shangyingyoupin.top/gtudunlnle.html

[Q45] EXISTS 判断存在
来源：http://hz.hammf.cn/gtkzbgljce.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangdashe.top/gtseqvigqd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.c1oappe.top/gtvqyjgrig.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtwejtefmc.html

[Q47] 与平均值比较
来源：http://hz.vqdsnc.cn/gtxskhslbr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangshuangyany.cn/gtglgmeljc.html

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangtech.top/gtguyjwyum.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fzhhl.top/gtuzivcczc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fengsongda.top/gtfvkiuaac.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gtcwpplorn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yuxming.cn/gtesdziukp.html

[Q50] 批量更新
来源：http://hz.ehwqpu.com/gtnbmumnor.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cdnleiting.top/gtcpwsxhmb.html

[Q51] 用子查询更新
来源：http://hz.aibaodan.cn/gtfcehphqd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhixingplan.top/gtujremhja.html

[Q52] 删除指定行
来源：http://hz.andypj.xyz/gtxofuxjio.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nwbrower.top/gtmglebvwz.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtngnzenmo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yvedp.cn/gtrqpudtry.html

[Q54] 清空表
来源：http://hz.xylfe.cn/gtfqwzuzgz.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258.top/gtezqhwyop.html

[Q55] 排名（并列占位）
来源：http://hz.shzxlz.cn/gtoyorwfxk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ywan-chungtsiang.top/gtgcufmomp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenlongwang.top/gtydmcoslv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.c1oappe.top/gtoqhcubpn.html

[Q57] 行号
来源：http://hz.tian-w.cn/gtpjsctpkt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258888.top/gtavdboqxn.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gtkuekuvll.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sufxvd.cn/gtmroayeni.html

[Q59] 分组内累计
来源：http://hz.52xcode.cn/gtguwwkcdf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnxiangtu.top/gtladythgy.html

[Q60] 取上一行 / 下一行
来源：http://hz.tanke756.top/gtwrzzmztu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.aizwys.cn/gtksspjynf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.316326.xyz/gtskgamxwm.html

[Q61] 移动平均
来源：http://hz.tian-w.cn/gtvlphvjmu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cdnleiting.top/gtahmwirkt.html

[Q62] 分组占比
来源：http://hz.quarkkingdee.top/gtyfwkkndb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sweek.top/gtnrxtoxmn.html

[Q63] 开启事务
来源：http://hz.zhongyouzk.top/gtnuekotsg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tian-w.cn/gtewmbmihi.html

[Q64] 提交事务
来源：http://hz.cucudq.cn/gtghwahmyd.html

COMMIT;
来源：http://hz.ppjwa.cn/gtprjksqxw.html

[Q65] 回滚事务
来源：http://hz.cqqwz.cn/gtpzajdgud.html

ROLLBACK;
来源：http://hz.yangfankeji.com/gtwbdjmlcz.html

[Q66] 行锁查询
来源：http://hz.jinqigfzy.top/gtntasjfcq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtsxqklunk.html

[Q67] 设置隔离级别
来源：http://hz.cheryme.top/gttmptdxgs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gotoacloud.top/gtprdbxuci.html

[Q68] 保存点
来源：http://hz.xingfuxueyuan.xyz/gtpdteovtd.html

SAVEPOINT sp1;
来源：http://hz.316326.xyz/gtsgnarzgh.html

ROLLBACK TO sp1;
来源：http://hz.sxryk.cn/gttduunlnt.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gtypzrefne.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.svipenyu.cn/gtqkffphhz.html

[Q70] 更新统计信息
来源：http://hz.gaohongyu789.top/gtazzllnuy.html

ANALYZE TABLE users;
来源：http://hz.jlsjyb.cn/gtuhoicfmw.html

[Q71] 查看建表语句
来源：http://hz.zhijiandao.cn/gtregxhpgh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gtunwkimib.html

[Q72] 查看索引
来源：http://hz.yanxiufei.cn/gtcwichshe.html

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtegriwoif.html

[Q73] 查看表状态
来源：http://hz.ydjk.org.cn/gtzqswqtcv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tianlin.xyz/gtshxstgcd.html

[Q74] 强制使用索引
来源：http://hz.sweek.top/gtxzfapsie.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gtopegbsjp.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gtxalhyegi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daxiang520.top/gtlechmuht.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shuidangran.top/gtxaibcnal.html

[Q76] 按天统计
来源：http://hz.yongpay.top/gtgkoaooco.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jianghu66.top/gtncetwozo.html

[Q77] 时间加减
来源：http://hz.smart0.xyz/gtbnaydljb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhoulong.xyz/gtfkbjrele.html

[Q78] 当前时间
来源：http://hz.daria6918.cn/gtyizrcgll.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.andypj.xyz/gtbmtkuqxs.html

[Q79] 字符串拼接
来源：http://hz.kuanghao11.cn/gtxbfeekeh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.kuanghao11.cn/gtvcaotbei.html

[Q80] 字符串截取
来源：http://hz.gogol.net.cn/gtmqgofmhm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xylfe.cn/gtkhkhejey.html

[Q81] 字符串替换
来源：http://hz.cucudq.cn/gtedqutpkp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fzhhl.top/gtlindupam.html

[Q82] 字符长度与字节长度
来源：http://hz.316326.xyz/gtpmczdoxl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtbytxgwqz.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtapkpjrof.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtfazupixi.html

[Q84] 去除首尾空格
来源：http://hz.xinyue.icu/gtsorovxlb.html

SELECT TRIM(name) FROM users;
来源：http://hz.kuanghao11.cn/gtgiiduywt.html

[Q85] 数值取整
来源：http://hz.pycfn.com/gtlncxmnmn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gogol.net.cn/gtaetwuwhs.html

[Q86] 读取 JSON 字段
来源：http://hz.jiagoushi.top/gtflahavnj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sxryk.cn/gtkypmkych.html

[Q87] JSON 字段做条件
来源：http://hz.sxryk.cn/gttrgquwke.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj202588.top/gthhoctudo.html

[Q88] 行转列（条件聚合）
来源：http://hz.svipenyu.cn/gtxghfrrks.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yanxiufei.cn/gtaiyucvad.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtgxcqwxuv.html

[Q89] 判断表是否存在
来源：http://hz.jiagoushi.top/gtsgvphbrw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gtmakriumx.html

[Q90] 生成序号列
来源：http://hz.guannengcc.top/gthingldmp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jyoumei.cn/gtpblqpgcf.html

================================================================================
来源：http://hz.sufxvd.cn/gtfevkotkd.html

R. Bash 专题
来源：http://hz.tanke756.top/gtduwqzbmt.html

================================================================================
来源：http://hz.gzhubu.top/gtcjczfcmv.html

[R01] shebang 与严格模式
来源：http://hz.316326.xyz/gttpruuxek.html

#!/usr/bin/env bash
来源：http://hz.jiagoushi.top/gtnvwilkhq.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gtwfazncrw.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangtech.top/gtkoewpaqt.html

name="Tom"; echo "$name"
来源：http://hz.c1oappe.top/gtubznwhfb.html

[R03] 只读变量
来源：http://hz.gogol.net.cn/gtrdchgfae.html

readonly PI=3.14
来源：http://hz.wangshuangyany.cn/gtumbglxvg.html

[R04] 位置参数
来源：http://hz.aizwys.cn/gttisfdciz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gtkepgsbjh.html

[R05] 参数默认值
来源：http://hz.shanyushiyangtech.top/gtaeeypqry.html

name="${1:-default}"
来源：http://hz.yuanzhike.top/gtjuwbmygz.html

[R06] 判断命令是否存在
来源：http://hz.sufxvd.cn/gtsuekebsf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtrptasmnz.html

[R07] if 判断文件
来源：http://hz.pengpengdd.cyou/gtfezbpbkl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.birdmap.top/gtckqjjyrg.html

[R08] 数值比较
来源：http://hz.fengsongda.top/gtpqyjelis.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dianchejie.cn/gtcnonytuu.html

[R09] 字符串比较
来源：http://hz.chenlongwang.top/gtijrflijp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinyuanbaomall.cn/gthrkiwcov.html

[R10] 正则匹配
来源：http://hz.jinghuilouyu.cn/gtmugkkrow.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xingfuxueyuan.xyz/gtzodojiaq.html

[R11] case 多分支
来源：http://hz.ppjwa.cn/gtqpaaaafh.html

case "$1" in
来源：http://hz.aizwys.cn/gtnecubixh.html

start) echo "启动" ;;
来源：http://hz.hfpthk.cn/gtipksdklh.html

stop)  echo "停止" ;;
来源：http://hz.ywan-chungtsiang.top/gtsrbrcefs.html

*)     echo "未知命令" ;;
来源：http://hz.zycfv.cn/gthidlcahd.html

esac
来源：http://hz.svipenyu.cn/gtdtwedtka.html

[R12] for 遍历文件
来源：http://hz.nanxinkj.top/gtoombnwmx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.iojbl.cn/gtphlxkqtj.html

[R13] for 计数循环
来源：http://hz.wangdashe.top/gtxuzncnpi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenzaomai.com/gtkutfygnd.html

[R14] C 风格 for
来源：http://hz.yuxming.cn/gtqomhoppm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yangfankeji.com/gtkedasbak.html

[R15] while 逐行读文件
来源：http://hz.wangdashe.top/gtivtkyszn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sxryk.cn/gtzuzcniii.html

[R16] until 等待条件
来源：http://hz.jinqigfzy.top/gtoxyfnnms.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtvlgnwrpo.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gteqtcrows.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhengqikj.top/gtmbmhhufm.html

[R18] 遍历数组
来源：http://hz.jqgfzy.top/gtyvnkgcre.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydjk.org.cn/gtwmqdnbtg.html

[R19] 数组长度
来源：http://hz.hammf.cn/gtxokdimuh.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtouadpktu.html

[R20] 关联数组（字典）
来源：http://hz.andypj.xyz/gttbrdeirv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangshuangyany.cn/gtxlcyboir.html

[R21] 字符串长度
来源：http://hz.svipenyu.cn/gtmpsshgay.html


<!-- 参考信息 -->