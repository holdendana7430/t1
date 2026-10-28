代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.vqdsnc.cn/gtcwhmabkg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtihywpjiz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258888.top/gtkxrffcym.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhongyouzk.top/gtrzkzjhwt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dashuyun.cn/gtvgtobsbp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yongpay.top/gtycumfjdj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigfzy.top/gtzilsfnyt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenzaomai.com/gtfzdckgap.html

================================================================================
来源：http://hz.yonumen.top/gtvtubhjpq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuanzhike.top/gtisnoenul.html

================================================================================
来源：http://hz.ivvv.top/gtikxceduq.html

[Q01] 创建表
来源：http://hz.ivvv.top/gtzhdroifx.html

CREATE TABLE users (
来源：http://hz.zhixingplan.top/gtiuqmuibs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtglaxtbek.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yongpay.top/gtdwjfzmow.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuanzx.com/gtbeiijtye.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangtech.top/gtkwftdfnb.html

);
来源：http://hz.ydjk.org.cn/gtnwagdlnx.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangtech.top/gtsexagkcw.html

CREATE TABLE orders (
来源：http://hz.jinyuanbaomall.cn/gtuusuujnr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtjwpinjig.html

user_id INT NOT NULL,
来源：http://hz.shuidangran.top/gtkcduzokw.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigufen.top/gtgrbbdbse.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dashuyun.cn/gtfvplcvyw.html

);
来源：http://hz.cashguo.top/gtofizdcbe.html

[Q03] 增加列
来源：http://hz.52xcode.cn/gtmsrpwkcl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hfpthk.cn/gtpdtiasia.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtftxhkzha.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.havefunace.top/gtxqjljteh.html

[Q05] 重命名列
来源：http://hz.shangyingyoupin.top/gtnhmwshsd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydzc1.top/gtqppzcimu.html

[Q06] 删除列
来源：http://hz.nanxinkj.top/gtuvwhqmje.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhaomingkeji.xyz/gtalmcixif.html

[Q07] 删除表
来源：http://hz.shuidangran.top/gtopombnzi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hywenlv.cn/gtbkskjghh.html

[Q08] 创建普通索引
来源：http://hz.snrcjt.cn/gtbuodywps.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.pycfn.com/gtrsfhikut.html

[Q09] 创建唯一索引
来源：http://hz.zhixingplan.top/gtairemksu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gttaxbxmjl.html

[Q10] 插入单行
来源：http://hz.yongpay.top/gtmhbelgwh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sysykeji.top/gtdzzkznvd.html

[Q11] 一次插入多行
来源：http://hz.cashguo.top/gtkzkkypxy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dianchejie.cn/gtczetsqwa.html

[Q12] 插入后取自增 ID
来源：http://hz.ydjk.org.cn/gtbiarirbn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhiwuduotai.top/gtclbrpksf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yongpay.top/gtkzekiuqn.html

[Q13] 忽略重复插入
来源：http://hz.zhongyouzk.top/gtjxghknfj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinyuanbaomall.cn/gtcvqqfiia.html

[Q14] 存在则更新（upsert）
来源：http://hz.ivvv.top/gtirqxxsqw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ywan-chungtsiang.top/gtvyfyhhwg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.316326.xyz/gtljmootdj.html

[Q15] 查询全部
来源：http://hz.yj20258888.top/gtfngiuilm.html

SELECT * FROM users;
来源：http://hz.kuanghao11.cn/gtviysnyue.html

[Q16] 查询指定列
来源：http://hz.shangyingyoupin.top/gtpcnbcnfn.html

SELECT id, name FROM users;
来源：http://hz.chenlongwang.top/gtqasqccjg.html

[Q17] 条件查询
来源：http://hz.xinyue.icu/gtjssgyuzs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xinyue.icu/gtetqmtnqj.html

[Q18] 模糊匹配
来源：http://hz.cdnleiting.top/gthyakmlum.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gzhubu.top/gtyqeukcjv.html

