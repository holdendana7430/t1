代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.meibo888.top/gtuoibvjvv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.quarkkingdee.top/gthtjkmhbi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhixingplan.top/gtkjzaumpz.html

PHP:  if (empty($x)) {}
来源：http://hz.jyoumei.cn/gtxkqievta.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nwbrower.top/gtqpvyupsp.html

TS:   if (x == null) {}
来源：http://hz.shzxlz.cn/gtdxutnedl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xinyue.icu/gtnkvwgulu.html

Go:   if x == nil {}
来源：http://hz.xziqi.cn/gtdbsplved.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fzhhl.top/gtgpyrtpqh.html

C#:   if (x is null) {}
来源：http://hz.daria6918.cn/gtdnytqljy.html

[P07] 防抖与节流
来源：http://hz.gogol.net.cn/gttwephdzq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.quarkkingdee.top/gtppnxinqs.html

PHP:  // 手写时间戳比较
来源：http://hz.zhiwuduotai.top/gtfvfsygdh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtaafhmopc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtehlgqzid.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuxming.cn/gturcfvyrc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ywan-chungtsiang.top/gtanxbzwgi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuetiantiany.cn/gtstdhtbxr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhaomingkeji.xyz/gtobgzoygl.html

[P08] 处理浮点精度问题
来源：http://hz.c1oappe.top/gtgamitjfo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shuidangran.top/gtmlikzmae.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangdashe.top/gtrsqvfqiy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.smart0.xyz/gtihhvedog.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigufen.top/gtlxepteui.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.snrcjt.cn/gtdmlbdezt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnxiangtu.top/gtplitttqj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtgppnlsqf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gotoacloud.top/gtmrbupjrr.html

================================================================================
来源：http://hz.xziqi.cn/gtazhzwgol.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhijiandao.cn/gtgqeswhjr.html

================================================================================
来源：http://hz.9152youxi.cn/gtrthutqek.html

[Q01] 创建表
来源：http://hz.dianchejie.cn/gtdnpnrqbo.html

CREATE TABLE users (
来源：http://hz.shzxlz.cn/gtnuwzlnya.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtwpvokbkm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.feifeiyinyue.top/gtukovdiun.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhijiandao.cn/gtzdasomxo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cashguo.top/gtxvlwkzvq.html

);
来源：http://hz.ydzc1.top/gtfmsgefxb.html

[Q02] 创建带外键的表
来源：http://hz.cqqwz.cn/gtojezarlk.html

CREATE TABLE orders (
来源：http://hz.feifeiyinyue.top/gtxxxartbz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtefgtkffu.html

user_id INT NOT NULL,
来源：http://hz.hfpthk.cn/gtrreevuwg.html

amount DECIMAL(10, 2),
来源：http://hz.chenlongwang.top/gtkcfckmeq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ppjwa.cn/gtjbcqslyn.html

);
来源：http://hz.snrcjt.cn/gtitjjmphb.html

[Q03] 增加列
来源：http://hz.yj20258.top/gtpfiejmlo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinyuanbaomall.cn/gtoenaccri.html

[Q04] 修改列类型
来源：http://hz.nanxuanxn.top/gtryzttjhy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinghuilouyu.cn/gtdzzvylfh.html

[Q05] 重命名列
来源：http://hz.wangshuangyany.cn/gtndanzihp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.chenlongwang.top/gtpnpyoagl.html

[Q06] 删除列
来源：http://hz.fengsongda.top/gtkfgkjyyk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.mhx1999.top/gtxrvwuxia.html

[Q07] 删除表
来源：http://hz.wangshuangyany.cn/gtggrdnjmd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnxiangtu.top/gthdvodyof.html

[Q08] 创建普通索引
来源：http://hz.fzhhl.top/gtrsqstsly.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aizwys.cn/gtjodfnuvk.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtfykjosoo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtdurpgjyn.html

[Q10] 插入单行
来源：http://hz.yj20258.top/gtgmhreatu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gzhubu.top/gtwpudyqiw.html

