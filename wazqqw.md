代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuetiantiany.cn/gtofuewfjg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sweek.top/gtnllmkvvp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinyuanbaomall.cn/gtufmidlws.html

[P04] 求长度
来源：http://hz.chenlongwang.top/gtmckhegtf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtznrbjrfe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtuaaeligg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtzmzzejtw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtmeidnmgh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtqnarnzwl.html

Go:   len(arr);  len(m)
来源：http://hz.zdqjudy.top/gtzzndxvsu.html

Ruby: x.length;  x.size
来源：http://hz.sxryk.cn/gtwuwxilhm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cheryme.top/gtlkqhniwg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gttnbfnpmk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yangfankeji.com/gtrydlhyrx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnxiangtu.top/gtrbteehva.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxuanxn.top/gtoarvgqsc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258.top/gtekpwsvbd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hammf.cn/gttrbyogou.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yongpay.top/gthhfdetzi.html

Ruby: a == b
来源：http://hz.shanyushiyangkeji.top/gtmahmuwqt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhiwuduotai.top/gtjgyamorz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ivvv.top/gtrnasuvno.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yvedp.cn/gtqijricml.html

PHP:  if (empty($x)) {}
来源：http://hz.kuanghao11.cn/gtyjpjaibl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cashguo.top/gtprlgvwxj.html

TS:   if (x == null) {}
来源：http://hz.chenzaomai.com/gtfsmojjfk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gtklztozhf.html

Go:   if x == nil {}
来源：http://hz.hysaishi.cn/gtdlxtvuqj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ywan-chungtsiang.top/gtpsrktgpq.html

C#:   if (x is null) {}
来源：http://hz.wangdashe.top/gtxrxkpgdc.html

[P07] 防抖与节流
来源：http://hz.mhx1999.top/gtulvszeuq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtaajmtzeq.html

PHP:  // 手写时间戳比较
来源：http://hz.shzxlz.cn/gtlbayjvgu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtjntrsdiq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtejbcedkz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.0kj1m.cn/gthudivaud.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ehwqpu.com/gtxlneibdc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yanxiufei.cn/gtodolcfiu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daria6918.cn/gtyejywkiu.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gtiwnanxpj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtztijpogp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhaomingkeji.xyz/gtnolacinj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.meibo888.top/gtvodkhbdl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtqwcgvggr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zycfv.cn/gtmxvkkvik.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhoulong.xyz/gtnpqqdusv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ehwqpu.com/gtksajzqdm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nwbrower.top/gtyeoiodgl.html

================================================================================
来源：http://hz.fzhhl.top/gtvgozromp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zycfv.cn/gtsjzqohur.html

================================================================================
来源：http://hz.gaohongyu789.top/gtgidqboed.html

[Q01] 创建表
来源：http://hz.hysaishi.cn/gtzdmcwgqr.html

CREATE TABLE users (
来源：http://hz.yangfankeji.com/gtzvayvwgd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtpjzhydlv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hnxiangtu.top/gtvwuqqwni.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xylfe.cn/gtrjtbskfb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhoulong.xyz/gtelonzwbk.html

);
来源：http://hz.0kj1m.cn/gtpkvzdnwp.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gtwwczzhux.html

CREATE TABLE orders (
来源：http://hz.tianlin.xyz/gtsutrnadm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtshevjqal.html

user_id INT NOT NULL,
来源：http://hz.jinghuilouyu.cn/gthetfhjph.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtivdzmvzw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jiagoushi.top/gtedmwbats.html

);
来源：http://hz.jianghu66.top/gtzzufffkc.html

[Q03] 增加列
来源：http://hz.c1oappe.top/gtcwtusbwm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtovsupdwp.html

[Q04] 修改列类型
来源：http://hz.nanxinkj.top/gtklauuept.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xingfuxueyuan.xyz/gtdpfrfbbm.html