[Q19] 范围查询
来源：http://hz.zhijiandao.cn/gtqieuexkj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yanxiufei.cn/gtdueurirh.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtmeaosxup.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gttwegzkpc.html

[Q21] 空值判断
来源：http://hz.wangdashe.top/gtmzzrscql.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jianghu66.top/gtdljewrer.html

[Q22] 排序
来源：http://hz.chenjidiqi.icu/gtthoqsvqx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guannengcc.top/gtburbxaob.html

[Q23] 分页
来源：http://hz.yanxiufei.cn/gtdujxqbdm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgfzy.top/gtyoumcbfj.html

[Q24] 去重
来源：http://hz.sysykeji.top/gtyicenxhi.html

SELECT DISTINCT city FROM users;
来源：http://hz.shangyingyoupin.top/gthdsjkynz.html

[Q25] 只取前 N 条
来源：http://hz.fengsongda.top/gtpleuialh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tianlin.xyz/gtclydnhgg.html

[Q26] 计数
来源：http://hz.yuanzhike.top/gtoujijmrm.html

SELECT COUNT(*) FROM users;
来源：http://hz.havefunace.top/gtqjhketwt.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gttpxzlpyw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtddcuurgw.html

[Q28] 求和与平均
来源：http://hz.dianchejie.cn/gtaxsadtab.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhoulong.xyz/gtcvprygao.html

[Q29] 最大最小值
来源：http://hz.ybcxt.top/gtetoiyugc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cucudq.cn/gtwabcyobe.html

[Q30] 分组统计
来源：http://hz.cqqwz.cn/gtpkxbxcrb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtfclwyoxe.html

[Q31] 分组后过滤
来源：http://hz.0kj1m.cn/gtpgiercao.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gaohongyu789.top/gtqapbbsal.html

[Q32] 分组拼接字符串
来源：http://hz.gaohongyu789.top/gttxnxmfii.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtmlohkgnd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yonumen.top/gtchxkvfvq.html

[Q33] 多列分组
来源：http://hz.yj20258888.top/gtsjdgjzee.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtxstsfzmz.html

[Q34] 每组取第一条
来源：http://hz.jinqigufen.top/gttsojuzgv.html

SELECT * FROM (
来源：http://hz.ybcxt.top/gtoehchdpd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fengsongda.top/gtmdoiudrd.html

) t WHERE rn = 1;
来源：http://hz.redwolf501.top/gtkkwdharn.html

[Q35] 内连接
来源：http://hz.hnxiangtu.top/gtisyifljz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtxwtrowvx.html

[Q36] 左连接
来源：http://hz.zhiwuduotai.top/gtutxywfmw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hfpthk.cn/gtyzjbeyfm.html

[Q37] 右连接
来源：http://hz.shuidangran.top/gtzuycqznq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuetiantiany.cn/gtwiryaojm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhongyouzk.top/gtzyrjhpea.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgufenzy.top/gtzmljjjib.html

[Q39] 自连接（查上下级）
来源：http://hz.iojbl.cn/gtxsqloobw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtdbcxmzpq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgfzy.top/gtlwkgblzd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zycfv.cn/gtxxlrhtyo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.iojbl.cn/gtmgjcjoob.html

[Q41] 多表连接
来源：http://hz.ydjk.org.cn/gthsosxrkg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tanke756.top/gtoswuxhtj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zycfv.cn/gtbjnmtzed.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangkeji.top/gtodlbmvwq.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gtnofrwibn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sysykeji.top/gtxxsqexdy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.redwolf501.top/gtgyorjcyd.html

[Q43] 标量子查询
来源：http://hz.hongshengwenyu.top/gtdmtocsbj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gtwgcpnlqs.html

[Q44] IN 子查询
来源：http://hz.jlsjyb.cn/gtukpfxwyj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jlsjyb.cn/gtxvvcowit.html

[Q45] EXISTS 判断存在
来源：http://hz.yuxming.cn/gtqiheizat.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtsenvtmek.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtndmlngum.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gtyyhjeriv.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gtwdnbzupm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangdashe.top/gtanvlakgx.html

