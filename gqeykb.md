代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.bjfxy.top/gtvemraefy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.andypj.xyz/gtbuwhjumd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhongyouzk.top/gtzmcgafaa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtppcosigu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtqpnwkdoq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daxiang520.top/gtkvlnztfj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zycfv.cn/gtvmxmdjys.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangtech.top/gtylmsrxjb.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtqqofxivl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cqqwz.cn/gtwaflckzs.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnwqzanmn.html

[Q01] 创建表
来源：http://hz.yvedp.cn/gtwingpxlb.html

CREATE TABLE users (
来源：http://hz.jianghu66.top/gttztprnpg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtxfmdmrnh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtowktbebl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yangfankeji.com/gtqxraphyd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daxiang520.top/gtmdmeyblj.html

);
来源：http://hz.yonumen.top/gtqlufzgnd.html

[Q02] 创建带外键的表
来源：http://hz.cucudq.cn/gtosdxwkrj.html

CREATE TABLE orders (
来源：http://hz.0kj1m.cn/gtkbichxne.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtcjtcprsu.html

user_id INT NOT NULL,
来源：http://hz.jqgfzy.top/gtrscklwlz.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtiszldqpr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jqgfzy.top/gtimkuoikg.html

);
来源：http://hz.xinyue.icu/gtjatkmfvp.html

[Q03] 增加列
来源：http://hz.chenlongwang.top/gttdwjyiwm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ywan-chungtsiang.top/gtllmmwyfo.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtfmwsxhjt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.bjfxy.top/gthupltgnk.html

[Q05] 重命名列
来源：http://hz.kuanghao11.cn/gtkhxrtvsw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgufenzy.top/gtxrrgupup.html

[Q06] 删除列
来源：http://hz.ydjk.org.cn/gtirlrrlks.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtcjqmnqhb.html

[Q07] 删除表
来源：http://hz.tianlin.xyz/gtyngirflf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nanxuanxn.top/gtfxtqqrjp.html

[Q08] 创建普通索引
来源：http://hz.zhaomingkeji.xyz/gtciadavvr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jianghu66.top/gtrpgsqbuq.html

[Q09] 创建唯一索引
来源：http://hz.svipenyu.cn/gtbsskmqyg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtdwmueljw.html

[Q10] 插入单行
来源：http://hz.wangdashe.top/gthfgdwefl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.feifeiyinyue.top/gtqfgtmita.html

[Q11] 一次插入多行
来源：http://hz.yj20258.top/gtacekxrks.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xinyue.icu/gtkemoqatv.html

[Q12] 插入后取自增 ID
来源：http://hz.andypj.xyz/gtferxhscm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.iojbl.cn/gtvkbpstkx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sufxvd.cn/gtchjcxnts.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtzaqxzhwh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgufenzy.top/gtufzgkrot.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtdtrtjyjw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pengpengdd.cyou/gtbdxiilhf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hfpthk.cn/gtawmrzvtu.html

[Q15] 查询全部
来源：http://hz.dashuyun.cn/gtsnkwftls.html

SELECT * FROM users;
来源：http://hz.sweek.top/gtalxpymhp.html

[Q16] 查询指定列
来源：http://hz.yonumen.top/gtyjsuvcjl.html

SELECT id, name FROM users;
来源：http://hz.ehwqpu.com/gtliuqsmxj.html

[Q17] 条件查询
来源：http://hz.hywenlv.cn/gtosflgpks.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cashguo.top/gtzujorxwt.html

[Q18] 模糊匹配
来源：http://hz.xinyue.icu/gtolulwxbt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hysaishi.cn/gtfaofndad.html

[Q19] 范围查询
来源：http://hz.smart0.xyz/gtpbnqgixt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.fzhhl.top/gtzqwyavzk.html

[Q20] IN 列表
来源：http://hz.9152youxi.cn/gtpvgfgkhf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.snrcjt.cn/gtrecumkvy.html

