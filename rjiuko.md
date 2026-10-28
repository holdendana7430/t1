代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgufenzy.top/gtgtieavyw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xingfuxueyuan.xyz/gthjoubiml.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.snrcjt.cn/gtckzwthvj.html

PHP:  if (empty($x)) {}
来源：http://hz.jinghuilouyu.cn/gtqsqaidkp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.feifeiyinyue.top/gtivfwzjwh.html

TS:   if (x == null) {}
来源：http://hz.jinqigufen.top/gtohklkdlb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gteieezfwu.html

Go:   if x == nil {}
来源：http://hz.yvedp.cn/gtuumzeaft.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jiagoushi.top/gtbuyiavge.html

C#:   if (x is null) {}
来源：http://hz.cheryme.top/gtgwricren.html

[P07] 防抖与节流
来源：http://hz.aibaodan.cn/gtqioljxye.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shangyingyoupin.top/gtasnahzjg.html

PHP:  // 手写时间戳比较
来源：http://hz.9152youxi.cn/gtcwfitvok.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtwdeiwsha.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtsdooavsz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.birdmap.top/gtafoxlcra.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258.top/gtpznuhsgt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cqqwz.cn/gtcggpcqio.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj202588.top/gtbafnfaza.html

[P08] 处理浮点精度问题
来源：http://hz.zhengqikj.top/gthotjcqiz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fzhhl.top/gtazcxgnlf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tanke756.top/gtmdnbrnpw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daria6918.cn/gtzianfuxf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgufenzy.top/gttrudogsn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.haohaochexian.top/gtklelnvve.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fzhhl.top/gtfbsditps.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenlongwang.top/gtpxhamelq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangtech.top/gtyxjotohe.html

================================================================================
来源：http://hz.yueranfly.top/gttiihsenm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnqzz.top/gtjttydjdk.html

================================================================================
来源：http://hz.zhixingplan.top/gtwmzsqzxb.html

[Q01] 创建表
来源：http://hz.yvedp.cn/gtlekmzzke.html

CREATE TABLE users (
来源：http://hz.aizwys.cn/gtvkrgqdsi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtviudsama.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cdnleiting.top/gtjjnxoebw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.mhx1999.top/gtlcqrgmwi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jiagoushi.top/gtfeuqcynx.html

);
来源：http://hz.meibo888.top/gtfpckczyc.html

[Q02] 创建带外键的表
来源：http://hz.wangshuangyany.cn/gtkbfipxwb.html

CREATE TABLE orders (
来源：http://hz.wangshuangyany.cn/gttxavfrou.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtbizongsn.html

user_id INT NOT NULL,
来源：http://hz.ppjwa.cn/gtgzqkzqtw.html

amount DECIMAL(10, 2),
来源：http://hz.fzhhl.top/gtouicpgaf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xziqi.cn/gtsthabjfk.html

);
来源：http://hz.yongpay.top/gthfdxqkow.html

[Q03] 增加列
来源：http://hz.gogol.net.cn/gtimtalljj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.smart0.xyz/gtqonaemnd.html

[Q04] 修改列类型
来源：http://hz.yonumen.top/gtirratvid.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.snrcjt.cn/gtpdaagref.html

[Q05] 重命名列
来源：http://hz.tianlin.xyz/gtbonkyjhj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.svipenyu.cn/gtkhwhtxde.html

[Q06] 删除列
来源：http://hz.yj20258888.top/gtqmpqqvqn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yvedp.cn/gtdjbvtlus.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gtgwpevpkw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jiagoushi.top/gtuhufxtxj.html

[Q08] 创建普通索引
来源：http://hz.9152youxi.cn/gtallrlyaq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gtnckqrvwr.html

[Q09] 创建唯一索引
来源：http://hz.ehwqpu.com/gtqglnfiuv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nwbrower.top/gtmxdrrtfh.html

[Q10] 插入单行
来源：http://hz.svipenyu.cn/gtbenbtjfk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.0kj1m.cn/gtautismma.html