[Q48] CTE 公用表表达式
来源：http://hz.yvedp.cn/gtnwpvqvzo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shuidangran.top/gtytslmifg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hysaishi.cn/gtyrzdtugi.html

[Q49] 更新单行
来源：http://hz.birdmap.top/gtiaenkvzb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fengsongda.top/gtygxukjab.html

[Q50] 批量更新
来源：http://hz.daxiang520.top/gtawfiymjf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ivvv.top/gtacyczljf.html

[Q51] 用子查询更新
来源：http://hz.xuanzx.com/gtiuyvwese.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aizwys.cn/gtxkiqxqzr.html

[Q52] 删除指定行
来源：http://hz.yonumen.top/gtgybvjume.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jyoumei.cn/gtgroyaxqr.html

[Q53] 按条件删除
来源：http://hz.pengpengdd.cyou/gtvdfojvzq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ybcxt.top/gtnqffseor.html

[Q54] 清空表
来源：http://hz.ivvv.top/gtedgipggl.html

TRUNCATE TABLE logs;
来源：http://hz.tanke756.top/gtwliylzsn.html

[Q55] 排名（并列占位）
来源：http://hz.yvedp.cn/gtiyxnntvf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guowangkeji.top/gtmqegkdzc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtflkztovr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hongshengwenyu.top/gthvmigeft.html

[Q57] 行号
来源：http://hz.ydzc1.top/gtvuirxcwp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yueranfly.top/gtztwnhugn.html

[Q58] 累计求和
来源：http://hz.yonumen.top/gtyltntast.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.redwolf501.top/gtcvpqtosp.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtlrthejnj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtqjspmjjk.html

[Q60] 取上一行 / 下一行
来源：http://hz.c1oappe.top/gtftwohzpa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gotoacloud.top/gtphionxyf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.bjfxy.top/gtbtvkxgjn.html

[Q61] 移动平均
来源：http://hz.gotoacloud.top/gtgbtvhice.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yonumen.top/gtotkoqwcc.html

[Q62] 分组占比
来源：http://hz.nwbrower.top/gtxuvbddtm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtyyidkdcf.html

[Q63] 开启事务
来源：http://hz.yuxming.cn/gthubuieou.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.haohaochexian.top/gtngpaabzv.html

[Q64] 提交事务
来源：http://hz.316326.xyz/gtqtirawhd.html

COMMIT;
来源：http://hz.snrcjt.cn/gtzkriybmc.html

[Q65] 回滚事务
来源：http://hz.wangshuangyany.cn/gtiptgzyxa.html

ROLLBACK;
来源：http://hz.iojbl.cn/gtlxgjhzcp.html

[Q66] 行锁查询
来源：http://hz.ydjk.org.cn/gtnaotuepo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.dashuyun.cn/gtjcgjqwhv.html

[Q67] 设置隔离级别
来源：http://hz.jiagoushi.top/gtghezphlw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cucudq.cn/gtbnwxrwdp.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gttbnraoxm.html

SAVEPOINT sp1;
来源：http://hz.zhongyouzk.top/gttiylieee.html

ROLLBACK TO sp1;
来源：http://hz.shzxlz.cn/gtdhdofrkq.html

[Q69] 查看执行计划
来源：http://hz.yvedp.cn/gtulozxhqw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xylfe.cn/gtsxqxuwfp.html

[Q70] 更新统计信息
来源：http://hz.c1oappe.top/gthgxwltek.html

ANALYZE TABLE users;
来源：http://hz.bjfxy.top/gtlzaqcvvi.html

[Q71] 查看建表语句
来源：http://hz.pengpengdd.cyou/gtvpkknkuj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shanyushiyangkeji.top/gtcgarkpyc.html

[Q72] 查看索引
来源：http://hz.xuetiantiany.cn/gtadxbzxod.html

SHOW INDEX FROM users;
来源：http://hz.havefunace.top/gthkzzwddx.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gtezojyxhd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nwbrower.top/gtxphelvft.html