[Q05] 重命名列
来源：http://hz.ywan-chungtsiang.top/gtindeqehb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtxuwikfth.html

[Q06] 删除列
来源：http://hz.dianchejie.cn/gtucuqhabe.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gotoacloud.top/gtghmipmdu.html

[Q07] 删除表
来源：http://hz.wangdashe.top/gtfqsndjro.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aizwys.cn/gtoksnsyuv.html

[Q08] 创建普通索引
来源：http://hz.wangshuangyany.cn/gtndqadfws.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtlxmmlwtt.html

[Q09] 创建唯一索引
来源：http://hz.ydjk.org.cn/gthykhixsj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.birdmap.top/gtavwytbdo.html

[Q10] 插入单行
来源：http://hz.zhiwuduotai.top/gtrarcgkzw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hongshengwenyu.top/gtxplnjxsm.html

[Q11] 一次插入多行
来源：http://hz.kuanghao11.cn/gtajtwwnni.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenzaomai.com/gtmjyjidam.html

[Q12] 插入后取自增 ID
来源：http://hz.ivvv.top/gtrvjafxrz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.tian-w.cn/gtzbolahmg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtkqtkepyi.html

[Q13] 忽略重复插入
来源：http://hz.tian-w.cn/gtccfpsbzg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.haohaochexian.top/gtzxrzpfpm.html

[Q14] 存在则更新（upsert）
来源：http://hz.316326.xyz/gtspnezxdu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.andypj.xyz/gtvdgbuhqk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258.top/gtqqsacoby.html

[Q15] 查询全部
来源：http://hz.zhengqikj.top/gtjjgizzat.html

SELECT * FROM users;
来源：http://hz.snrcjt.cn/gtxxymfknj.html

[Q16] 查询指定列
来源：http://hz.hnqzz.top/gtzdenkqty.html

SELECT id, name FROM users;
来源：http://hz.xingfuxueyuan.xyz/gttnpwguir.html

[Q17] 条件查询
来源：http://hz.aizwys.cn/gtpurycooj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sweek.top/gtciilwlqi.html

[Q18] 模糊匹配
来源：http://hz.fzhhl.top/gtytnqyreu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.meibo888.top/gtetaibdhg.html

[Q19] 范围查询
来源：http://hz.tian-w.cn/gtdiawlcvl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nwbrower.top/gtumtdslmc.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gtjrkmhrkg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtquudpnbu.html

[Q21] 空值判断
来源：http://hz.shzxlz.cn/gtjlubrqxs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.smart0.xyz/gtolyahslp.html

[Q22] 排序
来源：http://hz.iojbl.cn/gtbiwgselx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tian-w.cn/gtszlexcbv.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtqkkwaehv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daria6918.cn/gthcfkokah.html

[Q24] 去重
来源：http://hz.hysaishi.cn/gtlsixzsbk.html

SELECT DISTINCT city FROM users;
来源：http://hz.0kj1m.cn/gtxjfiywfh.html

[Q25] 只取前 N 条
来源：http://hz.pycfn.com/gtzrjkvbmz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cashguo.top/gtumunkpuv.html

[Q26] 计数
来源：http://hz.zhijiandao.cn/gtmnfozjkx.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxinkj.top/gtscawprzo.html

[Q27] 条件计数
来源：http://hz.ivvv.top/gtbpuuvfmg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sxryk.cn/gtmekwqxje.html

[Q28] 求和与平均
来源：http://hz.pycfn.com/gtziyjgbmu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shzxlz.cn/gtqjfumsga.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gtygdikjbn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.guowangkeji.top/gtuhwtwqse.html

[Q30] 分组统计
来源：http://hz.yj202588.top/gtowqdbfqy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtrqlvsrpc.html

[Q31] 分组后过滤
来源：http://hz.ivvv.top/gtietcibqj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gtxhgjembf.html

