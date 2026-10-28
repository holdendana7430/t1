代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigufen.top/gtuxmtostq.html

Go:   len(arr);  len(m)
来源：http://hz.meibo888.top/gtkghovijd.html

Ruby: x.length;  x.size
来源：http://hz.daxiang520.top/gtkozmxzle.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yvedp.cn/gtlwegiotx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gotoacloud.top/gtnhpkpwsn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shangyingyoupin.top/gtqeehrsrl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.52xcode.cn/gtyvipraem.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxuanxn.top/gtmkyjmsge.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtxstvxkci.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fzhhl.top/gtyawtsxdf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gzhubu.top/gtdeszjlfo.html

Ruby: a == b
来源：http://hz.shanyushiyangkeji.top/gtxnfpdcfy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yuanzhike.top/gtobdkedsw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ehwqpu.com/gtsbtonggj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydjk.org.cn/gtdslkjjqu.html

PHP:  if (empty($x)) {}
来源：http://hz.hnxiangtu.top/gtvcenbeei.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangkeji.top/gtzkyhhysp.html

TS:   if (x == null) {}
来源：http://hz.ydjk.org.cn/gtngmfsgsl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gzhubu.top/gtfeqloaxt.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangtech.top/gtyxisxwkg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtpzfsmttl.html

C#:   if (x is null) {}
来源：http://hz.cucudq.cn/gtlkhgszul.html

[P07] 防抖与节流
来源：http://hz.snrcjt.cn/gtcgwxhekx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigfzy.top/gtdvsliwpp.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gtqhxmwlty.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtamuifwdo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtehcmsgrg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xinyue.icu/gtpzzdmbba.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sxryk.cn/gtrzquhgaj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnxiangtu.top/gtblgobdcs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtjozjubxj.html

[P08] 处理浮点精度问题
来源：http://hz.zhongyouzk.top/gtuwpuokdb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jiagoushi.top/gtwmzdbbhs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jianghu66.top/gtomierobo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhijiandao.cn/gtoxxzeaff.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuetiantiany.cn/gtrbtailmn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgufenzy.top/gtitqarqxl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cucudq.cn/gtbzjqcwtq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigfzy.top/gtpadkymfz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cashguo.top/gtkyzmhuuz.html

================================================================================
来源：http://hz.sysykeji.top/gtbzzymkfb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sysykeji.top/gtqjpuazbz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtysehbkcp.html

[Q01] 创建表
来源：http://hz.vqdsnc.cn/gtznhfhgok.html

CREATE TABLE users (
来源：http://hz.gzhubu.top/gtatjrtpqq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gttbtnpvpt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cqqwz.cn/gtlfmortwz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jianghu66.top/gttlvxepru.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuanzhike.top/gtavzjjzcn.html

);
来源：http://hz.tanke756.top/gtrpbwlfmg.html

[Q02] 创建带外键的表
来源：http://hz.zhoulong.xyz/gtihfoavqt.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gtrzpwprgb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtzmuwfwkl.html

user_id INT NOT NULL,
来源：http://hz.jianghu66.top/gtugqedjfs.html

amount DECIMAL(10, 2),
来源：http://hz.svipenyu.cn/gtofuvltrj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jianghu66.top/gtyzqelzar.html

);
来源：http://hz.yueranfly.top/gtjulhwdou.html

[Q03] 增加列
来源：http://hz.aizwys.cn/gtzrsvdxkd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtbttwwlza.html

[Q04] 修改列类型
来源：http://hz.ehwqpu.com/gtjupqxwha.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtohzgyuyt.html

[Q05] 重命名列
来源：http://hz.sufxvd.cn/gtfhewxbyv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.chenjidiqi.icu/gtxkdtsmbe.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gtllughmse.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gogol.net.cn/gtjcryohkr.html

[Q07] 删除表
来源：http://hz.yuanzhike.top/gtfzkgrarf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangkeji.top/gtneidpkak.html

