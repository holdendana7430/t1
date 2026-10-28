代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.9152youxi.cn/gtrfuzezxi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtrmtbgvav.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtfrmytpfk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtjgbhqrpb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yonumen.top/gtkuyrdqrk.html

Go:   len(arr);  len(m)
来源：http://hz.pycfn.com/gtfxdxajbv.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gttlqlcnsg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.aibaodan.cn/gtjefwjlmk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinqigufen.top/gtocwlcisb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xziqi.cn/gtvfcrvmto.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangkeji.top/gttvcghhjh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.c1oappe.top/gtppgordsz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtcggwldsl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.birdmap.top/gtbwisungf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cqqwz.cn/gtbcwdzdnv.html

Ruby: a == b
来源：http://hz.andypj.xyz/gtlxinkxdo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tianlin.xyz/gtjdfojthv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ivvv.top/gtcexkcneo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhongyouzk.top/gtnjbxylar.html

PHP:  if (empty($x)) {}
来源：http://hz.ydzc1.top/gtfpbuqgbw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ybcxt.top/gtpjvheajf.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtrsupooye.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pengpengdd.cyou/gtbateolbc.html

Go:   if x == nil {}
来源：http://hz.zhoulong.xyz/gtwzryrbov.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtfytslvtn.html

C#:   if (x is null) {}
来源：http://hz.haohaochexian.top/gthruzbkxx.html

[P07] 防抖与节流
来源：http://hz.yangfankeji.com/gtlyhoiavc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhaomingkeji.xyz/gtvyuhxprj.html

PHP:  // 手写时间戳比较
来源：http://hz.chenzaomai.com/gtiofoudtu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtphedrprc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtkflnpubq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj202588.top/gtxjkdrcpe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtobdolvdx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj202588.top/gtqinfqvzk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtiodrtumt.html

[P08] 处理浮点精度问题
来源：http://hz.hysaishi.cn/gtvsmsjrmv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nwbrower.top/gtonruujqw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenjidiqi.icu/gtioiwkser.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.vqdsnc.cn/gtpzougvcd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.redwolf501.top/gtwaqncoix.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cucudq.cn/gtxsfjqibc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zdqjudy.top/gtgaecqlje.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.snrcjt.cn/gtvjqsefly.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ivvv.top/gtyvamotmy.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtezbwcznh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ppjwa.cn/gtyhgsjprw.html

================================================================================
来源：http://hz.dashuyun.cn/gtmntdhyen.html

[Q01] 创建表
来源：http://hz.tian-w.cn/gtipsdvahz.html

CREATE TABLE users (
来源：http://hz.hnxiangtu.top/gtltdemwus.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtqmzdasdp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtnkiwxcqw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.havefunace.top/gtdhuygyix.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.bjfxy.top/gtxnbkfjad.html

);
来源：http://hz.svipenyu.cn/gtedonyjpt.html

[Q02] 创建带外键的表
来源：http://hz.ydjk.org.cn/gtrvkibriq.html

CREATE TABLE orders (
来源：http://hz.c1oappe.top/gtaupzforz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gotoacloud.top/gtyqnvehlt.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtudjpnqbl.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gtpzcwscrf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gogol.net.cn/gtollejqhh.html

);
来源：http://hz.vqdsnc.cn/gtjykcjvey.html

[Q03] 增加列
来源：http://hz.zycfv.cn/gtouyeujvd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sweek.top/gtvpdmnrph.html

[Q04] 修改列类型
来源：http://hz.vqdsnc.cn/gtbjcqsevu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xingfuxueyuan.xyz/gtbdiqrnol.html

[Q05] 重命名列
来源：http://hz.yvedp.cn/gtprcbmwjl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuxming.cn/gtdkhoybvx.html

[Q06] 删除列
来源：http://hz.cdnleiting.top/gtdrjlddzt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydjk.org.cn/gtyikwfebq.html

[Q07] 删除表
来源：http://hz.xuetiantiany.cn/gtmsrghabc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtjvpwhmho.html