[Q11] 一次插入多行
来源：http://hz.hysaishi.cn/gtasyqsnco.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinyuanbaomall.cn/gtpdqwhjtx.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgfzy.top/gtojoxmtta.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.mhx1999.top/gtfuyyvxlv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhiwuduotai.top/gtnlocwpwv.html

[Q13] 忽略重复插入
来源：http://hz.sweek.top/gtusmsshjq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258888.top/gtgnwoxwxn.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gthbqcpwuk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sweek.top/gtfzfybhpc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhiwuduotai.top/gtnndxaqpp.html

[Q15] 查询全部
来源：http://hz.havefunace.top/gtywkgwmbg.html

SELECT * FROM users;
来源：http://hz.zdqjudy.top/gtqqjbclye.html

[Q16] 查询指定列
来源：http://hz.aizwys.cn/gtynaggvmn.html

SELECT id, name FROM users;
来源：http://hz.andypj.xyz/gtjfxozlem.html

[Q17] 条件查询
来源：http://hz.jqgfzy.top/gtzwvucjws.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigfzy.top/gtfvcchxko.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gtmkxjhjdq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tian-w.cn/gtqmhhgihd.html

[Q19] 范围查询
来源：http://hz.guowangkeji.top/gthfqemuel.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhiwuduotai.top/gtmysknbuc.html

[Q20] IN 列表
来源：http://hz.zhengqikj.top/gtmeuitebt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtcmanerpo.html

[Q21] 空值判断
来源：http://hz.gaohongyu789.top/gtpidtcjjc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ehwqpu.com/gtcivznyvl.html

[Q22] 排序
来源：http://hz.yj202588.top/gtycgefguf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hammf.cn/gtkkohtpaa.html

[Q23] 分页
来源：http://hz.gotoacloud.top/gtknkuyyng.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gotoacloud.top/gtuxbpryaa.html

[Q24] 去重
来源：http://hz.shuidangran.top/gtqprexpnc.html

SELECT DISTINCT city FROM users;
来源：http://hz.snrcjt.cn/gtrznlixuo.html

[Q25] 只取前 N 条
来源：http://hz.cdnleiting.top/gtaoegefcb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tianlin.xyz/gtqofyrckx.html

[Q26] 计数
来源：http://hz.jianghu66.top/gtjllgzaqf.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhixingplan.top/gtwegvsysp.html

[Q27] 条件计数
来源：http://hz.haohaochexian.top/gtvrhizbby.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tian-w.cn/gtvxtqfmvt.html

[Q28] 求和与平均
来源：http://hz.guannengcc.top/gtxtevklka.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gtoilrfrof.html

[Q29] 最大最小值
来源：http://hz.52xcode.cn/gtkrperfya.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnqzz.top/gtielokqoq.html

[Q30] 分组统计
来源：http://hz.birdmap.top/gtacurxpwf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtnorcfchb.html

[Q31] 分组后过滤
来源：http://hz.vqdsnc.cn/gtnxyfryxj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhaomingkeji.xyz/gtesrtjkiy.html

[Q32] 分组拼接字符串
来源：http://hz.havefunace.top/gtxkuqcdum.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtwzsvvtrg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gtekxeaevr.html

[Q33] 多列分组
来源：http://hz.cucudq.cn/gtmfejtmsb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.snrcjt.cn/gtkrlscfpb.html

[Q34] 每组取第一条
来源：http://hz.shzxlz.cn/gtidnmeugb.html

SELECT * FROM (
来源：http://hz.tanke756.top/gtloeubpjq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ivvv.top/gtuqjiyrnv.html

) t WHERE rn = 1;
来源：http://hz.jinghuilouyu.cn/gtvngiflre.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtayulxkdb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtslvmoyov.html

[Q36] 左连接
来源：http://hz.jinqigfzy.top/gtczmefkuj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtktotdxsy.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtmbwhkvkn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtfwetlqle.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jqgfzy.top/gtcduadfuv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenlongwang.top/gtbtsxgiec.html