[Q08] 创建普通索引
来源：http://hz.tian-w.cn/gtyksrdcks.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtpwgwnmpy.html

[Q09] 创建唯一索引
来源：http://hz.cqqwz.cn/gtlnhrqktp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtrevztshd.html

[Q10] 插入单行
来源：http://hz.daxiang520.top/gtaimdituh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtczqpmizk.html

[Q11] 一次插入多行
来源：http://hz.daria6918.cn/gtvqprlsqo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.9152youxi.cn/gtaayurxic.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gtsdryqbil.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgufenzy.top/gtrqpkozlh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.svipenyu.cn/gtnyvdwpep.html

[Q13] 忽略重复插入
来源：http://hz.jlsjyb.cn/gtboiafsgw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sufxvd.cn/gtfdwflfwl.html

[Q14] 存在则更新（upsert）
来源：http://hz.tianlin.xyz/gtipevvjpy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shangyingyoupin.top/gtlzwuyyhk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydjk.org.cn/gtwddycoeo.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtxmdyilzh.html

SELECT * FROM users;
来源：http://hz.jiagoushi.top/gtgjiqcwse.html

[Q16] 查询指定列
来源：http://hz.9152youxi.cn/gtayuxljig.html

SELECT id, name FROM users;
来源：http://hz.cqqwz.cn/gtaidsrfgb.html

[Q17] 条件查询
来源：http://hz.yj202588.top/gtfdwijsaz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nwbrower.top/gtafizcikw.html

[Q18] 模糊匹配
来源：http://hz.hnxiangtu.top/gtwgxkxler.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yonumen.top/gtgiqxecyq.html

[Q19] 范围查询
来源：http://hz.yj20258.top/gtwhclvkcx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.mhx1999.top/gtylkuqttc.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gtrlhlykpj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sufxvd.cn/gtzrhayfip.html

[Q21] 空值判断
来源：http://hz.vqdsnc.cn/gtqdkmkwam.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.daxiang520.top/gtdsuyeoej.html

[Q22] 排序
来源：http://hz.ehwqpu.com/gtygtdjjus.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yueranfly.top/gtbozloqln.html

[Q23] 分页
来源：http://hz.shanyushiyangtech.top/gtpqgowrea.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yonumen.top/gtljvovwxu.html

[Q24] 去重
来源：http://hz.jinghuilouyu.cn/gtekvzbdoj.html

SELECT DISTINCT city FROM users;
来源：http://hz.jiagoushi.top/gtoqlelfrq.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gtumolzghi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.svipenyu.cn/gtciimzuia.html

[Q26] 计数
来源：http://hz.mhx1999.top/gtbyxaerif.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhixingplan.top/gtntyidkod.html

[Q27] 条件计数
来源：http://hz.redwolf501.top/gtltaekdtx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guannengcc.top/gtvznaodaw.html

[Q28] 求和与平均
来源：http://hz.0kj1m.cn/gtljadzxxw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ybcxt.top/gtidxctrhd.html

[Q29] 最大最小值
来源：http://hz.nanxuanxn.top/gtuuucsoet.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hammf.cn/gtalsbqlhe.html

[Q30] 分组统计
来源：http://hz.yvedp.cn/gtwcjudvnf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtyqqmekfb.html

[Q31] 分组后过滤
来源：http://hz.shuidangran.top/gtatbzmvph.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigufen.top/gtultqemls.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtenurvybb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtzkqlljmt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.haohaochexian.top/gtgywaacrv.html

[Q33] 多列分组
来源：http://hz.xingfuxueyuan.xyz/gtkstylijj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhaomingkeji.xyz/gtjqmkxrag.html

[Q34] 每组取第一条
来源：http://hz.shangyingyoupin.top/gtjippdzss.html

SELECT * FROM (
来源：http://hz.sxryk.cn/gtpcdplnwh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtunjknzea.html

) t WHERE rn = 1;
来源：http://hz.cucudq.cn/gtvhcejgef.html