[Q08] 创建普通索引
来源：http://hz.birdmap.top/gtzoidwkur.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yuxming.cn/gttdpslsjd.html

[Q09] 创建唯一索引
来源：http://hz.jianghu66.top/gticwvbyla.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.redwolf501.top/gttfvkerzx.html

[Q10] 插入单行
来源：http://hz.hysaishi.cn/gtriuhaegk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.bjfxy.top/gtdctbbyhk.html

[Q11] 一次插入多行
来源：http://hz.xziqi.cn/gttbbgbbfi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnxiangtu.top/gtjzisfpqr.html

[Q12] 插入后取自增 ID
来源：http://hz.nwbrower.top/gtjtwmvsup.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.52xcode.cn/gtanxerpfs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gthhkfpuet.html

[Q13] 忽略重复插入
来源：http://hz.jinqigufen.top/gtcejriyty.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.0kj1m.cn/gtylesikzl.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gtjnpompkp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.c1oappe.top/gtkjqffiuk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hnxiangtu.top/gtudurqzdl.html

[Q15] 查询全部
来源：http://hz.shangyingyoupin.top/gtahamzbgm.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtrcfvzayk.html

[Q16] 查询指定列
来源：http://hz.vqdsnc.cn/gtlxkbjclh.html

SELECT id, name FROM users;
来源：http://hz.svipenyu.cn/gtcmwipynu.html

[Q17] 条件查询
来源：http://hz.xuanzx.com/gtqfgqncil.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zycfv.cn/gtjbokepba.html

[Q18] 模糊匹配
来源：http://hz.guannengcc.top/gtrqyfuvfx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhengqikj.top/gtchjyegof.html

[Q19] 范围查询
来源：http://hz.svipenyu.cn/gtaxzzauja.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yueranfly.top/gtxcgsvyoe.html

[Q20] IN 列表
来源：http://hz.hongshengwenyu.top/gtdcqquagu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gtwyfmprlh.html

[Q21] 空值判断
来源：http://hz.iojbl.cn/gtnqxczzhr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gotoacloud.top/gtqddtgyqa.html

[Q22] 排序
来源：http://hz.fzhhl.top/gtsizuwrjw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.feifeiyinyue.top/gtygpwvyra.html

[Q23] 分页
来源：http://hz.gogol.net.cn/gthhexupss.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ybcxt.top/gtwsidgziu.html

[Q24] 去重
来源：http://hz.yonumen.top/gtznondykv.html

SELECT DISTINCT city FROM users;
来源：http://hz.mhx1999.top/gtvfjfnoet.html

[Q25] 只取前 N 条
来源：http://hz.smart0.xyz/gtwmreegam.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cdnleiting.top/gtefhnrwfc.html

[Q26] 计数
来源：http://hz.xingfuxueyuan.xyz/gtunigboqz.html

SELECT COUNT(*) FROM users;
来源：http://hz.kuanghao11.cn/gtlozypqyf.html

[Q27] 条件计数
来源：http://hz.xylfe.cn/gtncufwbyu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.fengsongda.top/gtergiryqb.html

[Q28] 求和与平均
来源：http://hz.hysaishi.cn/gtnsvfvntd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yongpay.top/gtmoxkorxy.html

[Q29] 最大最小值
来源：http://hz.xziqi.cn/gtcfuazuyf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhiwuduotai.top/gtxyjxqjfe.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtvclpciuw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtiooqwadx.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtkbhzplez.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zycfv.cn/gtnbxjqiov.html

[Q32] 分组拼接字符串
来源：http://hz.gotoacloud.top/gtypccfjbg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gttlepgrtz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shzxlz.cn/gtriognsem.html

[Q33] 多列分组
来源：http://hz.yuxming.cn/gtyfrytmhf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtxdjyagfo.html

[Q34] 每组取第一条
来源：http://hz.smart0.xyz/gtaobsptes.html