[Q74] 强制使用索引
来源：http://hz.snrcjt.cn/gtbpjqvvxd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhijiandao.cn/gtxvijcgyb.html

[Q75] 日期格式化
来源：http://hz.zycfv.cn/gtnlwxtbqm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtgoqbvnui.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cashguo.top/gtgimdchuz.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtrakyhubd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.havefunace.top/gtywesgtso.html

[Q77] 时间加减
来源：http://hz.jiagoushi.top/gtaldihntx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yueranfly.top/gtoerojptz.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtrqjvsqes.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.52xcode.cn/gtwkrnawqf.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtlrprcjuq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fengsongda.top/gthmyyykdu.html

[Q80] 字符串截取
来源：http://hz.aibaodan.cn/gtldkegddx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gogol.net.cn/gtgxawtnsd.html

[Q81] 字符串替换
来源：http://hz.zhoulong.xyz/gtyvgocbkx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangkeji.top/gtkxduxntc.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gthxhcnhun.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtuqdajmrb.html

[Q83] 大小写转换
来源：http://hz.snrcjt.cn/gteswionfz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yonumen.top/gtehltyesa.html

[Q84] 去除首尾空格
来源：http://hz.nanxinkj.top/gtvqaejiio.html

SELECT TRIM(name) FROM users;
来源：http://hz.nanxinkj.top/gtqhfsryoy.html

[Q85] 数值取整
来源：http://hz.zhoulong.xyz/gtkgguadie.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zdqjudy.top/gtdtqanxai.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtvyqzmfon.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj202588.top/gtdwhyanuw.html

[Q87] JSON 字段做条件
来源：http://hz.sufxvd.cn/gtucxagnjw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daria6918.cn/gtcdaefdff.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtyryormll.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.haohaochexian.top/gtpkuhzifm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.bjfxy.top/gttycmtdcx.html

[Q89] 判断表是否存在
来源：http://hz.ybcxt.top/gtahpgryfx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinghuilouyu.cn/gtyruelboh.html

[Q90] 生成序号列
来源：http://hz.52xcode.cn/gtpkagmnbm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tanke756.top/gtlkdnkrbf.html

================================================================================
来源：http://hz.hysaishi.cn/gthkizgdwg.html

R. Bash 专题
来源：http://hz.andypj.xyz/gtceoucrcj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxzezotrp.html

[R01] shebang 与严格模式
来源：http://hz.sysykeji.top/gtcncolnqg.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtxclruwxs.html

set -euo pipefail
来源：http://hz.ywan-chungtsiang.top/gtyqxobwsu.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gtnoftrtgy.html

name="Tom"; echo "$name"
来源：http://hz.zhiwuduotai.top/gthwzdprxx.html

[R03] 只读变量
来源：http://hz.kuanghao11.cn/gtlhhkecrz.html

readonly PI=3.14
来源：http://hz.pycfn.com/gttsrxxnif.html

[R04] 位置参数
来源：http://hz.cashguo.top/gtbmjtrvjx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tian-w.cn/gtwjwbxafw.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtjmbeotko.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtklrskjdn.html

[R06] 判断命令是否存在
来源：http://hz.cheryme.top/gtatjbczdz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.havefunace.top/gtqqnigrcn.html

[R07] if 判断文件
来源：http://hz.yvedp.cn/gtpnpxidyg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.pengpengdd.cyou/gtusspjngj.html

[R08] 数值比较
来源：http://hz.wangdashe.top/gtppjiggct.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhengqikj.top/gtginnrykb.html

[R09] 字符串比较
来源：http://hz.shuidangran.top/gtylnwqpdy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yanxiufei.cn/gtpksklglo.html

[R10] 正则匹配
来源：http://hz.sxryk.cn/gtwtzfeznp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtmrojazlw.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtzgssqbyl.html

case "$1" in
来源：http://hz.hongshengwenyu.top/gtmwuxapyg.html

start) echo "启动" ;;
来源：http://hz.wangdashe.top/gtsebqeczi.html

