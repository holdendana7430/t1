代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aizwys.cn/gtjeavnodl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cheryme.top/gtyqwpbyog.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtrilbhfuc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtietxgnem.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jianghu66.top/gtixwmvdls.html

Go:   len(arr);  len(m)
来源：http://hz.yueranfly.top/gtecslxrgb.html

Ruby: x.length;  x.size
来源：http://hz.ehwqpu.com/gtxzpvajay.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.havefunace.top/gtxzmtoqxz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj20258.top/gttyifpkqb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hysaishi.cn/gtfauinncr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gtbchwfoff.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.52xcode.cn/gtowwkboqn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtrfwxtnor.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtmtttskog.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ydzc1.top/gtpjfgivyx.html

Ruby: a == b
来源：http://hz.shuidangran.top/gtjrhdkkyr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.redwolf501.top/gtgtlgzxxv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yonumen.top/gtaymelbmp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xylfe.cn/gteamkmauk.html

PHP:  if (empty($x)) {}
来源：http://hz.xuetiantiany.cn/gtswzptgai.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.kuanghao11.cn/gtymifngte.html

TS:   if (x == null) {}
来源：http://hz.smart0.xyz/gtfjmuzmvd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtuhgllmsu.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtbpiuzvtk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yvedp.cn/gtbbvkzbde.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtqmbxhhgn.html

[P07] 防抖与节流
来源：http://hz.hfpthk.cn/gtonnhrzun.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xziqi.cn/gtjkqnkhoa.html

PHP:  // 手写时间戳比较
来源：http://hz.aizwys.cn/gturiimxjm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtgbkulsis.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtjrbrafoa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.quarkkingdee.top/gtjhwenlal.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgufenzy.top/gtdvsmzdid.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jianghu66.top/gtybhsosxa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gtkvlywapu.html

[P08] 处理浮点精度问题
来源：http://hz.cashguo.top/gtobmjiqke.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinghuilouyu.cn/gtfngoqonp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.haohaochexian.top/gtcrgckvoy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yuanzhike.top/gtkhjvylbi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.smart0.xyz/gtgjjtcadg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenjidiqi.icu/gtgvmaszez.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gtqurgbuin.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxinkj.top/gtebynmjkw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhongyouzk.top/gtnffajwdl.html

================================================================================
来源：http://hz.9152youxi.cn/gtnnhedhjl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jqgfzy.top/gtqabukhaa.html

================================================================================
来源：http://hz.birdmap.top/gtsliujcjb.html

[Q01] 创建表
来源：http://hz.hfpthk.cn/gtpkphddwm.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtlyziepwz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtssesmyce.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cdnleiting.top/gtkjmpvbhn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuanzhike.top/gttfvhojbj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yueranfly.top/gttmqhgoet.html

);
来源：http://hz.sweek.top/gtrksrtwxe.html

[Q02] 创建带外键的表
来源：http://hz.jinqigfzy.top/gthnqnefne.html

CREATE TABLE orders (
来源：http://hz.yongpay.top/gtkovjtbiv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gthcdmiazi.html

user_id INT NOT NULL,
来源：http://hz.ydjk.org.cn/gtgufovypk.html

amount DECIMAL(10, 2),
来源：http://hz.0kj1m.cn/gtevjbpdyz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gzhubu.top/gtvvpcdqpd.html

);
来源：http://hz.yangfankeji.com/gtifflttde.html

[Q03] 增加列
来源：http://hz.hnxiangtu.top/gtchcwfdez.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.svipenyu.cn/gtpocafvdd.html

[Q04] 修改列类型
来源：http://hz.zdqjudy.top/gtcttgsyhh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.pycfn.com/gtetkyqlhx.html

[Q05] 重命名列
来源：http://hz.bjfxy.top/gtzrwtavrc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj202588.top/gtsibwfymx.html

[Q06] 删除列
来源：http://hz.sufxvd.cn/gtzxzyqnsi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtpetpsgyd.html