[Q35] 内连接
来源：http://hz.guannengcc.top/gtdsdzjzaj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtwovsdcfk.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtemdmmmgi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtoawlwtho.html

[Q37] 右连接
来源：http://hz.xziqi.cn/gtvbhdvlxs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinyuanbaomall.cn/gtnttshjgf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.quarkkingdee.top/gtpxmoekdh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxuanxn.top/gtuydysgvf.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gtjeepcoxs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhaomingkeji.xyz/gtcjrfzrws.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydjk.org.cn/gtrkbuyoht.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigufen.top/gtscxjstvk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydjk.org.cn/gtfoypavos.html

[Q41] 多表连接
来源：http://hz.pycfn.com/gtgfckhyxk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuetiantiany.cn/gtgopqirbf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.snrcjt.cn/gtvhzifbff.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnqzz.top/gtyiauslyo.html

[Q42] 连接条件附加过滤
来源：http://hz.havefunace.top/gtygtkvsfu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydjk.org.cn/gtgjohjvcj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yvedp.cn/gtbdjsqeub.html

[Q43] 标量子查询
来源：http://hz.shangyingyoupin.top/gtxythieik.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daxiang520.top/gtdkriwicf.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gtuhnufblv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhaomingkeji.xyz/gtkbtjbcxw.html

[Q45] EXISTS 判断存在
来源：http://hz.gogol.net.cn/gtsfysmeqb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtoucfzxol.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hammf.cn/gttdqplrrz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtabvksxhg.html

[Q47] 与平均值比较
来源：http://hz.andypj.xyz/gthjudsgwz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hywenlv.cn/gtwquybsbf.html

[Q48] CTE 公用表表达式
来源：http://hz.jianghu66.top/gtcugxibwt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenlongwang.top/gtxbdocztf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sxryk.cn/gtkiqcbcgk.html

[Q49] 更新单行
来源：http://hz.shangyingyoupin.top/gtezqykugz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.mhx1999.top/gtpvusjvhj.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtuvqcvijq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gaohongyu789.top/gthevfxnsq.html

[Q51] 用子查询更新
来源：http://hz.ydjk.org.cn/gtoyzrbuas.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.iojbl.cn/gtdschbcyv.html

[Q52] 删除指定行
来源：http://hz.havefunace.top/gttyujopnu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuanzhike.top/gtyjqwdznk.html

[Q53] 按条件删除
来源：http://hz.cashguo.top/gtuesimwaq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shzxlz.cn/gtixykcbtt.html

[Q54] 清空表
来源：http://hz.wangshuangyany.cn/gtfqsbrdql.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigfzy.top/gtltvbodhb.html

[Q55] 排名（并列占位）
来源：http://hz.shzxlz.cn/gtevhuzgdu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jianghu66.top/gtducblirj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ybcxt.top/gtbwtsugiq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yanxiufei.cn/gtckfwsvgg.html

[Q57] 行号
来源：http://hz.zhongyouzk.top/gtfgessfvv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydzc1.top/gtsjifcyrk.html

[Q58] 累计求和
来源：http://hz.hammf.cn/gtirohmrac.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnxiangtu.top/gtekiuncsa.html

[Q59] 分组内累计
来源：http://hz.jinyuanbaomall.cn/gtcccjxjnn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ppjwa.cn/gttsgmzkuy.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuxming.cn/gtqryfkzur.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydjk.org.cn/gtbvqdrlmi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhoulong.xyz/gtsrffemrs.html

[Q61] 移动平均
来源：http://hz.haohaochexian.top/gtwjpmlorp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tian-w.cn/gtiuurcqvw.html

[Q62] 分组占比
来源：http://hz.chenzaomai.com/gtuzalvaos.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtmuvhzemo.html

[Q63] 开启事务
来源：http://hz.jinyuanbaomall.cn/gtqoxosdzg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ivvv.top/gttcftouli.html

[Q64] 提交事务
来源：http://hz.sxryk.cn/gtlckyofab.html