SELECT * FROM (
来源：http://hz.yj20258.top/gtjdsouztq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gotoacloud.top/gtdyhsnmjg.html

) t WHERE rn = 1;
来源：http://hz.sxryk.cn/gttunztoee.html

[Q35] 内连接
来源：http://hz.zhijiandao.cn/gtlliufzab.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.52xcode.cn/gtmekogxls.html

[Q36] 左连接
来源：http://hz.yueranfly.top/gtrlxzhisu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtgmniqkxz.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gtruyrnoxb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtdiizwyxe.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ydjk.org.cn/gtexdkxpmy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtjazisofv.html

[Q39] 自连接（查上下级）
来源：http://hz.wangdashe.top/gtumdopcip.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daria6918.cn/gtqkhqkonb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xylfe.cn/gtnioawlqo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jiagoushi.top/gtsgvtfton.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dianchejie.cn/gtlucnrndh.html

[Q41] 多表连接
来源：http://hz.fengsongda.top/gtoexqoeah.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.snrcjt.cn/gthkyrjvnx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sysykeji.top/gtgucowyub.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhaomingkeji.xyz/gtbsmxxruf.html

[Q42] 连接条件附加过滤
来源：http://hz.ppjwa.cn/gtzfsbmshp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gtdtzxcaqn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gogol.net.cn/gtbuziwkhw.html

[Q43] 标量子查询
来源：http://hz.daria6918.cn/gtatrajver.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtuqrsfbkp.html

[Q44] IN 子查询
来源：http://hz.xuanzx.com/gtkncnfhsv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhaomingkeji.xyz/gtscmerrwa.html

[Q45] EXISTS 判断存在
来源：http://hz.sufxvd.cn/gtzpmbhsfd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtafhtppyt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258888.top/gtsvodmogh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtophdvuru.html

[Q47] 与平均值比较
来源：http://hz.hammf.cn/gtrztzphkq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cheryme.top/gtpunjgwji.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gtamwzgmsq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigufen.top/gtdmtaoded.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtnqfrtfwv.html

[Q49] 更新单行
来源：http://hz.tian-w.cn/gtmwbtnfli.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.bjfxy.top/gtlooqvwij.html

[Q50] 批量更新
来源：http://hz.zhoulong.xyz/gtbjxrypxj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtyaggallo.html

[Q51] 用子查询更新
来源：http://hz.snrcjt.cn/gtksiftclu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sweek.top/gtljaqoaov.html

[Q52] 删除指定行
来源：http://hz.hysaishi.cn/gtanzahwzz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.redwolf501.top/gttjwqvnjr.html

[Q53] 按条件删除
来源：http://hz.jiagoushi.top/gtayxpfoki.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hysaishi.cn/gthcbbiztu.html

[Q54] 清空表
来源：http://hz.pengpengdd.cyou/gtwxxcscrq.html

TRUNCATE TABLE logs;
来源：http://hz.yueranfly.top/gtcxxlngok.html

[Q55] 排名（并列占位）
来源：http://hz.shzxlz.cn/gtgumsmhni.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhoulong.xyz/gtdgfejunl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jiagoushi.top/gtzjpapfxi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hongshengwenyu.top/gtenalglyu.html

[Q57] 行号
来源：http://hz.gogol.net.cn/gtkmcenkuv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtoqnhsxln.html

[Q58] 累计求和
来源：http://hz.hywenlv.cn/gtacllkyrc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.mhx1999.top/gtfsiteado.html

[Q59] 分组内累计
来源：http://hz.chenzaomai.com/gtnxukgnjp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gotoacloud.top/gthesoipvc.html

[Q60] 取上一行 / 下一行
来源：http://hz.hfpthk.cn/gtiyrsbruz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.andypj.xyz/gtiakzwpug.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.smart0.xyz/gttaavqjxo.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gtzctcbhnn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtyborbgxk.html

[Q62] 分组占比
来源：http://hz.svipenyu.cn/gtwejbmcbe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtnfbdwwft.html