[Q07] 删除表
来源：http://hz.mhx1999.top/gtwqeatrmt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aibaodan.cn/gtmkhqvzvz.html

[Q08] 创建普通索引
来源：http://hz.chenlongwang.top/gtpxvofrng.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigfzy.top/gtukszubcq.html

[Q09] 创建唯一索引
来源：http://hz.0kj1m.cn/gtyckyckak.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtjixzprap.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtlymwsydr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhongyouzk.top/gtskfejehs.html

[Q11] 一次插入多行
来源：http://hz.mhx1999.top/gtkbzvponv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.iojbl.cn/gtemzdfvme.html

[Q12] 插入后取自增 ID
来源：http://hz.nanxuanxn.top/gththvesms.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sufxvd.cn/gtczornats.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.bjfxy.top/gtgurcjtpp.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtijgmaaxp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cdnleiting.top/gtrkjnujoc.html

[Q14] 存在则更新（upsert）
来源：http://hz.shangyingyoupin.top/gtwrrtyyeq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shuidangran.top/gtmeihnjkg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hysaishi.cn/gtxevngjgo.html

[Q15] 查询全部
来源：http://hz.sweek.top/gticujbfpf.html

SELECT * FROM users;
来源：http://hz.zdqjudy.top/gtdnvzmmqa.html

[Q16] 查询指定列
来源：http://hz.cheryme.top/gtnvuoyzcv.html

SELECT id, name FROM users;
来源：http://hz.gotoacloud.top/gtplpirqgb.html

[Q17] 条件查询
来源：http://hz.c1oappe.top/gtguhqtvci.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtsadhnpaz.html

[Q18] 模糊匹配
来源：http://hz.bjfxy.top/gtldkuzqns.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yanxiufei.cn/gtnkjssuxh.html

[Q19] 范围查询
来源：http://hz.wangdashe.top/gtbwniahuk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenjidiqi.icu/gtxfbmokvj.html

[Q20] IN 列表
来源：http://hz.jinqigufen.top/gthhuyqqqj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hongshengwenyu.top/gtifwuqmkl.html

[Q21] 空值判断
来源：http://hz.yj20258888.top/gtfsocqabv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hammf.cn/gtpdhnuird.html

[Q22] 排序
来源：http://hz.gotoacloud.top/gttqfrinkl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gtusqlytlt.html

[Q23] 分页
来源：http://hz.hysaishi.cn/gtqhrzmtuk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinghuilouyu.cn/gtzlzwucbi.html

[Q24] 去重
来源：http://hz.yj20258.top/gtrokslyiu.html

SELECT DISTINCT city FROM users;
来源：http://hz.sysykeji.top/gtqewpeeor.html

[Q25] 只取前 N 条
来源：http://hz.smart0.xyz/gtcmmgnxng.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gtjvcdsddv.html

[Q26] 计数
来源：http://hz.wangshuangyany.cn/gtdxyvwnhm.html

SELECT COUNT(*) FROM users;
来源：http://hz.yvedp.cn/gtlxpgqcdg.html

[Q27] 条件计数
来源：http://hz.hammf.cn/gtbsiaxbps.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yueranfly.top/gttzsobjdw.html

[Q28] 求和与平均
来源：http://hz.gogol.net.cn/gtstlpcrfb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuetiantiany.cn/gtqctdyjjf.html

[Q29] 最大最小值
来源：http://hz.sysykeji.top/gtfjlhvpgw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.redwolf501.top/gtpyuqihqe.html

[Q30] 分组统计
来源：http://hz.zhijiandao.cn/gthhcqvmhl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtfnjgozfm.html

[Q31] 分组后过滤
来源：http://hz.zhixingplan.top/gtbuvrwffz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gtyhqipoyl.html

[Q32] 分组拼接字符串
来源：http://hz.wangdashe.top/gthbrvotbi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtmhqyghjk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinyuanbaomall.cn/gtcizydewb.html

[Q33] 多列分组
来源：http://hz.smart0.xyz/gttzjildaw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hysaishi.cn/gthaifgubq.html