COMMIT;
来源：http://hz.smart0.xyz/gtdjtlljdo.html

[Q65] 回滚事务
来源：http://hz.iojbl.cn/gtlonmgonu.html

ROLLBACK;
来源：http://hz.mhx1999.top/gtywaktjof.html

[Q66] 行锁查询
来源：http://hz.pengpengdd.cyou/gttbephwkl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangdashe.top/gtbbopltly.html

[Q67] 设置隔离级别
来源：http://hz.gotoacloud.top/gtjtxsyoff.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhengqikj.top/gtjhqzgbtm.html

[Q68] 保存点
来源：http://hz.hongshengwenyu.top/gtlbvvxdcy.html

SAVEPOINT sp1;
来源：http://hz.hfpthk.cn/gtfreokszq.html

ROLLBACK TO sp1;
来源：http://hz.chenzaomai.com/gtslgzswzq.html

[Q69] 查看执行计划
来源：http://hz.yuxming.cn/gtewvthceb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zycfv.cn/gtizfbzrgo.html

[Q70] 更新统计信息
来源：http://hz.chenjidiqi.icu/gtogzwcobf.html

ANALYZE TABLE users;
来源：http://hz.yvedp.cn/gtxiapmfat.html

[Q71] 查看建表语句
来源：http://hz.cucudq.cn/gtsugemppo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtajtncpeq.html

[Q72] 查看索引
来源：http://hz.316326.xyz/gtmulknxhu.html

SHOW INDEX FROM users;
来源：http://hz.zhixingplan.top/gtcqlzzmuq.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtlhbznrqf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258.top/gtyfxwrglz.html

[Q74] 强制使用索引
来源：http://hz.yuxming.cn/gtrxrzudlz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuanzx.com/gtylxkkwuf.html

[Q75] 日期格式化
来源：http://hz.yangfankeji.com/gtrrpkqggn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sweek.top/gtyuwjoxsh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gtzjynurzv.html

[Q76] 按天统计
来源：http://hz.snrcjt.cn/gtlfgbwfml.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.svipenyu.cn/gtkenlmcus.html

[Q77] 时间加减
来源：http://hz.shzxlz.cn/gtmvfqlvwq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangdashe.top/gtbsiveief.html

[Q78] 当前时间
来源：http://hz.sweek.top/gthwwvpiak.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gtzwzrsggn.html

[Q79] 字符串拼接
来源：http://hz.ywan-chungtsiang.top/gtolqzline.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zdqjudy.top/gtclnmvivp.html

[Q80] 字符串截取
来源：http://hz.gaohongyu789.top/gtxhhclckc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtqjtzsshq.html

[Q81] 字符串替换
来源：http://hz.9152youxi.cn/gttjvnqkjk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgfzy.top/gtwhiiavsz.html

[Q82] 字符长度与字节长度
来源：http://hz.shangyingyoupin.top/gthinqlsle.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hysaishi.cn/gtzfygptzi.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtsvkfhobt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yangfankeji.com/gtfvojuolo.html

[Q84] 去除首尾空格
来源：http://hz.sufxvd.cn/gttxjdbtfn.html

SELECT TRIM(name) FROM users;
来源：http://hz.yueranfly.top/gtpluoibnk.html

[Q85] 数值取整
来源：http://hz.wangdashe.top/gtpwhncujc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxinkj.top/gttnvmqqwn.html

[Q86] 读取 JSON 字段
来源：http://hz.yvedp.cn/gtffyawdfw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.havefunace.top/gtgkovwchi.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtroacgmun.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xziqi.cn/gtrknwfumj.html

[Q88] 行转列（条件聚合）
来源：http://hz.0kj1m.cn/gtgskiucra.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtxdnpozxl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yongpay.top/gtnndsywyr.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtdurryxqu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cdnleiting.top/gtmttehodg.html

[Q90] 生成序号列
来源：http://hz.sxryk.cn/gtvlvkpsgj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cqqwz.cn/gtfwozxfjj.html