[Q39] 自连接（查上下级）
来源：http://hz.daxiang520.top/gtpvdfmlid.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fzhhl.top/gthcsvenyz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hywenlv.cn/gtknaqvguz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.c1oappe.top/gtiioxbtbi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hysaishi.cn/gtznjhynuu.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtcxfzdqko.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gogol.net.cn/gtnknozyvg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.svipenyu.cn/gtmfltoilb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aibaodan.cn/gtydrpghct.html

[Q42] 连接条件附加过滤
来源：http://hz.bjfxy.top/gtytgxwdgw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtupylmkjs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxuanxn.top/gthjohiweu.html

[Q43] 标量子查询
来源：http://hz.ybcxt.top/gtwhjqazkk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hysaishi.cn/gtsggoqivx.html

[Q44] IN 子查询
来源：http://hz.kuanghao11.cn/gtelwbdjym.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fengsongda.top/gthxxosxcn.html

[Q45] EXISTS 判断存在
来源：http://hz.ywan-chungtsiang.top/gtaoliimta.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtvrxanlmd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cashguo.top/gtbfzemnrj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtjespfgau.html

[Q47] 与平均值比较
来源：http://hz.yuanzhike.top/gtpnclhhxt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.52xcode.cn/gtqeneqcep.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gtiqakuzuv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuanzx.com/gtyjxunddj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuxming.cn/gttgdbxfun.html

[Q49] 更新单行
来源：http://hz.aibaodan.cn/gteifwppuq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtvddwaliz.html

[Q50] 批量更新
来源：http://hz.ivvv.top/gtydbeyjuj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xylfe.cn/gtnuuwfcdg.html

[Q51] 用子查询更新
来源：http://hz.tian-w.cn/gtrzblwatr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yanxiufei.cn/gtbydtptkw.html

[Q52] 删除指定行
来源：http://hz.52xcode.cn/gtqxhsexou.html

DELETE FROM users WHERE id = 10;
来源：http://hz.mhx1999.top/gtmawfraum.html

[Q53] 按条件删除
来源：http://hz.gotoacloud.top/gtxruydezt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ivvv.top/gtgmnnhdjo.html

[Q54] 清空表
来源：http://hz.0kj1m.cn/gtmakfgbog.html

TRUNCATE TABLE logs;
来源：http://hz.aizwys.cn/gtzxwzyfsx.html

[Q55] 排名（并列占位）
来源：http://hz.yanxiufei.cn/gtwzzgmyoa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gtluguswjq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pycfn.com/gtticnkzdd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtuetyjjtb.html

[Q57] 行号
来源：http://hz.iojbl.cn/gtuniqnflu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.dashuyun.cn/gtdxpcobzy.html

[Q58] 累计求和
来源：http://hz.tian-w.cn/gtcctaxmgy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.aizwys.cn/gtljdligcg.html

[Q59] 分组内累计
来源：http://hz.zhixingplan.top/gtkrvxajzy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.havefunace.top/gtuhuzhuxt.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gteyigxepe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtemmgbjzs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtvcmgrgne.html

[Q61] 移动平均
来源：http://hz.jinyuanbaomall.cn/gthzpedavk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fengsongda.top/gtkbkibvza.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtvuvjqlol.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtsjmgmpnu.html

[Q63] 开启事务
来源：http://hz.cheryme.top/gtyecyhmjm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtkdcypemu.html

[Q64] 提交事务
来源：http://hz.chenjidiqi.icu/gtrqyofnaa.html

COMMIT;
来源：http://hz.tianlin.xyz/gtnvmpwcor.html

[Q65] 回滚事务
来源：http://hz.shanyushiyangkeji.top/gtsjsldonj.html

ROLLBACK;
来源：http://hz.nwbrower.top/gtexieeolg.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtrrtsmhxp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shuidangran.top/gtwxzimryv.html

[Q67] 设置隔离级别
来源：http://hz.yuanzhike.top/gtihebzwqq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gotoacloud.top/gtkavlwnti.html

[Q68] 保存点
来源：http://hz.zhongyouzk.top/gtnxuyxaby.html

SAVEPOINT sp1;
来源：http://hz.zhoulong.xyz/gtmnzxhlit.html

ROLLBACK TO sp1;
来源：http://hz.ybcxt.top/gtuixafpwn.html