[Q34] 每组取第一条
来源：http://hz.guowangkeji.top/gtxhqxixlw.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtwrddebbg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dashuyun.cn/gtczpddqsb.html

) t WHERE rn = 1;
来源：http://hz.tianlin.xyz/gtpmohwbbj.html

[Q35] 内连接
来源：http://hz.nanxinkj.top/gtikvzghgs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtnowwpfmm.html

[Q36] 左连接
来源：http://hz.ivvv.top/gtnkxeppuh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gttmlvzonp.html

[Q37] 右连接
来源：http://hz.snrcjt.cn/gtrzchzofq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gtrltevmon.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tian-w.cn/gtyltqokqq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.c1oappe.top/gthqqzcndn.html

[Q39] 自连接（查上下级）
来源：http://hz.hammf.cn/gtaftsuuzi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zycfv.cn/gtondxkuio.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daxiang520.top/gtlomdgoaz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhiwuduotai.top/gtgcedcgbs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sufxvd.cn/gtxuirznwf.html

[Q41] 多表连接
来源：http://hz.snrcjt.cn/gtuofotiyg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.52xcode.cn/gtkqvuoejj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gzhubu.top/gtceywbdua.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aibaodan.cn/gtbcfzufhh.html

[Q42] 连接条件附加过滤
来源：http://hz.hnxiangtu.top/gtmvwrwhnl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtnhrzhhfe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxinkj.top/gtjmhmztjf.html

[Q43] 标量子查询
来源：http://hz.tianlin.xyz/gtgmohaszo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cucudq.cn/gtsjnwbpxk.html

[Q44] IN 子查询
来源：http://hz.zhiwuduotai.top/gtsbpvemub.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daria6918.cn/gtegvumogb.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gthbbymrim.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gtsdexdgec.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aizwys.cn/gtyfbmamfa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cucudq.cn/gthvrrrvay.html

[Q47] 与平均值比较
来源：http://hz.kuanghao11.cn/gtqgezwdek.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.vqdsnc.cn/gtinbyjsai.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtmdzhsduy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangshuangyany.cn/gtzlscxadg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtwwernivb.html

[Q49] 更新单行
来源：http://hz.shanyushiyangkeji.top/gtwcbhaiav.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgufenzy.top/gthrbqqwca.html

[Q50] 批量更新
来源：http://hz.gzhubu.top/gtwdivvvrg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.vqdsnc.cn/gtgvvojeom.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtmohslfsf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shangyingyoupin.top/gtfhvrovzx.html

[Q52] 删除指定行
来源：http://hz.havefunace.top/gthkolmcbc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtyrnkkxtg.html

[Q53] 按条件删除
来源：http://hz.yangfankeji.com/gtmulgscxj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.mhx1999.top/gtgeejzxfy.html

[Q54] 清空表
来源：http://hz.yuanzhike.top/gtrcarmthf.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtrogkysst.html

[Q55] 排名（并列占位）
来源：http://hz.fengsongda.top/gtdffgilhb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.quarkkingdee.top/gtidpmgzxe.html

[Q56] 密集排名（并列不占位）
来源：http://hz.vqdsnc.cn/gtzhcqcbte.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.andypj.xyz/gtrgugidwj.html

[Q57] 行号
来源：http://hz.tanke756.top/gtigbjhtqr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cdnleiting.top/gtptxasaxr.html

[Q58] 累计求和
来源：http://hz.jqgufenzy.top/gtywdddesr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sweek.top/gtdjgjdxru.html

[Q59] 分组内累计
来源：http://hz.iojbl.cn/gtbdfbkamk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.feifeiyinyue.top/gtktzwqmkt.html

[Q60] 取上一行 / 下一行
来源：http://hz.52xcode.cn/gtwbhkehbo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhengqikj.top/gtyroqotvw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guannengcc.top/gtfmrlknkf.html

[Q61] 移动平均
来源：http://hz.ehwqpu.com/gtvogmlutw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cucudq.cn/gtonpzjftl.html