[Q32] 分组拼接字符串
来源：http://hz.sxryk.cn/gtxijuilai.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtpmkroeql.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhaomingkeji.xyz/gtdztomfaz.html

[Q33] 多列分组
来源：http://hz.jlsjyb.cn/gtfsismanv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shzxlz.cn/gtcykpjjyw.html

[Q34] 每组取第一条
来源：http://hz.jqgufenzy.top/gtayuuqfko.html

SELECT * FROM (
来源：http://hz.sufxvd.cn/gtebnnplzy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinghuilouyu.cn/gthnpzscjo.html

) t WHERE rn = 1;
来源：http://hz.pengpengdd.cyou/gtoltxalme.html

[Q35] 内连接
来源：http://hz.yvedp.cn/gtoqlofroq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtsslqfihi.html

[Q36] 左连接
来源：http://hz.0kj1m.cn/gtukotexra.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtsxcfmssq.html

[Q37] 右连接
来源：http://hz.iojbl.cn/gtzqdzualc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cheryme.top/gtkhqguwlf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.52xcode.cn/gtjlcjipsh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.snrcjt.cn/gtvmyvrcar.html

[Q39] 自连接（查上下级）
来源：http://hz.zhiwuduotai.top/gtnkgwggof.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj20258888.top/gttpucuqkz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hfpthk.cn/gtxzbkvoxi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtkbxtlwkf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gotoacloud.top/gtvbkeeeks.html

[Q41] 多表连接
来源：http://hz.zhixingplan.top/gtvockduon.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tanke756.top/gtyzvwzqei.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yueranfly.top/gtktxhfyrc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zycfv.cn/gttwoekrar.html

[Q42] 连接条件附加过滤
来源：http://hz.hammf.cn/gtndimhyea.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nanxinkj.top/gttzxvlucy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenzaomai.com/gtnuovgyxb.html

[Q43] 标量子查询
来源：http://hz.jinqigfzy.top/gtrberxwlt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gtoczuknic.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gtnwyxleqf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.meibo888.top/gtlnfgswud.html

[Q45] EXISTS 判断存在
来源：http://hz.xylfe.cn/gtfdpsgzyb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.mhx1999.top/gtkwhkuzyj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangshuangyany.cn/gtfjejsawk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtigizeydt.html

[Q47] 与平均值比较
来源：http://hz.52xcode.cn/gtdjsujyem.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sysykeji.top/gtfrbzowiy.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtvlipaqgu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zdqjudy.top/gtcislcvrl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.bjfxy.top/gtnwulvoxi.html

[Q49] 更新单行
来源：http://hz.meibo888.top/gtjpnacfrd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yuxming.cn/gtchpzijrz.html

[Q50] 批量更新
来源：http://hz.zdqjudy.top/gtkugypfmb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nwbrower.top/gtxfeqpiob.html

[Q51] 用子查询更新
来源：http://hz.jianghu66.top/gtyoxtnsij.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xylfe.cn/gtsfermktw.html

[Q52] 删除指定行
来源：http://hz.shangyingyoupin.top/gtklwfxupl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtscevbeez.html

[Q53] 按条件删除
来源：http://hz.shuidangran.top/gtlkukwgkr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhiwuduotai.top/gtmapcrbxi.html

[Q54] 清空表
来源：http://hz.316326.xyz/gtvqsglzib.html

TRUNCATE TABLE logs;
来源：http://hz.cqqwz.cn/gthbauhxse.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtrjmwwydx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cashguo.top/gtbahoohqe.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhaomingkeji.xyz/gtvtyzvqhw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hammf.cn/gtqersqraz.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtgruevjum.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhongyouzk.top/gtrfoumynz.html

[Q58] 累计求和
来源：http://hz.svipenyu.cn/gtdhmgiduk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258888.top/gtkxrdfvzf.html

[Q59] 分组内累计
来源：http://hz.0kj1m.cn/gtffirbjmr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhijiandao.cn/gtslhxcvic.html