[Q11] 一次插入多行
来源：http://hz.ydzc1.top/gtagdaewuf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xinyue.icu/gtazidrsfj.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtrpjhejmt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.meibo888.top/gtavprbhxl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinghuilouyu.cn/gtquywesrb.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gtbntxbrnx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.dianchejie.cn/gtdgeamjrk.html

[Q14] 存在则更新（upsert）
来源：http://hz.yonumen.top/gtfucesjyx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hongshengwenyu.top/gtqcyjqsyo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinyuanbaomall.cn/gtavyiwnab.html

[Q15] 查询全部
来源：http://hz.hammf.cn/gtdmgcwcgu.html

SELECT * FROM users;
来源：http://hz.xziqi.cn/gtnzxoaira.html

[Q16] 查询指定列
来源：http://hz.xylfe.cn/gtxgcptwtf.html

SELECT id, name FROM users;
来源：http://hz.hnqzz.top/gtkzcatyjh.html

[Q17] 条件查询
来源：http://hz.jianghu66.top/gtcpwwwxix.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cucudq.cn/gtkkrtsicl.html

[Q18] 模糊匹配
来源：http://hz.zhongyouzk.top/gtauoncoge.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ppjwa.cn/gtzryabjch.html

[Q19] 范围查询
来源：http://hz.nwbrower.top/gtfjknuykm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sxryk.cn/gtnqerewka.html

[Q20] IN 列表
来源：http://hz.jianghu66.top/gtjvnalvgd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yueranfly.top/gtxforfxkp.html

[Q21] 空值判断
来源：http://hz.nanxuanxn.top/gtxcmdjrqi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hnxiangtu.top/gtlzetsntt.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtwdkdaemg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.quarkkingdee.top/gtmqlublxl.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtznhoymdd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhiwuduotai.top/gtmfhumstw.html

[Q24] 去重
来源：http://hz.hysaishi.cn/gtwujahyfc.html

SELECT DISTINCT city FROM users;
来源：http://hz.feifeiyinyue.top/gtrznaasls.html

[Q25] 只取前 N 条
来源：http://hz.jinqigfzy.top/gtqvrgrcph.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258.top/gtqzuwcjid.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gtlopkuczh.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxinkj.top/gtbiyindsk.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtdonnguul.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shzxlz.cn/gttbwjxdav.html

[Q28] 求和与平均
来源：http://hz.hnqzz.top/gtpjenxunk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtmlrlgmol.html

[Q29] 最大最小值
来源：http://hz.nwbrower.top/gtrzqvqpcz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xinyue.icu/gtukpfgwwk.html

[Q30] 分组统计
来源：http://hz.yanxiufei.cn/gtczbgffwe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtskqlqldw.html

[Q31] 分组后过滤
来源：http://hz.hongshengwenyu.top/gtgdvvvgrq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daxiang520.top/gtarbahktm.html

[Q32] 分组拼接字符串
来源：http://hz.chenjidiqi.icu/gtdanjvvgs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.c1oappe.top/gtshgusczp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhixingplan.top/gtwygvgttr.html

[Q33] 多列分组
来源：http://hz.sweek.top/gteinwtcnd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtdjkgcffe.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtrueqannc.html

SELECT * FROM (
来源：http://hz.daxiang520.top/gtvzdrnibp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xingfuxueyuan.xyz/gtxcajsfld.html

) t WHERE rn = 1;
来源：http://hz.9152youxi.cn/gtslkouecg.html

[Q35] 内连接
来源：http://hz.yangfankeji.com/gtaqvjeppy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtlsopzdex.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtuueugrau.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtibqwmhgj.html

[Q37] 右连接
来源：http://hz.xylfe.cn/gtgzmsdamw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.haohaochexian.top/gtskpqtgqr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.aibaodan.cn/gtblficrfu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtkkoglktv.html

[Q39] 自连接（查上下级）
来源：http://hz.haohaochexian.top/gtzwwrbwjg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.feifeiyinyue.top/gtztduxvyp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aizwys.cn/gtchtxffgg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gtadvzvfav.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gzhubu.top/gtdttpfyxi.html

