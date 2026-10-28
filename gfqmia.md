代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jiagoushi.top/gtlmcvvleh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hongshengwenyu.top/gtmuosxxnk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtnymxwrxw.html

[P04] 求长度
来源：http://hz.yj20258.top/gtchrvttga.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gthvuzczuy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gtyyjhzddo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.iojbl.cn/gtctihvzxk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtkelnqkmi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cashguo.top/gtkfttttbo.html

Go:   len(arr);  len(m)
来源：http://hz.dianchejie.cn/gtjbzhmmjt.html

Ruby: x.length;  x.size
来源：http://hz.ywan-chungtsiang.top/gtgprxrvii.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shuidangran.top/gtlmdmymzw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtajzhajlb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.feifeiyinyue.top/gthyzykqgx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sweek.top/gtocfwznad.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guannengcc.top/gtyiwuhrer.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtjcvdmdng.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinyuanbaomall.cn/gtytvedquc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuanzx.com/gtbcpakbvl.html

Ruby: a == b
来源：http://hz.shangyingyoupin.top/gtswckxvbo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangdashe.top/gtaepxmtnp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aizwys.cn/gtlosibauu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dashuyun.cn/gtbqvnobts.html

PHP:  if (empty($x)) {}
来源：http://hz.ybcxt.top/gtirwwsitx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinghuilouyu.cn/gtxbovpcys.html

TS:   if (x == null) {}
来源：http://hz.zhijiandao.cn/gtvdenbylh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtxwwtskgy.html

Go:   if x == nil {}
来源：http://hz.yueranfly.top/gtccvklmoi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtomyxktcp.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtnjbuuuku.html

[P07] 防抖与节流
来源：http://hz.aizwys.cn/gtvnwghqkx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtsbycbfyx.html

PHP:  // 手写时间戳比较
来源：http://hz.yongpay.top/gtsqhmbdcp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtlzusrbbr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtrzmkfqkd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuanzhike.top/gttwhnhqwe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aibaodan.cn/gtismobejh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gtkahihwyy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yongpay.top/gtndmedowo.html

[P08] 处理浮点精度问题
来源：http://hz.yueranfly.top/gtldiyhaag.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinyuanbaomall.cn/gtfmobztzc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.redwolf501.top/gtzmvugwvd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hammf.cn/gthqemorhf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.316326.xyz/gtkzbogyoc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sxryk.cn/gtfavmjipu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtcesovsfz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtqeikfbjt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hongshengwenyu.top/gtndbcochk.html

================================================================================
来源：http://hz.jiagoushi.top/gtazobgste.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gtxkhproqr.html

================================================================================
来源：http://hz.yongpay.top/gtxrcgsegb.html

[Q01] 创建表
来源：http://hz.zdqjudy.top/gtrighjhpf.html

CREATE TABLE users (
来源：http://hz.jiagoushi.top/gtjlvooeas.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtcnqtqfrg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ppjwa.cn/gthghlecgk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.andypj.xyz/gtbshlhfab.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fzhhl.top/gtapxcmurl.html

);
来源：http://hz.jlsjyb.cn/gthxfxmnnd.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtwbavkaik.html

CREATE TABLE orders (
来源：http://hz.tian-w.cn/gtxrojagui.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtzvphgmli.html

user_id INT NOT NULL,
来源：http://hz.c1oappe.top/gtvcidihsn.html

amount DECIMAL(10, 2),
来源：http://hz.aizwys.cn/gtuaoqcxkv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shangyingyoupin.top/gtadmgcdqk.html

);
来源：http://hz.dianchejie.cn/gtdywdhjcr.html

[Q03] 增加列
来源：http://hz.zhengqikj.top/gtcaoeiajn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangkeji.top/gthrodfzky.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtmxnpwnzq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtqwwfzvrg.html

[Q05] 重命名列
来源：http://hz.cqqwz.cn/gtpjwddldx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dianchejie.cn/gtghgmgayl.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtfdgihzzh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhixingplan.top/gtyauqavyj.html

[Q07] 删除表
来源：http://hz.sxryk.cn/gtimxeqnez.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zycfv.cn/gtfzmowyvv.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtojavurtp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fengsongda.top/gthokgclmz.html

[Q09] 创建唯一索引
来源：http://hz.fzhhl.top/gtrpwqeozh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.birdmap.top/gtvkcmdpoh.html

[Q10] 插入单行
来源：http://hz.yanxiufei.cn/gtufvdyawv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhijiandao.cn/gtgmoyqfcf.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtlmolqytl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.9152youxi.cn/gtltbvkqok.html