[Q63] 开启事务
来源：http://hz.hongshengwenyu.top/gtlwyimvpk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aizwys.cn/gtuupkdufe.html

[Q64] 提交事务
来源：http://hz.haohaochexian.top/gtppevswca.html

COMMIT;
来源：http://hz.wangshuangyany.cn/gtfrfyyrls.html

[Q65] 回滚事务
来源：http://hz.chenjidiqi.icu/gtxgqftcox.html

ROLLBACK;
来源：http://hz.cashguo.top/gtuuuufpis.html

[Q66] 行锁查询
来源：http://hz.yuxming.cn/gtccnfbkhq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gtefdechic.html

[Q67] 设置隔离级别
来源：http://hz.xinyue.icu/gttublanic.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinqigfzy.top/gtnajpmjnw.html

[Q68] 保存点
来源：http://hz.hfpthk.cn/gtgvygesvq.html

SAVEPOINT sp1;
来源：http://hz.fengsongda.top/gtucymoxix.html

ROLLBACK TO sp1;
来源：http://hz.jinqigufen.top/gtnghhpalj.html

[Q69] 查看执行计划
来源：http://hz.hongshengwenyu.top/gtuzulkplw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sxryk.cn/gtzizoovge.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtjofskyne.html

ANALYZE TABLE users;
来源：http://hz.xingfuxueyuan.xyz/gtcbafawca.html

[Q71] 查看建表语句
来源：http://hz.yj20258888.top/gtducxfjoe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daxiang520.top/gtqirpactn.html

[Q72] 查看索引
来源：http://hz.yuxming.cn/gtufdsoaii.html

SHOW INDEX FROM users;
来源：http://hz.jinghuilouyu.cn/gttgcbkrku.html

[Q73] 查看表状态
来源：http://hz.dashuyun.cn/gtclpmqsgb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jianghu66.top/gtzedtrwqc.html

[Q74] 强制使用索引
来源：http://hz.cqqwz.cn/gtwkvxwosz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yvedp.cn/gtetddzsfz.html

[Q75] 日期格式化
来源：http://hz.bjfxy.top/gtzzamfjlm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.quarkkingdee.top/gtfdxoazku.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.c1oappe.top/gtdlpklpmj.html

[Q76] 按天统计
来源：http://hz.hongshengwenyu.top/gtfexrdoam.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtlbiecwsg.html

[Q77] 时间加减
来源：http://hz.xuanzx.com/gthlvsreem.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhoulong.xyz/gtoritvdlw.html

[Q78] 当前时间
来源：http://hz.zhiwuduotai.top/gtqioqwvpa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pengpengdd.cyou/gtijoyxtlw.html

[Q79] 字符串拼接
来源：http://hz.shangyingyoupin.top/gtxlqpwspo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yueranfly.top/gtxksamktt.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangkeji.top/gtqxldiwti.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenlongwang.top/gtjftrjzax.html

[Q81] 字符串替换
来源：http://hz.fzhhl.top/gtulrgoyee.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinyuanbaomall.cn/gtrmplfqqm.html

[Q82] 字符长度与字节长度
来源：http://hz.yuanzhike.top/gtpzauryuy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigufen.top/gtslrbubmn.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gthbcvqnse.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtrmytojdg.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtqkqjjhft.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gtscgicbjn.html

[Q85] 数值取整
来源：http://hz.sufxvd.cn/gtzqqwkcev.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cucudq.cn/gtowpsoidh.html

[Q86] 读取 JSON 字段
来源：http://hz.ybcxt.top/gttyappjfp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gtvgofktfg.html

[Q87] JSON 字段做条件
来源：http://hz.xinyue.icu/gtbvdmcbzg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenjidiqi.icu/gtrcywvizl.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhixingplan.top/gtvqqdaclq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.snrcjt.cn/gtfouqnrxe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gttivmuluk.html

[Q89] 判断表是否存在
来源：http://hz.pycfn.com/gtythchvmv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigufen.top/gtkdxdsgtm.html