[Q21] 空值判断
来源：http://hz.zhoulong.xyz/gtqpwqdpmw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.andypj.xyz/gttsfiihpe.html

[Q22] 排序
来源：http://hz.hnxiangtu.top/gtfnhjblqy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtojtiohbq.html

[Q23] 分页
来源：http://hz.c1oappe.top/gtqargrtqf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tianlin.xyz/gtzmqpobtw.html

[Q24] 去重
来源：http://hz.shanyushiyangtech.top/gtvljqvmkk.html

SELECT DISTINCT city FROM users;
来源：http://hz.sweek.top/gtfqzppfks.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gtzsdgeuti.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shuidangran.top/gtwcswowww.html

[Q26] 计数
来源：http://hz.xylfe.cn/gtqgofmanb.html

SELECT COUNT(*) FROM users;
来源：http://hz.cashguo.top/gtqnowiuzj.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gtiqufcxvo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuxming.cn/gtexrzrgmz.html

[Q28] 求和与平均
来源：http://hz.hfpthk.cn/gtdmehbgoo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hywenlv.cn/gtxcdwldxv.html

[Q29] 最大最小值
来源：http://hz.mhx1999.top/gtyeopsmai.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sxryk.cn/gtkbxafbfs.html

[Q30] 分组统计
来源：http://hz.pycfn.com/gtcdljqtua.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtcgajmaca.html

[Q31] 分组后过滤
来源：http://hz.cqqwz.cn/gtgnbulrzf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yangfankeji.com/gtddtmgsqk.html

[Q32] 分组拼接字符串
来源：http://hz.zhongyouzk.top/gtgfokcokc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtdeemwwmg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ehwqpu.com/gttouzhnck.html

[Q33] 多列分组
来源：http://hz.sweek.top/gtnzunbyvx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.kuanghao11.cn/gtljakhuqb.html

[Q34] 每组取第一条
来源：http://hz.zycfv.cn/gtfdvfcdya.html

SELECT * FROM (
来源：http://hz.yvedp.cn/gtmaepqvxe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydzc1.top/gtypkoocrs.html

) t WHERE rn = 1;
来源：http://hz.jqgufenzy.top/gtkxfavlyh.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gtczobucug.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtkprcyqph.html

[Q36] 左连接
来源：http://hz.ehwqpu.com/gtquzeoikm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigufen.top/gtvprvdgwj.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gtspdvspwr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.9152youxi.cn/gtbckmsdia.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtrsuxwmyd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yueranfly.top/gtfyenfgca.html

[Q39] 自连接（查上下级）
来源：http://hz.pengpengdd.cyou/gtgifalykh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gtfspvpqyj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtzzuvrzun.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gtxrllmmog.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtzyqvinik.html

[Q41] 多表连接
来源：http://hz.cashguo.top/gtkcspenpk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jiagoushi.top/gtkduoqklh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pycfn.com/gtfhuekbie.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhengqikj.top/gtjdcgoboz.html

[Q42] 连接条件附加过滤
来源：http://hz.hywenlv.cn/gtrkqalsem.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydzc1.top/gtnstkoywi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.svipenyu.cn/gtjnhzsuxz.html

[Q43] 标量子查询
来源：http://hz.yanxiufei.cn/gtstkmxllp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuetiantiany.cn/gtmebupblw.html

[Q44] IN 子查询
来源：http://hz.jinghuilouyu.cn/gtisvqdizx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtjybcqkkw.html

[Q45] EXISTS 判断存在
来源：http://hz.hnxiangtu.top/gtvkvvipfa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtncxxrefx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zycfv.cn/gtmljvopwc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtypwkwoxp.html

[Q47] 与平均值比较
来源：http://hz.pengpengdd.cyou/gtucdsinmc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhengqikj.top/gtxvwojken.html

[Q48] CTE 公用表表达式
来源：http://hz.kuanghao11.cn/gtfhgtmfhf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jyoumei.cn/gtawubrard.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yangfankeji.com/gtoskwzkdb.html