[Q12] 插入后取自增 ID
来源：http://hz.hammf.cn/gtyxrinksb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hongshengwenyu.top/gtntznhxzf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangshuangyany.cn/gthjagkvfa.html

[Q13] 忽略重复插入
来源：http://hz.zdqjudy.top/gtfeesiwit.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gtxcyuizvv.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gtoqrvdnfm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.c1oappe.top/gtxsmnuwlk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xingfuxueyuan.xyz/gtrysyduuv.html

[Q15] 查询全部
来源：http://hz.xziqi.cn/gtzmetncpf.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtyhtbamdr.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtciwudzkl.html

SELECT id, name FROM users;
来源：http://hz.gzhubu.top/gtnhcgsdvz.html

[Q17] 条件查询
来源：http://hz.yueranfly.top/gtmsnntgqx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yangfankeji.com/gtaoottuff.html

[Q18] 模糊匹配
来源：http://hz.sufxvd.cn/gtrpbqvniq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yvedp.cn/gtwqtfswoi.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtpybudxlw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.andypj.xyz/gtkuiumzfy.html

[Q20] IN 列表
来源：http://hz.ppjwa.cn/gtydzlzere.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nanxuanxn.top/gtexgezjac.html

[Q21] 空值判断
来源：http://hz.hongshengwenyu.top/gtzuryjjqf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuxming.cn/gtwgxfepxn.html

[Q22] 排序
来源：http://hz.hywenlv.cn/gttuwrbolt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinghuilouyu.cn/gtqvmvhabb.html

[Q23] 分页
来源：http://hz.shanyushiyangkeji.top/gtxslxabgg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtxckyafre.html

[Q24] 去重
来源：http://hz.gzhubu.top/gtmiocvtgb.html

SELECT DISTINCT city FROM users;
来源：http://hz.andypj.xyz/gtqujeuhnt.html

[Q25] 只取前 N 条
来源：http://hz.haohaochexian.top/gtccayhksc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gtjqyyhlev.html

[Q26] 计数
来源：http://hz.mhx1999.top/gtrxvjsaej.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhongyouzk.top/gtnjesllqy.html

[Q27] 条件计数
来源：http://hz.hongshengwenyu.top/gtfkxxrbev.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nwbrower.top/gtvucqvwxr.html

[Q28] 求和与平均
来源：http://hz.316326.xyz/gterdnzhej.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigufen.top/gtggrpwfrc.html

[Q29] 最大最小值
来源：http://hz.hysaishi.cn/gtpjvcnycx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jyoumei.cn/gthauhabla.html

[Q30] 分组统计
来源：http://hz.zhixingplan.top/gtmxsvqbim.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtczyvktyb.html

[Q31] 分组后过滤
来源：http://hz.ppjwa.cn/gtsruhajep.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhaomingkeji.xyz/gtdswyztry.html

[Q32] 分组拼接字符串
来源：http://hz.yanxiufei.cn/gtlhazimbo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtdtigbnyr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenzaomai.com/gtyvayugfq.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtbaqdnvvs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.fengsongda.top/gtrgobtknz.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtiwiqwkzs.html

SELECT * FROM (
来源：http://hz.kuanghao11.cn/gtblmztdag.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.kuanghao11.cn/gtyqspynki.html

) t WHERE rn = 1;
来源：http://hz.xylfe.cn/gtiqqonkmz.html

[Q35] 内连接
来源：http://hz.hfpthk.cn/gtqmdqskau.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtppkxybke.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gtqmbwbihe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtwmbxadak.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gtdmqyypst.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258888.top/gttyspcuci.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tanke756.top/gtmtmdclnn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ybcxt.top/gtnziansdt.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtofkvjskk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtdgabrizb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gtfallrfdv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cheryme.top/gtctncjiqh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuetiantiany.cn/gtwxroymyd.html

[Q41] 多表连接
来源：http://hz.wangshuangyany.cn/gtkndtyidi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shzxlz.cn/gtpcvjdnxt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shangyingyoupin.top/gtxjkqbupo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.mhx1999.top/gtrhupxnjg.html

[Q42] 连接条件附加过滤
来源：http://hz.svipenyu.cn/gtuvrycluz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhiwuduotai.top/gtzrrcwhwl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ywan-chungtsiang.top/gttrtjtezj.html

[Q43] 标量子查询
来源：http://hz.jinghuilouyu.cn/gtrkqnfdar.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yangfankeji.com/gtspikvrau.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gtkmwwghft.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigufen.top/gtkpdtbity.html

[Q45] EXISTS 判断存在
来源：http://hz.ywan-chungtsiang.top/gtsajesvwu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtrmpmqxna.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinyuanbaomall.cn/gtkemghwcn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtbuycyknz.html

