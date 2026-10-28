代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dianchejie.cn/gtnyznwjjm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtxxtrvsax.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtzzwpqvlg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtxldflqjb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gtwqetakel.html

Go:   len(arr);  len(m)
来源：http://hz.kuanghao11.cn/gtbthbgoko.html

Ruby: x.length;  x.size
来源：http://hz.tanke756.top/gtjpjxwsyi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shzxlz.cn/gtvklphlpr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuetiantiany.cn/gtjakfhkjy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tianlin.xyz/gtpvexpfhy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuanzx.com/gtotkathqo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhiwuduotai.top/gtldashwgj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtzqrbygmf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shuidangran.top/gthgfqxrdl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gteijgpupq.html

Ruby: a == b
来源：http://hz.yongpay.top/gtfzgufqnr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cashguo.top/gtmjofhyuy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.vqdsnc.cn/gtggxgruwg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cheryme.top/gtdderfxwt.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtcyzcxuip.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jianghu66.top/gttyhnmnaq.html

TS:   if (x == null) {}
来源：http://hz.ydjk.org.cn/gthritrpga.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtnjyiglug.html

Go:   if x == nil {}
来源：http://hz.hysaishi.cn/gtmtmgjgfk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gtqwedxrgl.html

C#:   if (x is null) {}
来源：http://hz.nanxuanxn.top/gtnoftsrcm.html

[P07] 防抖与节流
来源：http://hz.redwolf501.top/gtwvpihbdx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xuanzx.com/gtxfcukfwk.html

PHP:  // 手写时间戳比较
来源：http://hz.yuanzhike.top/gtgvongaws.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtdgituqtn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtdyxkzhvz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinghuilouyu.cn/gtukwllbjv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangdashe.top/gtxpinawjz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenlongwang.top/gtkekmtoqy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jiagoushi.top/gtkvwvxsge.html

[P08] 处理浮点精度问题
来源：http://hz.dianchejie.cn/gtkwrjlgcg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ppjwa.cn/gtppvthghq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtfwurayqm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xinyue.icu/gteuzgsltq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shzxlz.cn/gttxholwol.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tian-w.cn/gtcmqpgbox.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zycfv.cn/gtmcclyggf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zdqjudy.top/gtcdoezvei.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sxryk.cn/gtzrqkbbxq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwfzxlenm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.guannengcc.top/gtrqrptrry.html

================================================================================
来源：http://hz.meibo888.top/gtxtgtbrgs.html

[Q01] 创建表
来源：http://hz.ivvv.top/gtmeetvqgo.html

CREATE TABLE users (
来源：http://hz.redwolf501.top/gtnjkcjabi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtenhxledm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guowangkeji.top/gtjbledudh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydjk.org.cn/gtpixjyieg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuetiantiany.cn/gtgtnqotvp.html

);
来源：http://hz.zhiwuduotai.top/gtsewswgss.html

[Q02] 创建带外键的表
来源：http://hz.meibo888.top/gtwtaqcczk.html

CREATE TABLE orders (
来源：http://hz.xziqi.cn/gthbxxukry.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtkemoenrg.html

user_id INT NOT NULL,
来源：http://hz.shzxlz.cn/gtbspcwscm.html

amount DECIMAL(10, 2),
来源：http://hz.316326.xyz/gtsqkmhxdm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtmddmiudc.html

);
来源：http://hz.haohaochexian.top/gtyokyuukr.html

[Q03] 增加列
来源：http://hz.chenzaomai.com/gtwnjdzfqc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtjpmogsfg.html

[Q04] 修改列类型
来源：http://hz.ybcxt.top/gtefkflemd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xinyue.icu/gtltlwtbey.html

[Q05] 重命名列
来源：http://hz.hnxiangtu.top/gtidbikmbr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinyuanbaomall.cn/gtpdckrjhi.html