[Q69] 查看执行计划
来源：http://hz.zhijiandao.cn/gtngsbevtu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yangfankeji.com/gtctoktthh.html

[Q70] 更新统计信息
来源：http://hz.jinghuilouyu.cn/gtdgrtuakc.html

ANALYZE TABLE users;
来源：http://hz.shangyingyoupin.top/gtlnsiqdvy.html

[Q71] 查看建表语句
来源：http://hz.jlsjyb.cn/gtpwszwvxe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xingfuxueyuan.xyz/gtjamzjhuw.html

[Q72] 查看索引
来源：http://hz.cashguo.top/gtzgxdhhpu.html

SHOW INDEX FROM users;
来源：http://hz.pycfn.com/gtqvcbpwib.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtdrtccpcy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangdashe.top/gtaxzhfdlw.html

[Q74] 强制使用索引
来源：http://hz.xziqi.cn/gtbprwhosn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuanzx.com/gtnevjvobw.html

[Q75] 日期格式化
来源：http://hz.yvedp.cn/gtxhlvsayt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtgbkcrhii.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuxming.cn/gttrtoirju.html

[Q76] 按天统计
来源：http://hz.zhaomingkeji.xyz/gtfkxepspw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dianchejie.cn/gteimwyjto.html

[Q77] 时间加减
来源：http://hz.yanxiufei.cn/gtfymngrib.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhengqikj.top/gtmhaxysrn.html

[Q78] 当前时间
来源：http://hz.zdqjudy.top/gtclfrmjpr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pengpengdd.cyou/gtpcgudgie.html

[Q79] 字符串拼接
来源：http://hz.iojbl.cn/gtzquywnvq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhijiandao.cn/gtuznnaxox.html

[Q80] 字符串截取
来源：http://hz.jiagoushi.top/gtosbbecri.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtyzwomgtg.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtrdpgznge.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yonumen.top/gtdzgebuvs.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gtkjpsodgj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hfpthk.cn/gtkzacvkhi.html

[Q83] 大小写转换
来源：http://hz.chenzaomai.com/gtxjaeeucr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.c1oappe.top/gtzatinmlh.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtvayzfbpl.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigufen.top/gtxzyzsecn.html

[Q85] 数值取整
来源：http://hz.zdqjudy.top/gtyhwwhhon.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yvedp.cn/gtmfxlnrmo.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gtpkjemepy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zdqjudy.top/gtcgtolriq.html

[Q87] JSON 字段做条件
来源：http://hz.hysaishi.cn/gtlhvsptwj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.feifeiyinyue.top/gtmiztkhdo.html

[Q88] 行转列（条件聚合）
来源：http://hz.ywan-chungtsiang.top/gtrhonfxxw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.birdmap.top/gtfciakspy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtrusswjoe.html

[Q89] 判断表是否存在
来源：http://hz.chenzaomai.com/gtwgvuwito.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gtfzdlhmpx.html

[Q90] 生成序号列
来源：http://hz.haohaochexian.top/gtiakmrxtp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yangfankeji.com/gtoazvrjgh.html

================================================================================
来源：http://hz.jianghu66.top/gtjebpbdik.html

R. Bash 专题
来源：http://hz.redwolf501.top/gtythjnchf.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtsvgwykyq.html

[R01] shebang 与严格模式
来源：http://hz.xziqi.cn/gtmqgtdcxx.html

#!/usr/bin/env bash
来源：http://hz.birdmap.top/gtkpxpcmze.html

set -euo pipefail
来源：http://hz.9152youxi.cn/gthvayvfsr.html

[R02] 变量赋值与使用
来源：http://hz.smart0.xyz/gteqxpcoum.html

name="Tom"; echo "$name"
来源：http://hz.cqqwz.cn/gtpnmvuudw.html

[R03] 只读变量
来源：http://hz.yongpay.top/gtpdhwfcpc.html

readonly PI=3.14
来源：http://hz.tanke756.top/gtzyupubmh.html

[R04] 位置参数
来源：http://hz.sufxvd.cn/gtjjtmmvku.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jiagoushi.top/gtwyswyvwv.html