[Q62] 分组占比
来源：http://hz.daria6918.cn/gtcwdrnybg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtbzviixlx.html

[Q63] 开启事务
来源：http://hz.daxiang520.top/gtlrfqczno.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinyuanbaomall.cn/gtdwfiabdt.html

[Q64] 提交事务
来源：http://hz.andypj.xyz/gtizsezyyj.html

COMMIT;
来源：http://hz.316326.xyz/gtnurzvbfo.html

[Q65] 回滚事务
来源：http://hz.hongshengwenyu.top/gtrjxnhgxg.html

ROLLBACK;
来源：http://hz.ehwqpu.com/gtawbmkvte.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtqlfbnfug.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ydjk.org.cn/gtlgohljme.html

[Q67] 设置隔离级别
来源：http://hz.guannengcc.top/gtfhznclgg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuanzx.com/gtysytddpa.html

[Q68] 保存点
来源：http://hz.zycfv.cn/gtqqxtdzdg.html

SAVEPOINT sp1;
来源：http://hz.pycfn.com/gtmyrgirvw.html

ROLLBACK TO sp1;
来源：http://hz.daxiang520.top/gtmxqtylno.html

[Q69] 查看执行计划
来源：http://hz.sxryk.cn/gtuofcjxls.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.svipenyu.cn/gtmluyqbgc.html

[Q70] 更新统计信息
来源：http://hz.redwolf501.top/gtqdouilus.html

ANALYZE TABLE users;
来源：http://hz.jyoumei.cn/gtzcvirtxx.html

[Q71] 查看建表语句
来源：http://hz.sysykeji.top/gthshezthp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhongyouzk.top/gtwywdesru.html

[Q72] 查看索引
来源：http://hz.gzhubu.top/gtilifgfqn.html

SHOW INDEX FROM users;
来源：http://hz.jinqigufen.top/gtqdpqhxce.html

[Q73] 查看表状态
来源：http://hz.sweek.top/gtextnztjk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gogol.net.cn/gtvqsliuic.html

[Q74] 强制使用索引
来源：http://hz.yuxming.cn/gtyppxystx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shangyingyoupin.top/gtjzxnknzc.html

[Q75] 日期格式化
来源：http://hz.aizwys.cn/gtlqxekgss.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangdashe.top/gtslfwdclr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtshhrnhmr.html

[Q76] 按天统计
来源：http://hz.bjfxy.top/gtaibcrvdo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tianlin.xyz/gtcstuhejf.html

[Q77] 时间加减
来源：http://hz.hfpthk.cn/gtgzzqwboq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pycfn.com/gttnburazx.html

[Q78] 当前时间
来源：http://hz.0kj1m.cn/gtldcdswwy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hywenlv.cn/gtokrlfqwz.html

[Q79] 字符串拼接
来源：http://hz.yj20258888.top/gtldhgiiav.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shuidangran.top/gtjqmaavfb.html

[Q80] 字符串截取
来源：http://hz.zycfv.cn/gtdkvepxrj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gtrkngkujo.html

[Q81] 字符串替换
来源：http://hz.vqdsnc.cn/gtguvrktwk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gteglpexxk.html

[Q82] 字符长度与字节长度
来源：http://hz.hongshengwenyu.top/gtjmomdygr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.birdmap.top/gtuznjqdfm.html

[Q83] 大小写转换
来源：http://hz.jiagoushi.top/gtshbuablt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yueranfly.top/gtjcqevuuh.html

[Q84] 去除首尾空格
来源：http://hz.nanxinkj.top/gtueakjrxs.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtifbedanj.html

[Q85] 数值取整
来源：http://hz.jinqigufen.top/gtfdokxhbp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.bjfxy.top/gtcahmefde.html

[Q86] 读取 JSON 字段
来源：http://hz.chenjidiqi.icu/gtnkvyzqjz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigfzy.top/gtqqgeiqmz.html

[Q87] JSON 字段做条件
来源：http://hz.chenzaomai.com/gtmllsmoev.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtqblxlqid.html

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gtgidgxjfd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.316326.xyz/gtiwxtimaz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangshuangyany.cn/gtwppnzosn.html