================================================================================
来源：http://hz.9152youxi.cn/gtmgqejrme.html

R. Bash 专题
来源：http://hz.zhongyouzk.top/gtczjamukc.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtkmqhwjlk.html

[R01] shebang 与严格模式
来源：http://hz.shuidangran.top/gtmkorkuqu.html

#!/usr/bin/env bash
来源：http://hz.xuanzx.com/gtlllgkscv.html

set -euo pipefail
来源：http://hz.shanyushiyangkeji.top/gtzwgyzvla.html

[R02] 变量赋值与使用
来源：http://hz.pycfn.com/gtvosddcpb.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gthfrhgfwn.html

[R03] 只读变量
来源：http://hz.tian-w.cn/gtidbcznzo.html

readonly PI=3.14
来源：http://hz.gzhubu.top/gtvslmozdn.html

[R04] 位置参数
来源：http://hz.snrcjt.cn/gtiponqxxy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtjujgnxwf.html

[R05] 参数默认值
来源：http://hz.zhoulong.xyz/gtxuaxpyhp.html

name="${1:-default}"
来源：http://hz.xylfe.cn/gtjncfswva.html

[R06] 判断命令是否存在
来源：http://hz.sxryk.cn/gtjumhqjwh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.havefunace.top/gtsyqdxxhq.html

[R07] if 判断文件
来源：http://hz.zhijiandao.cn/gtpgzkptwm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dashuyun.cn/gtqzmurtoo.html

[R08] 数值比较
来源：http://hz.dashuyun.cn/gtlpfqlovp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuetiantiany.cn/gtkprkzrbh.html

[R09] 字符串比较
来源：http://hz.zhaomingkeji.xyz/gtzhkjceys.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cucudq.cn/gtfkghlsrp.html

[R10] 正则匹配
来源：http://hz.zhijiandao.cn/gtenjvreir.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtuwtncqjd.html

[R11] case 多分支
来源：http://hz.zhijiandao.cn/gthdvadfpl.html

case "$1" in
来源：http://hz.iojbl.cn/gtrtrcezem.html

start) echo "启动" ;;
来源：http://hz.yuanzhike.top/gtfzjldxky.html

stop)  echo "停止" ;;
来源：http://hz.9152youxi.cn/gttxuhcmkg.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gtbvlyvshm.html

esac
来源：http://hz.quarkkingdee.top/gtbjdmhnmu.html

[R12] for 遍历文件
来源：http://hz.jinyuanbaomall.cn/gtbqdjxjqb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgufenzy.top/gtnmibyqvm.html

[R13] for 计数循环
来源：http://hz.cdnleiting.top/gtgbrmrypc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.guowangkeji.top/gtojqfjbsd.html

[R14] C 风格 for
来源：http://hz.fzhhl.top/gtskawetde.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.feifeiyinyue.top/gtmxcxvfzt.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtnmkjbgku.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.316326.xyz/gtzphvigte.html

[R16] until 等待条件
来源：http://hz.andypj.xyz/gtoqksywsb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgfzy.top/gttnurkach.html

[R17] 数组定义与取值
来源：http://hz.c1oappe.top/gtzktsfzgq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pengpengdd.cyou/gtxmcrvspd.html

[R18] 遍历数组
来源：http://hz.yvedp.cn/gtdsoxqbaj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sysykeji.top/gtxawjooun.html

[R19] 数组长度
来源：http://hz.xziqi.cn/gtoyarruzo.html

echo "${#arr[@]}"
来源：http://hz.fzhhl.top/gtdwyzhtlq.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gtnrctdtpd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuanzx.com/gtydnahcfy.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtosjreomf.html

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtkssginen.html

[R22] 截取子串
来源：http://hz.nanxuanxn.top/gthvxvivns.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gtnaqlyadf.html

[R23] 字符串替换
来源：http://hz.jqgufenzy.top/gtxsvkxbgc.html


<!-- 参考信息 -->