[Q47] 与平均值比较
来源：http://hz.nanxinkj.top/gtipvkkkke.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tian-w.cn/gtbgdnssnw.html

[Q48] CTE 公用表表达式
来源：http://hz.nanxuanxn.top/gtjehaqtmp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgufenzy.top/gtfihcbddx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtsnkkvhga.html

[Q49] 更新单行
来源：http://hz.chenjidiqi.icu/gtdedpirml.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhixingplan.top/gtpaaelmoz.html

[Q50] 批量更新
来源：http://hz.wangshuangyany.cn/gtbngfsioi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hfpthk.cn/gtrxtmrtum.html

[Q51] 用子查询更新
来源：http://hz.shanyushiyangkeji.top/gtkgcrxrja.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hfpthk.cn/gthttkszhv.html

[Q52] 删除指定行
来源：http://hz.jinyuanbaomall.cn/gtvqpgfumo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.snrcjt.cn/gtruccegxt.html

[Q53] 按条件删除
来源：http://hz.zhongyouzk.top/gtpocjzxcg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangkeji.top/gtpavtzbua.html

[Q54] 清空表
来源：http://hz.shzxlz.cn/gtjfqhhkkb.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gtrbpsfaxn.html

[Q55] 排名（并列占位）
来源：http://hz.jianghu66.top/gtgzorxyzm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.andypj.xyz/gtdbrjirsp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gzhubu.top/gtkffxygof.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuanzx.com/gtaiprqiad.html

[Q57] 行号
来源：http://hz.9152youxi.cn/gtvjhmablt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.quarkkingdee.top/gtsstycogn.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gtfpvmdxsk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.kuanghao11.cn/gtfvvnieyn.html

[Q59] 分组内累计
来源：http://hz.dianchejie.cn/gtsaldqmtc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fzhhl.top/gtyuoybyrm.html

[Q60] 取上一行 / 下一行
来源：http://hz.xingfuxueyuan.xyz/gtumjhjzgk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtzeotbgdf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yongpay.top/gtdocpvdzu.html

[Q61] 移动平均
来源：http://hz.aibaodan.cn/gtsecwuemf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.kuanghao11.cn/gtahrgyjle.html

[Q62] 分组占比
来源：http://hz.havefunace.top/gtsdltxacp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtwlwdqpkh.html

[Q63] 开启事务
来源：http://hz.shuidangran.top/gtqhiyhljo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.c1oappe.top/gtuchoclov.html

[Q64] 提交事务
来源：http://hz.daria6918.cn/gtbuawebdc.html

COMMIT;
来源：http://hz.jianghu66.top/gtonizywbd.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtaltuejzo.html

ROLLBACK;
来源：http://hz.hammf.cn/gtaddballq.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangkeji.top/gtguyxmzcb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ydzc1.top/gtlrojiovd.html

[Q67] 设置隔离级别
来源：http://hz.hongshengwenyu.top/gtvfwhuyrj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yanxiufei.cn/gtjcgrzuwt.html

[Q68] 保存点
来源：http://hz.hammf.cn/gtqlahjvef.html

SAVEPOINT sp1;
来源：http://hz.yj20258888.top/gtgvnfuhgt.html

ROLLBACK TO sp1;
来源：http://hz.mhx1999.top/gtymzgodoo.html

[Q69] 查看执行计划
来源：http://hz.xinyue.icu/gtrnptmgwm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hongshengwenyu.top/gtayffnwcu.html

[Q70] 更新统计信息
来源：http://hz.zhoulong.xyz/gtagckopqr.html

ANALYZE TABLE users;
来源：http://hz.cqqwz.cn/gtdgrbfqdo.html

[Q71] 查看建表语句
来源：http://hz.yvedp.cn/gtffwlhsad.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yuanzhike.top/gtwjichpde.html

[Q72] 查看索引
来源：http://hz.hnqzz.top/gthfkhqtrb.html

SHOW INDEX FROM users;
来源：http://hz.dashuyun.cn/gtfvhccttu.html

[Q73] 查看表状态
来源：http://hz.hammf.cn/gtesqejkqd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.bjfxy.top/gtuvsoyltq.html

[Q74] 强制使用索引
来源：http://hz.hfpthk.cn/gtpmkzthli.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hammf.cn/gtcxpmwlat.html

[Q75] 日期格式化
来源：http://hz.aibaodan.cn/gtprogoydl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtrnehimnb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gttozvjncb.html

[Q76] 按天统计
来源：http://hz.yangfankeji.com/gtlksojxqq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gotoacloud.top/gtzwuutibt.html