[Q49] 更新单行
来源：http://hz.guowangkeji.top/gtmbidiwua.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhixingplan.top/gtfnwsdlme.html

[Q50] 批量更新
来源：http://hz.xingfuxueyuan.xyz/gtnuearljz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.iojbl.cn/gtphuujfmy.html

[Q51] 用子查询更新
来源：http://hz.yueranfly.top/gtodqrzaoz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinyuanbaomall.cn/gtnkxkspsj.html

[Q52] 删除指定行
来源：http://hz.xylfe.cn/gtkhgdeltn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sysykeji.top/gtjkfleovy.html

[Q53] 按条件删除
来源：http://hz.dashuyun.cn/gtncyduovb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.vqdsnc.cn/gtrwdtlzcj.html

[Q54] 清空表
来源：http://hz.jinyuanbaomall.cn/gthpqfdkcg.html

TRUNCATE TABLE logs;
来源：http://hz.sxryk.cn/gtpilsonfu.html

[Q55] 排名（并列占位）
来源：http://hz.pengpengdd.cyou/gtgssjsjzg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ehwqpu.com/gtzmysbspy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hammf.cn/gtryogwyow.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yvedp.cn/gtqphsxpma.html

[Q57] 行号
来源：http://hz.vqdsnc.cn/gtkwwsyqqa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangtech.top/gtuqdqahmk.html

[Q58] 累计求和
来源：http://hz.zhixingplan.top/gthizvtluu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gtdxyrqesj.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtceicunsr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtxacilhtf.html

[Q60] 取上一行 / 下一行
来源：http://hz.cucudq.cn/gtqgnoflcq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hammf.cn/gtiajacmvy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cdnleiting.top/gttapppmhq.html

[Q61] 移动平均
来源：http://hz.zhongyouzk.top/gtbacaafua.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtdfyeadbi.html

[Q62] 分组占比
来源：http://hz.gotoacloud.top/gthqskbajj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtbndolssh.html

[Q63] 开启事务
来源：http://hz.tianlin.xyz/gtcljrcaii.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenzaomai.com/gtmbcaegjk.html

[Q64] 提交事务
来源：http://hz.tian-w.cn/gtjdxdzrvw.html

COMMIT;
来源：http://hz.hfpthk.cn/gttpwhzkbm.html

[Q65] 回滚事务
来源：http://hz.chenjidiqi.icu/gtxzjdjbyo.html

ROLLBACK;
来源：http://hz.wangshuangyany.cn/gtgaeiwlat.html

[Q66] 行锁查询
来源：http://hz.nanxinkj.top/gthjwaekmz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhongyouzk.top/gtbwtcrzje.html

[Q67] 设置隔离级别
来源：http://hz.hammf.cn/gtwhaggyik.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shuidangran.top/gtqufxmwzd.html

[Q68] 保存点
来源：http://hz.shanyushiyangkeji.top/gtbmayavtl.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtexwljexc.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtpfexksmm.html

[Q69] 查看执行计划
来源：http://hz.gzhubu.top/gtexlvddis.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.iojbl.cn/gtgnndlmec.html

[Q70] 更新统计信息
来源：http://hz.jiagoushi.top/gttdwvqtbr.html

ANALYZE TABLE users;
来源：http://hz.smart0.xyz/gtnhgxqfub.html

[Q71] 查看建表语句
来源：http://hz.xylfe.cn/gtizlrwxnc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guannengcc.top/gtercqxpvh.html

[Q72] 查看索引
来源：http://hz.316326.xyz/gtcfbglqbp.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtphrppjtq.html

[Q73] 查看表状态
来源：http://hz.aibaodan.cn/gtpeajzbzf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fzhhl.top/gtyfwvmmxd.html

[Q74] 强制使用索引
来源：http://hz.gogol.net.cn/gtvowkirek.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhijiandao.cn/gtuuwnhlwm.html

[Q75] 日期格式化
来源：http://hz.jinqigfzy.top/gtbzhpfjhu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtgljykqmt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangkeji.top/gtygbligob.html