[Q60] 取上一行 / 下一行
来源：http://hz.c1oappe.top/gttkzwlegt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtwaqhaerm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuanzhike.top/gtqmojssjn.html

[Q61] 移动平均
来源：http://hz.dianchejie.cn/gtpsiqosrj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhengqikj.top/gtgpntwfyu.html

[Q62] 分组占比
来源：http://hz.yj202588.top/gtqpmpaslj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtyqdzrpbv.html

[Q63] 开启事务
来源：http://hz.shzxlz.cn/gtqjdfbryb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jqgufenzy.top/gtwbsbteup.html

[Q64] 提交事务
来源：http://hz.jinghuilouyu.cn/gttqazelcr.html

COMMIT;
来源：http://hz.nanxuanxn.top/gtrcecpjnw.html

[Q65] 回滚事务
来源：http://hz.jinqigfzy.top/gtpoceoqnp.html

ROLLBACK;
来源：http://hz.guannengcc.top/gtfktnqwty.html

[Q66] 行锁查询
来源：http://hz.yj202588.top/gtnstjnfip.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hywenlv.cn/gtljbpkdsm.html

[Q67] 设置隔离级别
来源：http://hz.zhoulong.xyz/gtcsuicemo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aibaodan.cn/gtquxzemcr.html

[Q68] 保存点
来源：http://hz.zdqjudy.top/gtbedvhvyw.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtmlohmbnh.html

ROLLBACK TO sp1;
来源：http://hz.svipenyu.cn/gttduhbtij.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtuspztwmy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.quarkkingdee.top/gtwzmdvdzf.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gtawvqvang.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtlhfnvfdo.html

[Q71] 查看建表语句
来源：http://hz.aizwys.cn/gtwilkovnq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yueranfly.top/gtuuwevgns.html

[Q72] 查看索引
来源：http://hz.yj20258888.top/gtynjoryec.html

SHOW INDEX FROM users;
来源：http://hz.zhaomingkeji.xyz/gtrqcsaljg.html

[Q73] 查看表状态
来源：http://hz.yanxiufei.cn/gtynzkhiqw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xuetiantiany.cn/gtcuiqzekl.html

[Q74] 强制使用索引
来源：http://hz.fengsongda.top/gtoakiuydh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daria6918.cn/gtfqnxlmzp.html

[Q75] 日期格式化
来源：http://hz.c1oappe.top/gtbwqgkbjp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.vqdsnc.cn/gtzqkucgbx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuxming.cn/gtblowyljh.html

[Q76] 按天统计
来源：http://hz.jyoumei.cn/gtfmldqogp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nanxuanxn.top/gtjnsbjcwv.html

[Q77] 时间加减
来源：http://hz.cheryme.top/gtdgwgjqsk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xylfe.cn/gtepuokqsp.html

[Q78] 当前时间
来源：http://hz.sufxvd.cn/gtskgjsgxr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yangfankeji.com/gtnyslqxun.html

[Q79] 字符串拼接
来源：http://hz.ydjk.org.cn/gtifmkdsco.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangshuangyany.cn/gtxbxkypyr.html

[Q80] 字符串截取
来源：http://hz.meibo888.top/gtcougjhju.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cdnleiting.top/gtjdnhwkqj.html

[Q81] 字符串替换
来源：http://hz.iojbl.cn/gtsmtxcsoy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ywan-chungtsiang.top/gtffkbyxfi.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gtpqssgjxc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtyubtjdse.html

[Q83] 大小写转换
来源：http://hz.guannengcc.top/gthgggzfur.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtjbahnsxu.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtehxoypxm.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhixingplan.top/gtofhfqsgx.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtlswdzrfw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtpwtihfsd.html

[Q86] 读取 JSON 字段
来源：http://hz.xylfe.cn/gtgzcpodkp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.birdmap.top/gtjszmtwao.html