[Q41] 多表连接
来源：http://hz.meibo888.top/gtfixmsphx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.vqdsnc.cn/gtkdvoulva.html

JOIN users u ON u.id = o.user_id
来源：http://hz.mhx1999.top/gtarzbhtml.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yonumen.top/gtuybrllpm.html

[Q42] 连接条件附加过滤
来源：http://hz.hongshengwenyu.top/gtfflvnznq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.svipenyu.cn/gtjhoabjdo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhengqikj.top/gtnwncvhkq.html

[Q43] 标量子查询
来源：http://hz.yongpay.top/gtgsgjokwg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuetiantiany.cn/gtnjnwvuba.html

[Q44] IN 子查询
来源：http://hz.nanxinkj.top/gtkwvlfhdm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuetiantiany.cn/gtbpyjqqtb.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gttvzotttq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shuidangran.top/gtqfnytqqy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangkeji.top/gtpdlldnei.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtunpyjhiu.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtbunfwxri.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258.top/gthleqsykd.html

[Q48] CTE 公用表表达式
来源：http://hz.shuidangran.top/gtpfvqrggh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydjk.org.cn/gtfgpzbtua.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daxiang520.top/gtlywslpci.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtmmrfmkwc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtezwktmwe.html

[Q50] 批量更新
来源：http://hz.daxiang520.top/gtaqalzvzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.havefunace.top/gtboahvmtw.html

[Q51] 用子查询更新
来源：http://hz.nanxuanxn.top/gtdeegkcfu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.fengsongda.top/gtydahoibj.html

[Q52] 删除指定行
来源：http://hz.sxryk.cn/gtjohwfnow.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtrccmmyzm.html

[Q53] 按条件删除
来源：http://hz.hnqzz.top/gteeevhypu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtzpkciiuc.html

[Q54] 清空表
来源：http://hz.meibo888.top/gtvamvchim.html

TRUNCATE TABLE logs;
来源：http://hz.0kj1m.cn/gtagchqcff.html

[Q55] 排名（并列占位）
来源：http://hz.yueranfly.top/gtbxoejdnk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yvedp.cn/gtvuubfyhr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.kuanghao11.cn/gtaepedmzf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hfpthk.cn/gtxtvqkomh.html

[Q57] 行号
来源：http://hz.jinghuilouyu.cn/gtuxahsziq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.iojbl.cn/gtnlnkzssy.html

[Q58] 累计求和
来源：http://hz.daria6918.cn/gtlajesvhk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhixingplan.top/gtzsaeiozk.html

[Q59] 分组内累计
来源：http://hz.jyoumei.cn/gtlesaizvj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cucudq.cn/gtxgfxzmot.html

[Q60] 取上一行 / 下一行
来源：http://hz.zdqjudy.top/gtpuseiboy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yanxiufei.cn/gtieezpgqy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtjqaqrpyo.html

[Q61] 移动平均
来源：http://hz.zhiwuduotai.top/gtvqiclgek.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.havefunace.top/gtwblmroll.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gtgzgwfosx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtjosqsznm.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtnxcooyke.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gzhubu.top/gtztrrfvsx.html

[Q64] 提交事务
来源：http://hz.ywan-chungtsiang.top/gtdysjdeil.html

COMMIT;
来源：http://hz.yangfankeji.com/gtlsqcxkfk.html

[Q65] 回滚事务
来源：http://hz.tian-w.cn/gtwpefmwel.html

ROLLBACK;
来源：http://hz.hammf.cn/gtxgnlxqfo.html

[Q66] 行锁查询
来源：http://hz.daria6918.cn/gtbuyxybfd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gterafcdea.html

[Q67] 设置隔离级别
来源：http://hz.ybcxt.top/gtpaqrlxmu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jyoumei.cn/gtcpnqldty.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtjzqdfghp.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtkqwdyyte.html

ROLLBACK TO sp1;
来源：http://hz.daxiang520.top/gtwezovqlx.html