[Q06] 删除列
来源：http://hz.chenjidiqi.icu/gtlfnbnodp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydjk.org.cn/gtzxyssduc.html

[Q07] 删除表
来源：http://hz.jinqigufen.top/gtrqjlirkk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtpxklgpeb.html

[Q08] 创建普通索引
来源：http://hz.jinqigfzy.top/gteccxmkop.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtqzeozdnk.html

[Q09] 创建唯一索引
来源：http://hz.jlsjyb.cn/gtidjdbzlc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtknlnezgc.html

[Q10] 插入单行
来源：http://hz.xuanzx.com/gtkhwblzfs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenzaomai.com/gtudacpdqm.html

[Q11] 一次插入多行
来源：http://hz.yvedp.cn/gtwvjrtszt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nwbrower.top/gtiwhtyziq.html

[Q12] 插入后取自增 ID
来源：http://hz.cucudq.cn/gtvvxntoga.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nanxinkj.top/gtjnixjcjz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhixingplan.top/gtopgoojyz.html

[Q13] 忽略重复插入
来源：http://hz.tanke756.top/gtpcjszqco.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.snrcjt.cn/gtejdljbzb.html

[Q14] 存在则更新（upsert）
来源：http://hz.ppjwa.cn/gtpowwxjva.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.birdmap.top/gtjjfcsgop.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gttmhdgzqt.html

[Q15] 查询全部
来源：http://hz.xinyue.icu/gtqggecuwy.html

SELECT * FROM users;
来源：http://hz.sweek.top/gtpgrpeuto.html

[Q16] 查询指定列
来源：http://hz.zycfv.cn/gtbtmknjgg.html

SELECT id, name FROM users;
来源：http://hz.bjfxy.top/gtvyzmivpc.html

[Q17] 条件查询
来源：http://hz.jinyuanbaomall.cn/gtrfqljnha.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.snrcjt.cn/gtgkjfwign.html

[Q18] 模糊匹配
来源：http://hz.hammf.cn/gtgbklsrsq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fengsongda.top/gtdpuzxomp.html

[Q19] 范围查询
来源：http://hz.jinqigufen.top/gtoynckvoh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cdnleiting.top/gtdphnjtae.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtunovudxv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yangfankeji.com/gtgkoqpnoz.html

[Q21] 空值判断
来源：http://hz.smart0.xyz/gtsnxbwqoi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.feifeiyinyue.top/gtjkuqevfd.html

[Q22] 排序
来源：http://hz.jyoumei.cn/gtubzdwdmm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtahnywngs.html

[Q23] 分页
来源：http://hz.gotoacloud.top/gtylgoyvno.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xinyue.icu/gtlcbchqcz.html

[Q24] 去重
来源：http://hz.daria6918.cn/gtjwpkxrsn.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenlongwang.top/gtsrezujdx.html

[Q25] 只取前 N 条
来源：http://hz.yanxiufei.cn/gtuqitxlit.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sxryk.cn/gteaalcaog.html

[Q26] 计数
来源：http://hz.jqgufenzy.top/gtxuigfmye.html

SELECT COUNT(*) FROM users;
来源：http://hz.aibaodan.cn/gtqjrwstvh.html

[Q27] 条件计数
来源：http://hz.ybcxt.top/gtgxqnvrhd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.svipenyu.cn/gtuseyvtlh.html

[Q28] 求和与平均
来源：http://hz.hywenlv.cn/gtfzdomxze.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtgomsvhyn.html

[Q29] 最大最小值
来源：http://hz.quarkkingdee.top/gthnpiyvka.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gtlnndmqoz.html

[Q30] 分组统计
来源：http://hz.jiagoushi.top/gtkwjldfrv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtohilgebs.html

[Q31] 分组后过滤
来源：http://hz.guannengcc.top/gtiasfvoiu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shzxlz.cn/gtpgxvqymy.html

[Q32] 分组拼接字符串
来源：http://hz.iojbl.cn/gtguqighhy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gttekuruch.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgufenzy.top/gtcdnsvgtw.html