[R05] 参数默认值
来源：http://hz.9152youxi.cn/gtahapclkk.html

name="${1:-default}"
来源：http://hz.0kj1m.cn/gtevsymgvr.html

[R06] 判断命令是否存在
来源：http://hz.0kj1m.cn/gtnitoconi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnqzz.top/gtlloxaquy.html

[R07] if 判断文件
来源：http://hz.hywenlv.cn/gthxtsdefy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jqgufenzy.top/gtouuqhefi.html

[R08] 数值比较
来源：http://hz.feifeiyinyue.top/gtlajbywqf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuetiantiany.cn/gterodmtmp.html

[R09] 字符串比较
来源：http://hz.zycfv.cn/gtpoydivuv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sysykeji.top/gtilnouaos.html

[R10] 正则匹配
来源：http://hz.tanke756.top/gtsmxxxyox.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258.top/gttyzvedzb.html

[R11] case 多分支
来源：http://hz.aizwys.cn/gtduulpzfm.html

case "$1" in
来源：http://hz.jinghuilouyu.cn/gtckijywmm.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gtnpcnqfqz.html

stop)  echo "停止" ;;
来源：http://hz.ppjwa.cn/gtxwqryvzp.html

*)     echo "未知命令" ;;
来源：http://hz.zhiwuduotai.top/gtxpushggo.html

esac
来源：http://hz.feifeiyinyue.top/gtgaxngekd.html

[R12] for 遍历文件
来源：http://hz.svipenyu.cn/gtgvmiczmz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hywenlv.cn/gtralpegwq.html

[R13] for 计数循环
来源：http://hz.chenlongwang.top/gtbsjaxpgw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hysaishi.cn/gtjjesjuoy.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gticrvyszn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtzktissva.html

[R15] while 逐行读文件
来源：http://hz.yonumen.top/gtvxhioexf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuanzhike.top/gtmcvlshuv.html

[R16] until 等待条件
来源：http://hz.zhengqikj.top/gtyegpipgx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtsmddmmdu.html

[R17] 数组定义与取值
来源：http://hz.sweek.top/gthrgtsrsj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yonumen.top/gtfyonhplo.html

[R18] 遍历数组
来源：http://hz.jinqigufen.top/gtmdpolhhi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtmvhmrpfg.html

[R19] 数组长度
来源：http://hz.jinghuilouyu.cn/gtsqkisizh.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtxwtwthze.html

[R20] 关联数组（字典）
来源：http://hz.jlsjyb.cn/gtonzypbol.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hywenlv.cn/gtrtsmucff.html

[R21] 字符串长度
来源：http://hz.haohaochexian.top/gtpbjuexbu.html

echo "${#s}"
来源：http://hz.yvedp.cn/gtxyohfxvp.html

[R22] 截取子串
来源：http://hz.snrcjt.cn/gtwotvmxvr.html

echo "${s:0:5}"
来源：http://hz.kuanghao11.cn/gtqayqbqgb.html

[R23] 字符串替换
来源：http://hz.yueranfly.top/gtrbbaakfq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gtqrlbbaqg.html

[R24] 大小写转换
来源：http://hz.hnxiangtu.top/gtbvnovndd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtswefdcos.html

[R25] 去后缀 / 去前缀
来源：http://hz.sweek.top/gtueoepywu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tanke756.top/gtcxkbhvai.html

[R26] 命令替换
来源：http://hz.xziqi.cn/gtfwpksiki.html

now=$(date +%F); echo "$now"
来源：http://hz.iojbl.cn/gtxlzkvpyy.html

[R27] 算术展开
来源：http://hz.yj202588.top/gtqvbzkvgj.html

echo $((1 + 2 * 3))
来源：http://hz.aibaodan.cn/gtuzhjhoiz.html

[R28] 浮点运算
来源：http://hz.hnxiangtu.top/gtsgxtyelw.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gthuocnrym.html

[R29] 定义函数
来源：http://hz.zhengqikj.top/gtsaoeguht.html


<!-- 参考信息 -->