[Q76] 按天统计
来源：http://hz.hongshengwenyu.top/gtpdkwrmbv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.aizwys.cn/gtgwxlahfm.html

[Q77] 时间加减
来源：http://hz.gotoacloud.top/gtjsvttvjo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinyuanbaomall.cn/gtfgzvkiqg.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gtoglgbbyv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pengpengdd.cyou/gtklglnjjz.html

[Q79] 字符串拼接
来源：http://hz.bjfxy.top/gtrcmjeinx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.kuanghao11.cn/gtalhyiddd.html

[Q80] 字符串截取
来源：http://hz.zhongyouzk.top/gtmqasxvgi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258.top/gtgoxpvzrd.html

[Q81] 字符串替换
来源：http://hz.chenzaomai.com/gtfadyrnav.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtdfqzwhrw.html

[Q82] 字符长度与字节长度
来源：http://hz.jlsjyb.cn/gtejajutzd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.iojbl.cn/gtuznxhxmg.html

[Q83] 大小写转换
来源：http://hz.hnqzz.top/gtscihjige.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhixingplan.top/gtsvcitnnn.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtkhimgxhj.html

SELECT TRIM(name) FROM users;
来源：http://hz.gzhubu.top/gthpyhvudq.html

[Q85] 数值取整
来源：http://hz.sufxvd.cn/gtknynmbsl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtpyczheec.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gthghbyxir.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhoulong.xyz/gtrqpwipai.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gtdhrjxmhr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dianchejie.cn/gtayhzvrzl.html

[Q88] 行转列（条件聚合）
来源：http://hz.ehwqpu.com/gtotghzpwy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtxmzzunfl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydzc1.top/gtiqmhqemy.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtgjoztuhf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtgjjjeipl.html

[Q90] 生成序号列
来源：http://hz.zhoulong.xyz/gtkkrfurad.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gtiapipgyp.html

================================================================================
来源：http://hz.gogol.net.cn/gtpbyjacrg.html

R. Bash 专题
来源：http://hz.ybcxt.top/gturwwsjap.html

================================================================================
来源：http://hz.cdnleiting.top/gtdvlytovi.html

[R01] shebang 与严格模式
来源：http://hz.hnqzz.top/gtgiwwjxlp.html

#!/usr/bin/env bash
来源：http://hz.cqqwz.cn/gtsudknzbz.html

set -euo pipefail
来源：http://hz.fzhhl.top/gtghihgcfr.html

[R02] 变量赋值与使用
来源：http://hz.9152youxi.cn/gtmwoyizwp.html

name="Tom"; echo "$name"
来源：http://hz.gotoacloud.top/gtrmsbosto.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtopazomwb.html

readonly PI=3.14
来源：http://hz.smart0.xyz/gtcrdxhcrq.html

[R04] 位置参数
来源：http://hz.svipenyu.cn/gtpgzxkgcj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtvcramqpu.html

[R05] 参数默认值
来源：http://hz.jiagoushi.top/gtuiaawxwk.html

name="${1:-default}"
来源：http://hz.zhongyouzk.top/gtkkeenoxx.html

[R06] 判断命令是否存在
来源：http://hz.zhijiandao.cn/gtkkzbzfgy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.kuanghao11.cn/gtobfmnyqj.html

[R07] if 判断文件
来源：http://hz.yuanzhike.top/gthxazyyqf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ivvv.top/gtubublpal.html

[R08] 数值比较
来源：http://hz.ywan-chungtsiang.top/gtlequspof.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhengqikj.top/gtmuhnlgyk.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtwxdafhig.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.guowangkeji.top/gtebnfhxtu.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gtwikuixms.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtyejlydmg.html

[R11] case 多分支
来源：http://hz.dashuyun.cn/gtbegahlld.html

case "$1" in
来源：http://hz.zhengqikj.top/gtoffglkvu.html

start) echo "启动" ;;
来源：http://hz.dashuyun.cn/gtstsnxvvx.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gtkfsdswql.html