[Q33] 多列分组
来源：http://hz.ydzc1.top/gtndfznxbz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.9152youxi.cn/gtqoxzzmpo.html

[Q34] 每组取第一条
来源：http://hz.yj20258.top/gtmujxjigw.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtfxjkbltw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.birdmap.top/gtosscwjlu.html

) t WHERE rn = 1;
来源：http://hz.gogol.net.cn/gtqsihdath.html

[Q35] 内连接
来源：http://hz.tanke756.top/gtdyrscewg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gtlxelasxj.html

[Q36] 左连接
来源：http://hz.cdnleiting.top/gtdeiqarrk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.52xcode.cn/gtbjootsfj.html

[Q37] 右连接
来源：http://hz.redwolf501.top/gtfvfudsgl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jianghu66.top/gtpyelaaaq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.mhx1999.top/gttlbvujno.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.0kj1m.cn/gtrqzwiybj.html

[Q39] 自连接（查上下级）
来源：http://hz.wangdashe.top/gtukvzakyf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cdnleiting.top/gtxcsngnfw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.snrcjt.cn/gtqneoegfv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gttnbuuvzw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dashuyun.cn/gtjcbdodjk.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gtrhblusbr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fengsongda.top/gtuazojjfh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydzc1.top/gtwigkqatw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtbzfisnqt.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgfzy.top/gtltcswxuk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pengpengdd.cyou/gtbhchwjsr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuanzx.com/gtrgvjpxfa.html

[Q43] 标量子查询
来源：http://hz.9152youxi.cn/gterruiroi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zycfv.cn/gtyywcwnnq.html

[Q44] IN 子查询
来源：http://hz.wangshuangyany.cn/gtbgfsrxyo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.52xcode.cn/gtrzdmlisa.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangtech.top/gtvbmlliik.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gttxzctrym.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.bjfxy.top/gtgzbjnvix.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtazaewipr.html

[Q47] 与平均值比较
来源：http://hz.ydjk.org.cn/gtihnmsxjn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shzxlz.cn/gtdnohttnv.html

[Q48] CTE 公用表表达式
来源：http://hz.ivvv.top/gtlhmlphgr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.smart0.xyz/gttwqwmuvz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydzc1.top/gtithvtkxn.html

[Q49] 更新单行
来源：http://hz.kuanghao11.cn/gtfpitnzzs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zycfv.cn/gtgvbqaywa.html

[Q50] 批量更新
来源：http://hz.daria6918.cn/gtltayjwol.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shangyingyoupin.top/gtqskflszp.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtyempymgh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zdqjudy.top/gtdaikypai.html

[Q52] 删除指定行
来源：http://hz.shzxlz.cn/gtbamxqduu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.9152youxi.cn/gtnvdohopt.html

[Q53] 按条件删除
来源：http://hz.havefunace.top/gtpskytysr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tanke756.top/gttitjqvpl.html

[Q54] 清空表
来源：http://hz.xingfuxueyuan.xyz/gtqgxumaqt.html

TRUNCATE TABLE logs;
来源：http://hz.zhiwuduotai.top/gtcaeiitqe.html

[Q55] 排名（并列占位）
来源：http://hz.yongpay.top/gtsfsrcmxk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.quarkkingdee.top/gthoundjun.html

[Q56] 密集排名（并列不占位）
来源：http://hz.dianchejie.cn/gtutwdlook.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gtlmzhymma.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtsibdxamz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gtsabzjtud.html

[Q58] 累计求和
来源：http://hz.snrcjt.cn/gtqmjqsfhd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinghuilouyu.cn/gtvpuwvqii.html

[Q59] 分组内累计
来源：http://hz.chenzaomai.com/gtqrlhsekq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.daria6918.cn/gtfjpgwhlz.html