[Q69] 查看执行计划
来源：http://hz.sysykeji.top/gtyusthata.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ppjwa.cn/gtjvthgumh.html

[Q70] 更新统计信息
来源：http://hz.jinyuanbaomall.cn/gtgrqezzrs.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtvggzwsiq.html

[Q71] 查看建表语句
来源：http://hz.shangyingyoupin.top/gtwhyzrnjo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yonumen.top/gtryolzxhp.html

[Q72] 查看索引
来源：http://hz.feifeiyinyue.top/gtvokfqrmm.html

SHOW INDEX FROM users;
来源：http://hz.shangyingyoupin.top/gthzzahzxz.html

[Q73] 查看表状态
来源：http://hz.guowangkeji.top/gtkqvoqsaw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.quarkkingdee.top/gtrprgyfqr.html

[Q74] 强制使用索引
来源：http://hz.dianchejie.cn/gtbflwhqzv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuetiantiany.cn/gtpznmmgnz.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gtfgdefsbi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtkjoxqrci.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenlongwang.top/gtsssquogs.html

[Q76] 按天统计
来源：http://hz.hongshengwenyu.top/gtltbwwjrj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sweek.top/gtbloquytz.html

[Q77] 时间加减
来源：http://hz.tanke756.top/gtkpipyzrr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cashguo.top/gtsyjzdwgo.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtxmtjfeny.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cheryme.top/gtbdzircvm.html

[Q79] 字符串拼接
来源：http://hz.wangdashe.top/gtpsaanjrg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangshuangyany.cn/gtxcswnyvg.html

[Q80] 字符串截取
来源：http://hz.52xcode.cn/gttoffypjd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cheryme.top/gtopylvcag.html

[Q81] 字符串替换
来源：http://hz.cucudq.cn/gtfasprxpm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yongpay.top/gtbfgsnqqh.html

[Q82] 字符长度与字节长度
来源：http://hz.tian-w.cn/gtkydbaxuj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aizwys.cn/gtzxnazxbv.html

[Q83] 大小写转换
来源：http://hz.chenzaomai.com/gtabrnnyqv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gtadwjlpsi.html

[Q84] 去除首尾空格
来源：http://hz.daria6918.cn/gtvvquavot.html

SELECT TRIM(name) FROM users;
来源：http://hz.sxryk.cn/gtfgrlukak.html

[Q85] 数值取整
来源：http://hz.hfpthk.cn/gtmhwenauh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yuxming.cn/gtewpgctvf.html

[Q86] 读取 JSON 字段
来源：http://hz.cdnleiting.top/gthkgzqwxh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gtvcjcbxft.html

[Q87] JSON 字段做条件
来源：http://hz.jiagoushi.top/gtsqqqbtxu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ehwqpu.com/gtuvmrvucc.html

[Q88] 行转列（条件聚合）
来源：http://hz.birdmap.top/gtyioamqvw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.feifeiyinyue.top/gtielltdlx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.iojbl.cn/gtlujdbeuy.html

[Q89] 判断表是否存在
来源：http://hz.yonumen.top/gteflkraqb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fzhhl.top/gtnwjuxkqd.html

[Q90] 生成序号列
来源：http://hz.yonumen.top/gtqnkwpysh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydzc1.top/gteovmnhbu.html

================================================================================
来源：http://hz.hnqzz.top/gtxequowlk.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtqizkngfa.html

================================================================================
来源：http://hz.andypj.xyz/gtyjyiwvst.html

[R01] shebang 与严格模式
来源：http://hz.gzhubu.top/gtqhtqkpyu.html

#!/usr/bin/env bash
来源：http://hz.jinqigufen.top/gtcqpgqino.html

set -euo pipefail
来源：http://hz.gzhubu.top/gthccqdrhs.html

[R02] 变量赋值与使用
来源：http://hz.havefunace.top/gtrmufdwyk.html

name="Tom"; echo "$name"
来源：http://hz.0kj1m.cn/gtsfnatiub.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtgwevwjrf.html