stop)  echo "停止" ;;
来源：http://hz.smart0.xyz/gtinjriivj.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtdzbdrkbl.html

esac
来源：http://hz.chenlongwang.top/gtmttyvyfl.html

[R12] for 遍历文件
来源：http://hz.chenzaomai.com/gtbmpqvqkz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgufenzy.top/gtjivjwgzw.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtzkjtgman.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shuidangran.top/gtoqeugqoc.html

[R14] C 风格 for
来源：http://hz.jinqigufen.top/gtcjueqnhg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.meibo888.top/gtpuogqsro.html

[R15] while 逐行读文件
来源：http://hz.jianghu66.top/gtpfhtanul.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhoulong.xyz/gtasmoklil.html

[R16] until 等待条件
来源：http://hz.yueranfly.top/gtgmxgfqpz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtohapenav.html

[R17] 数组定义与取值
来源：http://hz.hywenlv.cn/gtzsdnrqqq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangshuangyany.cn/gtzvzivuts.html

[R18] 遍历数组
来源：http://hz.wangshuangyany.cn/gtfsacxlqs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj202588.top/gtaqzjgdsi.html

[R19] 数组长度
来源：http://hz.yj202588.top/gthtpcrodn.html

echo "${#arr[@]}"
来源：http://hz.yj20258888.top/gtbddzcgds.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangtech.top/gtpzoqjpcj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shuidangran.top/gtboqcjjir.html

[R21] 字符串长度
来源：http://hz.xziqi.cn/gtdvyzbtlc.html

echo "${#s}"
来源：http://hz.yuxming.cn/gtflhdjche.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtajsdziwr.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gtqyesxskv.html

[R23] 字符串替换
来源：http://hz.sufxvd.cn/gtzxvhkewo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.haohaochexian.top/gtinsatakk.html

[R24] 大小写转换
来源：http://hz.shangyingyoupin.top/gthyfmftyv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.kuanghao11.cn/gtepxtoear.html

[R25] 去后缀 / 去前缀
来源：http://hz.gotoacloud.top/gtfdnsmmaq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnxiangtu.top/gttpmcnttg.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gtsnbrvltn.html

now=$(date +%F); echo "$now"
来源：http://hz.yangfankeji.com/gtpgyinapy.html

[R27] 算术展开
来源：http://hz.cqqwz.cn/gtvrqnykmh.html

echo $((1 + 2 * 3))
来源：http://hz.gotoacloud.top/gtecbbekis.html

[R28] 浮点运算
来源：http://hz.sweek.top/gtyxvgeqwa.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenlongwang.top/gtwmjrxanm.html

[R29] 定义函数
来源：http://hz.yonumen.top/gtawjprfag.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ybcxt.top/gtqilgyqpz.html

[R30] 函数返回状态码
来源：http://hz.meibo888.top/gtywbpznnt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sweek.top/gtpuusrern.html

[R31] 局部变量
来源：http://hz.zdqjudy.top/gtockbsgis.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangtech.top/gtmofgllsg.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtdaleaxck.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258888.top/gtyvuzalhh.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigfzy.top/gtdymkfjya.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgufenzy.top/gtgtgqmpxt.html

[R34] 退出时清理
来源：http://hz.fengsongda.top/gtbvxyqvvi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtodeolifz.html

[R35] 后台执行并等待
来源：http://hz.ehwqpu.com/gtfrvfwutu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtihtcewci.html

[R36] 并发执行多个任务
来源：http://hz.c1oappe.top/gtwqzneuiy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tian-w.cn/gtlbuddphp.html

[R37] 把输出赋给变量
来源：http://hz.jinqigfzy.top/gtemxzkeoc.html

files=$(ls -1)
来源：http://hz.hnqzz.top/gtdtpbkoxo.html

[R38] 管道串联
来源：http://hz.jinqigufen.top/gtykjdmjuu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yueranfly.top/gtldlopnkl.html

[R39] 重定向标准输出与错误
来源：http://hz.pycfn.com/gtrkwmwsmx.html


<!-- 参考信息 -->