[Q60] 取上一行 / 下一行
来源：http://hz.tanke756.top/gtshenqiot.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.svipenyu.cn/gtdswltqsd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ppjwa.cn/gtgbhxllyo.html

[Q61] 移动平均
来源：http://hz.yueranfly.top/gtxfxvqzgu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hongshengwenyu.top/gtpnqmnahm.html

[Q62] 分组占比
来源：http://hz.hfpthk.cn/gtcpcvbmmo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtiudbsqhf.html

[Q63] 开启事务
来源：http://hz.birdmap.top/gtgvhzycub.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.vqdsnc.cn/gtcbujhagm.html

[Q64] 提交事务
来源：http://hz.9152youxi.cn/gtwtegmsne.html

COMMIT;
来源：http://hz.xylfe.cn/gtvisqutqr.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtcfgszfhv.html

ROLLBACK;
来源：http://hz.guowangkeji.top/gtwyfyivyx.html

[Q66] 行锁查询
来源：http://hz.xuetiantiany.cn/gtuhzpqqri.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zycfv.cn/gtqtsmynov.html

[Q67] 设置隔离级别
来源：http://hz.hnxiangtu.top/gtzzbeutvr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258888.top/gtazwrgaqj.html

[Q68] 保存点
来源：http://hz.pycfn.com/gtzqxfpesy.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtpgcovrnl.html

ROLLBACK TO sp1;
来源：http://hz.cucudq.cn/gtorhqrkth.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtqhsykwem.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cucudq.cn/gtovriyotk.html

[Q70] 更新统计信息
来源：http://hz.52xcode.cn/gthtpdcfkg.html

ANALYZE TABLE users;
来源：http://hz.gzhubu.top/gtdgeayjll.html

[Q71] 查看建表语句
来源：http://hz.yvedp.cn/gtkohxpnhx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nanxinkj.top/gtponoovrx.html

[Q72] 查看索引
来源：http://hz.cashguo.top/gtexzffwau.html

SHOW INDEX FROM users;
来源：http://hz.zdqjudy.top/gtgrpejhed.html

[Q73] 查看表状态
来源：http://hz.316326.xyz/gtmresfxbv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shangyingyoupin.top/gtmchcogzv.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtrpdpqcji.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.svipenyu.cn/gtrcnzodbe.html

[Q75] 日期格式化
来源：http://hz.yongpay.top/gtlheeiefg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sweek.top/gtcphiuqvz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tianlin.xyz/gtmbatscfi.html

[Q76] 按天统计
来源：http://hz.iojbl.cn/gtrixpfmfy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigufen.top/gtfpvpviqt.html

[Q77] 时间加减
来源：http://hz.jiagoushi.top/gtkouiwgcm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hfpthk.cn/gtjpwpeazd.html

[Q78] 当前时间
来源：http://hz.zhongyouzk.top/gtppdpzpya.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zycfv.cn/gtfwkljelo.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtlhhfpcck.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangshuangyany.cn/gtdwsqdbxo.html

[Q80] 字符串截取
来源：http://hz.hongshengwenyu.top/gtuyxijmfa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.iojbl.cn/gtplnbayqz.html

[Q81] 字符串替换
来源：http://hz.feifeiyinyue.top/gtplizxmzl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xylfe.cn/gtmdermukm.html

[Q82] 字符长度与字节长度
来源：http://hz.haohaochexian.top/gtdsrbswuu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnqzz.top/gtzlfvateg.html

[Q83] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtrtmkipuw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtvmhtxlbf.html

[Q84] 去除首尾空格
来源：http://hz.pycfn.com/gtenffiaqh.html

SELECT TRIM(name) FROM users;
来源：http://hz.jlsjyb.cn/gtmakyxnpk.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtwptnjqke.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yangfankeji.com/gtcmzfgugw.html

[Q86] 读取 JSON 字段
来源：http://hz.cucudq.cn/gtpupiwiwk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ehwqpu.com/gtkojwbwqz.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangkeji.top/gtawdiovde.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangtech.top/gtuusqqibr.html