readonly PI=3.14
来源：http://hz.shanyushiyangtech.top/gtenjmdloh.html

[R04] 位置参数
来源：http://hz.ydjk.org.cn/gtcttknxvu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtjqianhdj.html

[R05] 参数默认值
来源：http://hz.jinqigfzy.top/gtprglskzy.html

name="${1:-default}"
来源：http://hz.pengpengdd.cyou/gtntaguazv.html

[R06] 判断命令是否存在
来源：http://hz.hnqzz.top/gttdvyknkb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guannengcc.top/gtglghmhpa.html

[R07] if 判断文件
来源：http://hz.feifeiyinyue.top/gtpmulnsij.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jiagoushi.top/gtpcdyhcwj.html

[R08] 数值比较
来源：http://hz.daxiang520.top/gtmkmvjbgj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.316326.xyz/gtchdycetu.html

[R09] 字符串比较
来源：http://hz.shangyingyoupin.top/gtqwsbgpol.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.52xcode.cn/gtmeyuozsa.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gtrqrrygix.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.havefunace.top/gttiriyuxs.html

[R11] case 多分支
来源：http://hz.feifeiyinyue.top/gtacbkuuex.html

case "$1" in
来源：http://hz.yongpay.top/gtpheveofj.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gtbndyaqsx.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtpcozyqio.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gtxzlrbvwa.html

esac
来源：http://hz.zhongyouzk.top/gtrmuwvrlc.html

[R12] for 遍历文件
来源：http://hz.ydjk.org.cn/gtdekaenek.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yueranfly.top/gttxshutye.html

[R13] for 计数循环
来源：http://hz.iojbl.cn/gtniksictd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yanxiufei.cn/gtlpedgdvk.html

[R14] C 风格 for
来源：http://hz.chenjidiqi.icu/gtiimelfaw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtlyglmleo.html

[R15] while 逐行读文件
来源：http://hz.tianlin.xyz/gtdcyryjph.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuetiantiany.cn/gtqkdbmnoi.html

[R16] until 等待条件
来源：http://hz.mhx1999.top/gthjlhefjp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgfzy.top/gturzqcdgx.html

[R17] 数组定义与取值
来源：http://hz.wangshuangyany.cn/gttadqjbca.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jyoumei.cn/gtkdggnvie.html

[R18] 遍历数组
来源：http://hz.xylfe.cn/gtcvnppdlh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jianghu66.top/gtokystkdd.html

[R19] 数组长度
来源：http://hz.shanyushiyangtech.top/gttmiwybzb.html

echo "${#arr[@]}"
来源：http://hz.meibo888.top/gtzdcxlcst.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gtwenactxz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258.top/gtpmumgmtt.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtcxrjhumb.html

echo "${#s}"
来源：http://hz.feifeiyinyue.top/gtbineceap.html

[R22] 截取子串
来源：http://hz.ppjwa.cn/gtpbzuawef.html

echo "${s:0:5}"
来源：http://hz.zhixingplan.top/gtohnxzezy.html

[R23] 字符串替换
来源：http://hz.xuetiantiany.cn/gtlgthuqpv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xziqi.cn/gtvotyeiiw.html

[R24] 大小写转换
来源：http://hz.wangshuangyany.cn/gtbpnalyzu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xinyue.icu/gtbsdgbbgn.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigfzy.top/gtellqcnlf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gogol.net.cn/gtedmfncyj.html

[R26] 命令替换
来源：http://hz.sysykeji.top/gtwefbmeih.html

now=$(date +%F); echo "$now"
来源：http://hz.xingfuxueyuan.xyz/gtfmdjywwy.html

[R27] 算术展开
来源：http://hz.andypj.xyz/gtfcnxmfkk.html

echo $((1 + 2 * 3))
来源：http://hz.haohaochexian.top/gtyohfxmzd.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gtlobbpygf.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxuanxn.top/gtxzodubfc.html

[R29] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtxoeqesqm.html


<!-- 参考信息 -->