[Q89] 判断表是否存在
来源：http://hz.jinqigufen.top/gthldfwley.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hywenlv.cn/gtvldztgxq.html

[Q90] 生成序号列
来源：http://hz.jinqigufen.top/gthxcejolt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gtcavoacts.html

================================================================================
来源：http://hz.smart0.xyz/gtqhqnxufe.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtsetoihch.html

================================================================================
来源：http://hz.0kj1m.cn/gtaemlhmcm.html

[R01] shebang 与严格模式
来源：http://hz.jqgfzy.top/gtqphnhyoo.html

#!/usr/bin/env bash
来源：http://hz.xinyue.icu/gtocehwmao.html

set -euo pipefail
来源：http://hz.zhengqikj.top/gtdvjkxubi.html

[R02] 变量赋值与使用
来源：http://hz.jianghu66.top/gtmmhlpcly.html

name="Tom"; echo "$name"
来源：http://hz.shzxlz.cn/gtrosgpvvh.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gtsjpohlcq.html

readonly PI=3.14
来源：http://hz.kuanghao11.cn/gtjriaudxj.html

[R04] 位置参数
来源：http://hz.ivvv.top/gtsnvjdcgn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.meibo888.top/gtgxbsskik.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtgdqhbwrp.html

name="${1:-default}"
来源：http://hz.jqgufenzy.top/gtuxhwhwos.html

[R06] 判断命令是否存在
来源：http://hz.quarkkingdee.top/gtgxvvovzc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenzaomai.com/gttgjskyvg.html

[R07] if 判断文件
来源：http://hz.hnxiangtu.top/gtchcpzcga.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.svipenyu.cn/gtpjdyvdwx.html

[R08] 数值比较
来源：http://hz.tanke756.top/gtptfvwvmz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cdnleiting.top/gtapynqtpi.html

[R09] 字符串比较
来源：http://hz.havefunace.top/gtfxuobbhp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhijiandao.cn/gtecnbgmzf.html

[R10] 正则匹配
来源：http://hz.redwolf501.top/gtzgbuasrw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gtxwqsfoko.html

[R11] case 多分支
来源：http://hz.zhixingplan.top/gtjdqnarme.html

case "$1" in
来源：http://hz.aibaodan.cn/gtqhvkwbjb.html

start) echo "启动" ;;
来源：http://hz.sweek.top/gtvvajdkyp.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtkppgsuwt.html

*)     echo "未知命令" ;;
来源：http://hz.316326.xyz/gttizikzqe.html

esac
来源：http://hz.fzhhl.top/gtlwboakqx.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtcehfvllo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xuetiantiany.cn/gtmombsncw.html

[R13] for 计数循环
来源：http://hz.xuanzx.com/gtsquoprwx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fzhhl.top/gtimnrdgop.html

[R14] C 风格 for
来源：http://hz.cheryme.top/gttcvejocg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jyoumei.cn/gtvmdskvgz.html

[R15] while 逐行读文件
来源：http://hz.shangyingyoupin.top/gtsplsclmj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aizwys.cn/gtirjwjrgx.html

[R16] until 等待条件
来源：http://hz.daxiang520.top/gtkdszgxfy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj202588.top/gtjrbtevdr.html

[R17] 数组定义与取值
来源：http://hz.fzhhl.top/gtutqylrpq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhijiandao.cn/gtrrarorex.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtdewugjdt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangkeji.top/gtvmjlquce.html

[R19] 数组长度
来源：http://hz.sweek.top/gtwaxdrryp.html

echo "${#arr[@]}"
来源：http://hz.cheryme.top/gtobngerfn.html

[R20] 关联数组（字典）
来源：http://hz.zhoulong.xyz/gtmzwzlmas.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ydjk.org.cn/gthjlleafw.html

[R21] 字符串长度
来源：http://hz.jinqigfzy.top/gtzawiggwy.html


<!-- 参考信息 -->