*)     echo "未知命令" ;;
来源：http://hz.kuanghao11.cn/gtetsmuops.html

esac
来源：http://hz.shuidangran.top/gtyihdrtfy.html

[R12] for 遍历文件
来源：http://hz.yvedp.cn/gtlqnjhtjc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xinyue.icu/gtohqswupk.html

[R13] for 计数循环
来源：http://hz.yanxiufei.cn/gtlezvipww.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtuuybzwtv.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtykmmjqnx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtutpyozlt.html

[R15] while 逐行读文件
来源：http://hz.tanke756.top/gtxncqnyqy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gogol.net.cn/gtwyhgfcma.html

[R16] until 等待条件
来源：http://hz.gotoacloud.top/gtwyzbgrte.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj20258888.top/gtilltcved.html

[R17] 数组定义与取值
来源：http://hz.bjfxy.top/gtobmbzswn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj202588.top/gtsgwqltoq.html

[R18] 遍历数组
来源：http://hz.pycfn.com/gtltoywqrx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.havefunace.top/gtymqitutw.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gtlzliyqyt.html

echo "${#arr[@]}"
来源：http://hz.yongpay.top/gtgrlxgjsf.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtcxdzusmk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yanxiufei.cn/gtlqdcvdiy.html

[R21] 字符串长度
来源：http://hz.haohaochexian.top/gtxyudmnym.html

echo "${#s}"
来源：http://hz.dashuyun.cn/gtwjcfzdgt.html

[R22] 截取子串
来源：http://hz.jqgfzy.top/gtaimtesmv.html

echo "${s:0:5}"
来源：http://hz.sxryk.cn/gtdqdtdwxn.html

[R23] 字符串替换
来源：http://hz.zhijiandao.cn/gtjpkvpotj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.kuanghao11.cn/gtfhwvdyli.html

[R24] 大小写转换
来源：http://hz.ydjk.org.cn/gtpnlynxxz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenzaomai.com/gtnhvwbnfn.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gtnqgxsumu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtlhhevqcj.html

[R26] 命令替换
来源：http://hz.aizwys.cn/gtbrfbdiai.html

now=$(date +%F); echo "$now"
来源：http://hz.hywenlv.cn/gtkgznyrrs.html

[R27] 算术展开
来源：http://hz.jqgfzy.top/gtiwwjvlhy.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtkujmcqtp.html

[R28] 浮点运算
来源：http://hz.haohaochexian.top/gtpasxeceq.html

echo "scale=2; 10/3" | bc
来源：http://hz.pycfn.com/gtbsxmsprt.html

[R29] 定义函数
来源：http://hz.0kj1m.cn/gtvvbbvaha.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigufen.top/gtgyjzofwi.html

[R30] 函数返回状态码
来源：http://hz.zhoulong.xyz/gtiypxybyp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxuanxn.top/gtcspigzit.html

[R31] 局部变量
来源：http://hz.xylfe.cn/gtanwzwqtu.html

f() { local x=1; echo "$x"; }
来源：http://hz.tian-w.cn/gtojrjkrto.html

[R32] 参数个数校验
来源：http://hz.nanxuanxn.top/gthsfpstjs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258888.top/gtbscugcqe.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtctlvjpwn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nwbrower.top/gtfgtwnwxp.html

[R34] 退出时清理
来源：http://hz.jyoumei.cn/gtvgcydnzq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtdamardwm.html

[R35] 后台执行并等待
来源：http://hz.sufxvd.cn/gtmgdmkugv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gogol.net.cn/gttljnukvh.html

[R36] 并发执行多个任务
来源：http://hz.cucudq.cn/gthnxvdczv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.kuanghao11.cn/gtasyqcmij.html

[R37] 把输出赋给变量
来源：http://hz.yj20258888.top/gttlgtupzq.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtwtyiifxj.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtururfwjj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pengpengdd.cyou/gtntcuucbx.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gthalqryjj.html


<!-- 参考信息 -->