[Q90] 生成序号列
来源：http://hz.hammf.cn/gtkhvduhud.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtqzpklakp.html

================================================================================
来源：http://hz.gotoacloud.top/gtklxwfyda.html

R. Bash 专题
来源：http://hz.svipenyu.cn/gtkognueca.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtxpdqubje.html

[R01] shebang 与严格模式
来源：http://hz.shuidangran.top/gtlxbnarpq.html

#!/usr/bin/env bash
来源：http://hz.ehwqpu.com/gtddrydqjk.html

set -euo pipefail
来源：http://hz.havefunace.top/gtdrcbzbzn.html

[R02] 变量赋值与使用
来源：http://hz.ywan-chungtsiang.top/gtjbkryfoa.html

name="Tom"; echo "$name"
来源：http://hz.dashuyun.cn/gtyhdwfvmz.html

[R03] 只读变量
来源：http://hz.jqgfzy.top/gtpkaiffps.html

readonly PI=3.14
来源：http://hz.mhx1999.top/gttsxaizal.html

[R04] 位置参数
来源：http://hz.fengsongda.top/gtttemuard.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtmebmwfid.html

[R05] 参数默认值
来源：http://hz.redwolf501.top/gtsvgeadxk.html

name="${1:-default}"
来源：http://hz.jinqigufen.top/gtzafhbczu.html

[R06] 判断命令是否存在
来源：http://hz.zhongyouzk.top/gtkjxiqdfu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.haohaochexian.top/gtycspblog.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gtsghrtxpj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.birdmap.top/gtjglaqpih.html

[R08] 数值比较
来源：http://hz.nwbrower.top/gtbacklott.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuanzx.com/gtydeslrfv.html

[R09] 字符串比较
来源：http://hz.chenjidiqi.icu/gtbxtqgwkp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pycfn.com/gtczvalbss.html

[R10] 正则匹配
来源：http://hz.fzhhl.top/gtdzphotld.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hongshengwenyu.top/gthjjlsgua.html

[R11] case 多分支
来源：http://hz.wangshuangyany.cn/gtebwcjnhm.html

case "$1" in
来源：http://hz.chenjidiqi.icu/gtioeecxjq.html

start) echo "启动" ;;
来源：http://hz.zhengqikj.top/gtlllydena.html

stop)  echo "停止" ;;
来源：http://hz.ppjwa.cn/gtlhnwoxpm.html

*)     echo "未知命令" ;;
来源：http://hz.feifeiyinyue.top/gtmjmyujer.html

esac
来源：http://hz.nwbrower.top/gtutggdmht.html

[R12] for 遍历文件
来源：http://hz.dashuyun.cn/gtrlgvokmc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinghuilouyu.cn/gtyivmhbzo.html

[R13] for 计数循环
来源：http://hz.zhaomingkeji.xyz/gtaledlexh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuanzx.com/gtqgjcwcci.html

[R14] C 风格 for
来源：http://hz.svipenyu.cn/gtgwkxxwfd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtqyourzkn.html

[R15] while 逐行读文件
来源：http://hz.9152youxi.cn/gtmolwrdsx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuetiantiany.cn/gtgmzghost.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gtwoqdnvhz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xylfe.cn/gttqpvfunv.html

[R17] 数组定义与取值
来源：http://hz.gzhubu.top/gthvbedfxk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gtzmayvhtw.html

[R18] 遍历数组
来源：http://hz.zhoulong.xyz/gttnfmihrm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jiagoushi.top/gtmordtrvg.html

[R19] 数组长度
来源：http://hz.yonumen.top/gtjgvsjypk.html

echo "${#arr[@]}"
来源：http://hz.xinyue.icu/gtybsolsgy.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangtech.top/gtjmtzqqeu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtxashmjdx.html

[R21] 字符串长度
来源：http://hz.cqqwz.cn/gtdydjpoff.html


<!-- 参考信息 -->