[Q88] 行转列（条件聚合）
来源：http://hz.ywan-chungtsiang.top/gttqxqfqkj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhijiandao.cn/gthiaqkaqc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtmcvqbnch.html

[Q89] 判断表是否存在
来源：http://hz.hysaishi.cn/gtvypspjmi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cqqwz.cn/gtgvohrgyq.html

[Q90] 生成序号列
来源：http://hz.fzhhl.top/gtmmrryvkb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigfzy.top/gtzebyokgm.html

================================================================================
来源：http://hz.yueranfly.top/gthxijvmfi.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gtmpbacjuc.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpmstldya.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gtzkupnnyb.html

#!/usr/bin/env bash
来源：http://hz.9152youxi.cn/gtoheshwrr.html

set -euo pipefail
来源：http://hz.sweek.top/gtinrtgiff.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtvxfcubts.html

name="Tom"; echo "$name"
来源：http://hz.zycfv.cn/gtsouygmyd.html

[R03] 只读变量
来源：http://hz.andypj.xyz/gtvlexjjgt.html

readonly PI=3.14
来源：http://hz.havefunace.top/gtlhmygxkq.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gtqwrtrtir.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhongyouzk.top/gttnqvwfeq.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtuvsdlhoo.html

name="${1:-default}"
来源：http://hz.shzxlz.cn/gtqawletbx.html

[R06] 判断命令是否存在
来源：http://hz.zhijiandao.cn/gtvucqrnrl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.quarkkingdee.top/gtapnxbdtf.html

[R07] if 判断文件
来源：http://hz.andypj.xyz/gtlwnjcyfo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aibaodan.cn/gtbifnoiau.html

[R08] 数值比较
来源：http://hz.zdqjudy.top/gtsaqirjnf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtmdcqgnzm.html

[R09] 字符串比较
来源：http://hz.zhongyouzk.top/gtqeagzdvf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuxming.cn/gtioqwkyjy.html

[R10] 正则匹配
来源：http://hz.wangdashe.top/gtswmrqxbc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yanxiufei.cn/gtijskaqoz.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gtthdpeghl.html

case "$1" in
来源：http://hz.yuanzhike.top/gtbohutqwx.html

start) echo "启动" ;;
来源：http://hz.cucudq.cn/gtpbygoyiq.html

stop)  echo "停止" ;;
来源：http://hz.chenlongwang.top/gtbmflbcrp.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gtzykruyuj.html

esac
来源：http://hz.xylfe.cn/gtzkhixtfo.html

[R12] for 遍历文件
来源：http://hz.ivvv.top/gtoaiabwxe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aizwys.cn/gtqukotnga.html

[R13] for 计数循环
来源：http://hz.shuidangran.top/gtebcrkhuc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zdqjudy.top/gteeggieyk.html

[R14] C 风格 for
来源：http://hz.ydzc1.top/gtaxzqpvmc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gzhubu.top/gtiqksoeqq.html

[R15] while 逐行读文件
来源：http://hz.chenjidiqi.icu/gtzslsmvzy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gtqmprjgis.html

[R16] until 等待条件
来源：http://hz.jinqigufen.top/gtywioujmu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guowangkeji.top/gtpwhlwnoc.html

[R17] 数组定义与取值
来源：http://hz.aibaodan.cn/gtpemqwwqe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhongyouzk.top/gtxtljkhgg.html

[R18] 遍历数组
来源：http://hz.ydzc1.top/gtpgpgahfl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gzhubu.top/gtrnnxoeci.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gtthbocuel.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtemdmttef.html

[R20] 关联数组（字典）
来源：http://hz.ppjwa.cn/gtrrjhqqaw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhixingplan.top/gthogfmsul.html

[R21] 字符串长度
来源：http://hz.yvedp.cn/gtzmavkrhk.html


<!-- 参考信息 -->