[Q87] JSON 字段做条件
来源：http://hz.hnqzz.top/gtngllxtnj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gtvsfvfeqc.html

[Q88] 行转列（条件聚合）
来源：http://hz.sysykeji.top/gtyhakaxgx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jlsjyb.cn/gtliolnsen.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gtallxxqwe.html

[Q89] 判断表是否存在
来源：http://hz.hywenlv.cn/gtvinfqaex.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cqqwz.cn/gtqqazimgi.html

[Q90] 生成序号列
来源：http://hz.yuanzhike.top/gtnxoflsku.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fzhhl.top/gtpmrpqgck.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtftgrimwc.html

R. Bash 专题
来源：http://hz.kuanghao11.cn/gtnteluqyx.html

================================================================================
来源：http://hz.0kj1m.cn/gtduaseipd.html

[R01] shebang 与严格模式
来源：http://hz.chenlongwang.top/gtildxvzsa.html

#!/usr/bin/env bash
来源：http://hz.tanke756.top/gtqfbxzdif.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtetvfkmvo.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtkokaytoc.html

name="Tom"; echo "$name"
来源：http://hz.ppjwa.cn/gtgmfrsegz.html

[R03] 只读变量
来源：http://hz.jinghuilouyu.cn/gtfccemnci.html

readonly PI=3.14
来源：http://hz.svipenyu.cn/gttjedeior.html

[R04] 位置参数
来源：http://hz.guowangkeji.top/gtgzknaqjc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xziqi.cn/gtarboqdei.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtortgyzyp.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtlkvrbbse.html

[R06] 判断命令是否存在
来源：http://hz.xuanzx.com/gtnqlmlxnf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.0kj1m.cn/gtvcywtfyd.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gtcyjrlvfo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhongyouzk.top/gtoqzixglu.html

[R08] 数值比较
来源：http://hz.jqgfzy.top/gtssolhgut.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xylfe.cn/gteyvivvfj.html

[R09] 字符串比较
来源：http://hz.ydjk.org.cn/gtzdszlrlw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ybcxt.top/gtwghkkjhe.html

[R10] 正则匹配
来源：http://hz.jqgfzy.top/gtsajbvkii.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gogol.net.cn/gtrxeeempj.html

[R11] case 多分支
来源：http://hz.ivvv.top/gtkzxbodgp.html

case "$1" in
来源：http://hz.52xcode.cn/gtzulxjhqg.html

start) echo "启动" ;;
来源：http://hz.yj20258.top/gtdouwvocj.html

stop)  echo "停止" ;;
来源：http://hz.gaohongyu789.top/gtfmehqreb.html

*)     echo "未知命令" ;;
来源：http://hz.dashuyun.cn/gtulfwwxou.html

esac
来源：http://hz.cashguo.top/gtsqtdfypa.html

[R12] for 遍历文件
来源：http://hz.zycfv.cn/gtcbbsnbyj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangdashe.top/gtzkczzahk.html

[R13] for 计数循环
来源：http://hz.hongshengwenyu.top/gtzqogabai.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnqzz.top/gtpiyaovpx.html

[R14] C 风格 for
来源：http://hz.cdnleiting.top/gtmdhrexqh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtqtuiksyu.html

[R15] while 逐行读文件
来源：http://hz.guowangkeji.top/gttnrefvsu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daria6918.cn/gtdscalfsd.html

[R16] until 等待条件
来源：http://hz.zhoulong.xyz/gtlekvaxfw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cheryme.top/gtbggsaaeu.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangkeji.top/gttmyksres.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zycfv.cn/gtvnfiwoha.html

[R18] 遍历数组
来源：http://hz.yvedp.cn/gtgtgxnbua.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fzhhl.top/gtoauhdnwx.html

[R19] 数组长度
来源：http://hz.xziqi.cn/gtgqtzxzgc.html


<!-- 参考信息 -->