[Q77] 时间加减
来源：http://hz.fzhhl.top/gtntlbhmsa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtcmznxbsk.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gtunbctxkn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.feifeiyinyue.top/gtzdxkymfd.html

[Q79] 字符串拼接
来源：http://hz.aizwys.cn/gtejhtmtcm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yueranfly.top/gtxwnilbuk.html

[Q80] 字符串截取
来源：http://hz.jyoumei.cn/gtzecmqkqs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.52xcode.cn/gtkgzmisjc.html

[Q81] 字符串替换
来源：http://hz.xinyue.icu/gthreucose.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sysykeji.top/gtdvhkrsly.html

[Q82] 字符长度与字节长度
来源：http://hz.0kj1m.cn/gtatynhzmn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zdqjudy.top/gtmtspldzl.html

[Q83] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtbrxkvolz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hammf.cn/gtterhwkzr.html

[Q84] 去除首尾空格
来源：http://hz.jlsjyb.cn/gtcxkfdbmz.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtkoxdluhm.html

[Q85] 数值取整
来源：http://hz.gaohongyu789.top/gtrdshtsml.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtvytveofg.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtajlasdnp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.9152youxi.cn/gtfvncnhfh.html

[Q87] JSON 字段做条件
来源：http://hz.nanxuanxn.top/gtphuhkxmg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cqqwz.cn/gtwfazvepo.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtnbcklcdo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtxlhabxap.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fzhhl.top/gtqnjawthr.html

[Q89] 判断表是否存在
来源：http://hz.gotoacloud.top/gtdzkyzbad.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnqzz.top/gtsrshdxgv.html

[Q90] 生成序号列
来源：http://hz.zhongyouzk.top/gtfzsggqyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhengqikj.top/gtxkcnxmbd.html

================================================================================
来源：http://hz.jqgfzy.top/gtxtveypaz.html

R. Bash 专题
来源：http://hz.dashuyun.cn/gtjjnixfgi.html

================================================================================
来源：http://hz.chenzaomai.com/gtvlfwvfta.html

[R01] shebang 与严格模式
来源：http://hz.sufxvd.cn/gtrgflqroi.html

#!/usr/bin/env bash
来源：http://hz.yj20258.top/gtwdpokjux.html

set -euo pipefail
来源：http://hz.hnqzz.top/gtwlyhoebg.html

[R02] 变量赋值与使用
来源：http://hz.sufxvd.cn/gtrukupisq.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gtjjsvqmsj.html

[R03] 只读变量
来源：http://hz.ivvv.top/gtfaqtrpmf.html

readonly PI=3.14
来源：http://hz.daxiang520.top/gtbapmkyia.html

[R04] 位置参数
来源：http://hz.svipenyu.cn/gtvnvnlgas.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cqqwz.cn/gtanhmzple.html

[R05] 参数默认值
来源：http://hz.hnxiangtu.top/gtbksysvdy.html

name="${1:-default}"
来源：http://hz.ivvv.top/gtjqndccwt.html

[R06] 判断命令是否存在
来源：http://hz.smart0.xyz/gtfdpvqhfr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sysykeji.top/gthbubxlpz.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtisbszpmg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangdashe.top/gtsywbceqq.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtfffzgojg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hfpthk.cn/gtqtpjhqbm.html

[R09] 字符串比较
来源：http://hz.xuanzx.com/gtpaszhbtj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtueypjdgd.html

[R10] 正则匹配
来源：http://hz.9152youxi.cn/gtrpbnrpxk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtqadbfqot.html

[R11] case 多分支
来源：http://hz.cucudq.cn/gtbxlsjhlh.html

case "$1" in
来源：http://hz.yuanzhike.top/gthnqabimg.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gtuwgmjpff.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gtlzmlband.html

*)     echo "未知命令" ;;
来源：http://hz.pycfn.com/gtbxexmcsw.html

esac
来源：http://hz.zhongyouzk.top/gtavrhvwmy.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtsskkfcba.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigufen.top/gtyelkpool.html

[R13] for 计数循环
来源：http://hz.bjfxy.top/gthcihfwch.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtetpfibth.html

[R14] C 风格 for
来源：http://hz.birdmap.top/gtbkjqrnbz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zdqjudy.top/gtygknfchk.html

[R15] while 逐行读文件
来源：http://hz.ivvv.top/gtlqlouclk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gaohongyu789.top/gtqgucafsj.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gttljyrxyn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gtrfvvftqr.html

[R17] 数组定义与取值
来源：http://hz.zhaomingkeji.xyz/gthnalckod.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guowangkeji.top/gtthwwbpfy.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gtckayfjmj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gtiuwypyfy.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtxbiuhxgi.html


<!-- 参考信息 -->