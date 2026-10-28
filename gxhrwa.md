代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ppjwa.cn/gtuxebqgth.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ivvv.top/gtlejvksal.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tian-w.cn/gtbugwplee.html

[P08] 处理浮点精度问题
来源：http://hz.shzxlz.cn/gtdwjynpmp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sysykeji.top/gtdtfkwdbq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhongyouzk.top/gteiyxkkck.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.meibo888.top/gtoxxhmxzn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.316326.xyz/gtiqneanqk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yanxiufei.cn/gtevmncvmo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhengqikj.top/gtxtaggddf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.redwolf501.top/gtxypfndok.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shzxlz.cn/gtrstiqdoq.html

================================================================================
来源：http://hz.zycfv.cn/gtttlluiei.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cdnleiting.top/gtduxfgmta.html

================================================================================
来源：http://hz.yvedp.cn/gtanxeqtwt.html

[Q01] 创建表
来源：http://hz.jinghuilouyu.cn/gtffqszgjt.html

CREATE TABLE users (
来源：http://hz.yuxming.cn/gtviludoyg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtudlcwcei.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jlsjyb.cn/gttzkkjthn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhoulong.xyz/gteoaxjoxe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuxming.cn/gtkpsegejx.html

);
来源：http://hz.hnxiangtu.top/gtrvazcvsi.html

[Q02] 创建带外键的表
来源：http://hz.zhaomingkeji.xyz/gtcxyhjrll.html

CREATE TABLE orders (
来源：http://hz.nwbrower.top/gtsazeoxez.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtgprmpmpf.html

user_id INT NOT NULL,
来源：http://hz.cucudq.cn/gtlctxbwno.html

amount DECIMAL(10, 2),
来源：http://hz.gogol.net.cn/gtzgyblhnb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenlongwang.top/gtvcagwchx.html

);
来源：http://hz.dianchejie.cn/gtsquoulrj.html

[Q03] 增加列
来源：http://hz.tian-w.cn/gtpjlmlkua.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.quarkkingdee.top/gtyumxrshj.html

[Q04] 修改列类型
来源：http://hz.xuetiantiany.cn/gtofskkkuh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj20258.top/gtrunbzvch.html

[Q05] 重命名列
来源：http://hz.aibaodan.cn/gtuqpdaojk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtwvvfqbuw.html

[Q06] 删除列
来源：http://hz.dianchejie.cn/gtvxhpbhjj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gotoacloud.top/gtsxivjasp.html

[Q07] 删除表
来源：http://hz.fengsongda.top/gtnonvpxnq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangkeji.top/gtwwgaooiq.html

[Q08] 创建普通索引
来源：http://hz.yangfankeji.com/gthjzvtboy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gzhubu.top/gtpazqmoht.html

[Q09] 创建唯一索引
来源：http://hz.cqqwz.cn/gtxcnlbjoi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtpnokughw.html

[Q10] 插入单行
来源：http://hz.tian-w.cn/gtfiypgjcp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgufenzy.top/gttqjsylex.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gtrnxuuick.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jlsjyb.cn/gtmizfkxsg.html

[Q12] 插入后取自增 ID
来源：http://hz.hnqzz.top/gtzjqkrvxn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hammf.cn/gtjgkmvtmc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.birdmap.top/gtlkmjajxi.html

[Q13] 忽略重复插入
来源：http://hz.xingfuxueyuan.xyz/gtppqxkjco.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shzxlz.cn/gtzsudcsvr.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangkeji.top/gtpxtzpyaw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj202588.top/gtkookgxtt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tianlin.xyz/gtfqvlxcyd.html

[Q15] 查询全部
来源：http://hz.shanyushiyangkeji.top/gtsutwwnlq.html

SELECT * FROM users;
来源：http://hz.cheryme.top/gtkfnponmr.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gthxcsarrx.html

SELECT id, name FROM users;
来源：http://hz.chenlongwang.top/gtyuakpakm.html

[Q17] 条件查询
来源：http://hz.mhx1999.top/gtenmdkaug.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydzc1.top/gtdtzxeohl.html

[Q18] 模糊匹配
来源：http://hz.sxryk.cn/gtstfelbqt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhixingplan.top/gtiesesixb.html

[Q19] 范围查询
来源：http://hz.wangdashe.top/gtxvkrdtuy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.havefunace.top/gtwkhvmhul.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtqxwnwamv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ybcxt.top/gtxqvkrpua.html

[Q21] 空值判断
来源：http://hz.hnqzz.top/gtrpedveqa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangtech.top/gttpstvwgk.html

[Q22] 排序
来源：http://hz.iojbl.cn/gthnklnxxo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhixingplan.top/gtepstskby.html

[Q23] 分页
来源：http://hz.yonumen.top/gtrxptvxhb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gtzjskgvio.html

[Q24] 去重
来源：http://hz.cqqwz.cn/gtlsswdwtt.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtxwjthybu.html

[Q25] 只取前 N 条
来源：http://hz.nwbrower.top/gtbwbsbugj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yangfankeji.com/gtwexreyyr.html

[Q26] 计数
来源：http://hz.yj20258.top/gtkbobuqyd.html

SELECT COUNT(*) FROM users;
来源：http://hz.hammf.cn/gtvovfcnok.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gttapvxqtb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jiagoushi.top/gthuqnohpe.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtocumvppy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tianlin.xyz/gtwqclauqb.html

[Q29] 最大最小值
来源：http://hz.shangyingyoupin.top/gtrnfvmgwk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxinkj.top/gtgwbeqnvm.html

[Q30] 分组统计
来源：http://hz.gzhubu.top/gtkdarqczq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtemeeuxcq.html

[Q31] 分组后过滤
来源：http://hz.9152youxi.cn/gtswfnlhro.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yongpay.top/gtmoomzxml.html

[Q32] 分组拼接字符串
来源：http://hz.nanxuanxn.top/gtjczenqoq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtzmyxtgiw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cqqwz.cn/gtzmleadkv.html

[Q33] 多列分组
来源：http://hz.daxiang520.top/gtaeafbsof.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenlongwang.top/gtoeinomvj.html

[Q34] 每组取第一条
来源：http://hz.iojbl.cn/gtgjxlgakf.html

SELECT * FROM (
来源：http://hz.tian-w.cn/gtbyuklthb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zdqjudy.top/gteqxilkac.html

) t WHERE rn = 1;
来源：http://hz.jinghuilouyu.cn/gtuhalszce.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gteljnrnwp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtbxydeihu.html

[Q36] 左连接
来源：http://hz.chenzaomai.com/gtdttykvjo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtmbanosiq.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtnwwszslp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cqqwz.cn/gtufkgacxq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ybcxt.top/gthwdlanyt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenlongwang.top/gtyxpgkhbc.html

[Q39] 自连接（查上下级）
来源：http://hz.yvedp.cn/gtllbkwags.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigfzy.top/gtyksfubye.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.bjfxy.top/gttryejmxx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhixingplan.top/gtpqczeafo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xylfe.cn/gtecrxouey.html

[Q41] 多表连接
来源：http://hz.sxryk.cn/gtwxprlohb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daria6918.cn/gttgzwexnj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ybcxt.top/gtxowmodgs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtmfqygruv.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigfzy.top/gtzqzxxsqq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yanxiufei.cn/gtjvadwnto.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinghuilouyu.cn/gtmuayneiw.html

[Q43] 标量子查询
来源：http://hz.jqgufenzy.top/gttljlotgl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.316326.xyz/gtnqfvlgbp.html

[Q44] IN 子查询
来源：http://hz.cdnleiting.top/gtcpyhzkkf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtdzmhmtwi.html

[Q45] EXISTS 判断存在
来源：http://hz.cdnleiting.top/gtoifwgcye.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtnnhztqyj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gzhubu.top/gtxwigapdg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daria6918.cn/gtmwzqinrm.html

[Q47] 与平均值比较
来源：http://hz.yueranfly.top/gtamtvyqcb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xziqi.cn/gtmychjnmr.html

[Q48] CTE 公用表表达式
来源：http://hz.chenjidiqi.icu/gtxzsfylbf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhixingplan.top/gtarnnpsle.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangshuangyany.cn/gtyedesjzn.html

[Q49] 更新单行
来源：http://hz.c1oappe.top/gtyjiqqtkp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtfhzjixfz.html

[Q50] 批量更新
来源：http://hz.jianghu66.top/gtadrosvqm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hfpthk.cn/gtfagnvmyy.html

[Q51] 用子查询更新
来源：http://hz.hysaishi.cn/gtzzzqjhni.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hfpthk.cn/gtwvinkumx.html

[Q52] 删除指定行
来源：http://hz.hywenlv.cn/gtvcxdyncx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.meibo888.top/gtkqnqwiqq.html

[Q53] 按条件删除
来源：http://hz.xinyue.icu/gtbejpvcji.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.kuanghao11.cn/gtfdkltzfw.html

[Q54] 清空表
来源：http://hz.cheryme.top/gtoiapjtct.html

TRUNCATE TABLE logs;
来源：http://hz.chenjidiqi.icu/gtufrcylmg.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigufen.top/gtcowzadmv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydzc1.top/gtcstkqvpz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxuanxn.top/gtodrezjqv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jiagoushi.top/gtnlcyvysk.html

[Q57] 行号
来源：http://hz.tanke756.top/gtouqhawgb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydjk.org.cn/gtdsowmyfh.html

[Q58] 累计求和
来源：http://hz.dianchejie.cn/gtwxiujgae.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shuidangran.top/gtqqluxyfo.html

[Q59] 分组内累计
来源：http://hz.havefunace.top/gtjtpivpnf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuetiantiany.cn/gtzvkloanm.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydzc1.top/gtsgctlijn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zdqjudy.top/gttpfrxcut.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.c1oappe.top/gtcptpufxc.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtcuwbdcir.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhoulong.xyz/gtsqenqdaq.html

[Q62] 分组占比
来源：http://hz.yueranfly.top/gtzgglnivq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtnsvqdqni.html

[Q63] 开启事务
来源：http://hz.cashguo.top/gtivpkiagn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.0kj1m.cn/gtkavkwrnj.html

[Q64] 提交事务
来源：http://hz.mhx1999.top/gtkdcgmeus.html

COMMIT;
来源：http://hz.hywenlv.cn/gtxjpdhtnh.html

[Q65] 回滚事务
来源：http://hz.zhijiandao.cn/gtwctyyrtk.html

ROLLBACK;
来源：http://hz.yonumen.top/gtnbylnteq.html

[Q66] 行锁查询
来源：http://hz.cqqwz.cn/gtuuviiyaf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jlsjyb.cn/gtrwnqzfpj.html

[Q67] 设置隔离级别
来源：http://hz.0kj1m.cn/gtmcprefbm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.mhx1999.top/gtxjomduhm.html

[Q68] 保存点
来源：http://hz.vqdsnc.cn/gtwvroriyu.html

SAVEPOINT sp1;
来源：http://hz.xingfuxueyuan.xyz/gthpsrhcjp.html

ROLLBACK TO sp1;
来源：http://hz.yueranfly.top/gtgdelxtry.html

[Q69] 查看执行计划
来源：http://hz.c1oappe.top/gtqbnmsdug.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.bjfxy.top/gtlkwfwypd.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangkeji.top/gtueglnbxv.html

ANALYZE TABLE users;
来源：http://hz.zhixingplan.top/gttddswurm.html

[Q71] 查看建表语句
来源：http://hz.fengsongda.top/gtwkhzkvkd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinqigufen.top/gtefyidzqv.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtkzgnjawk.html

SHOW INDEX FROM users;
来源：http://hz.vqdsnc.cn/gtshyzsdds.html

[Q73] 查看表状态
来源：http://hz.9152youxi.cn/gtxfkazkgk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.smart0.xyz/gtxzlpmuwt.html

[Q74] 强制使用索引
来源：http://hz.zhoulong.xyz/gtgmkcbcax.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hfpthk.cn/gtbgoigehv.html

[Q75] 日期格式化
来源：http://hz.hysaishi.cn/gtrhmbzmkc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jqgufenzy.top/gtpeyzrwkz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydjk.org.cn/gtvcaxtyzd.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gtlozhfjgz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shuidangran.top/gteamjsdmt.html

[Q77] 时间加减
来源：http://hz.xinyue.icu/gtkuwbgddd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yonumen.top/gturmzcyti.html

[Q78] 当前时间
来源：http://hz.xziqi.cn/gtcfiwjezc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yueranfly.top/gtodjysquz.html

[Q79] 字符串拼接
来源：http://hz.andypj.xyz/gttykggopy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258.top/gtkvuwooht.html

[Q80] 字符串截取
来源：http://hz.jinyuanbaomall.cn/gttnhlhhnh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnqzz.top/gtiefioemr.html

[Q81] 字符串替换
来源：http://hz.nanxinkj.top/gtiywjmyba.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj202588.top/gtjpkdtjng.html

[Q82] 字符长度与字节长度
来源：http://hz.zhijiandao.cn/gtiympctcr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xinyue.icu/gtawnhlekz.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtpfxxvrii.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuanzhike.top/gttzzrcjmj.html

[Q84] 去除首尾空格
来源：http://hz.haohaochexian.top/gtriekjdlf.html

SELECT TRIM(name) FROM users;
来源：http://hz.sufxvd.cn/gtdiezflaa.html

[Q85] 数值取整
来源：http://hz.nanxuanxn.top/gtwswmpata.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtotxzmsvm.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtajfzewbe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yonumen.top/gtpesuaadp.html

[Q87] JSON 字段做条件
来源：http://hz.quarkkingdee.top/gtbccqaida.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.feifeiyinyue.top/gtcsjnoqlk.html

[Q88] 行转列（条件聚合）
来源：http://hz.hysaishi.cn/gtnecpnijp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zdqjudy.top/gtbujovuqj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fengsongda.top/gtwnpqrail.html

[Q89] 判断表是否存在
来源：http://hz.xingfuxueyuan.xyz/gtlixkclsn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.svipenyu.cn/gtngfbjdpf.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtvtzgfxty.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shzxlz.cn/gtwcrxgzhg.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtxpwylnwx.html

R. Bash 专题
来源：http://hz.zhixingplan.top/gtmrrzdpqz.html

================================================================================
来源：http://hz.yuxming.cn/gtdmojltkt.html

[R01] shebang 与严格模式
来源：http://hz.hongshengwenyu.top/gttektsoeg.html

#!/usr/bin/env bash
来源：http://hz.zhoulong.xyz/gttwisoipo.html

set -euo pipefail
来源：http://hz.sysykeji.top/gtnodgxcol.html

[R02] 变量赋值与使用
来源：http://hz.sysykeji.top/gtieixmrqf.html

name="Tom"; echo "$name"
来源：http://hz.zhoulong.xyz/gtgjlhbufm.html

[R03] 只读变量
来源：http://hz.pengpengdd.cyou/gtedxcpxdo.html

readonly PI=3.14
来源：http://hz.hammf.cn/gtuawvaudf.html

[R04] 位置参数
来源：http://hz.jianghu66.top/gtemriuhfx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fengsongda.top/gtqjjfejgu.html

[R05] 参数默认值
来源：http://hz.xingfuxueyuan.xyz/gtpsccyxor.html

name="${1:-default}"
来源：http://hz.gzhubu.top/gtvyisumkr.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangtech.top/gtcnpzhhyk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.52xcode.cn/gtknzmbiza.html

[R07] if 判断文件
来源：http://hz.sufxvd.cn/gtwxwtqtqs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.birdmap.top/gtzzvkztnh.html

[R08] 数值比较
来源：http://hz.dianchejie.cn/gtnnjeifsj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhoulong.xyz/gttcuttyoy.html

[R09] 字符串比较
来源：http://hz.52xcode.cn/gtxrzchyhz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tianlin.xyz/gtvrmcmfmj.html

[R10] 正则匹配
来源：http://hz.sysykeji.top/gtxqxemokr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fzhhl.top/gttxcccdxm.html

[R11] case 多分支
来源：http://hz.yvedp.cn/gtbkcchwvs.html

case "$1" in
来源：http://hz.guannengcc.top/gteoqdazwx.html

start) echo "启动" ;;
来源：http://hz.jqgfzy.top/gtlecloebw.html

stop)  echo "停止" ;;
来源：http://hz.52xcode.cn/gtujtrfvif.html

*)     echo "未知命令" ;;
来源：http://hz.andypj.xyz/gtmjbavypk.html

esac
来源：http://hz.birdmap.top/gtjcdqggbt.html

[R12] for 遍历文件
来源：http://hz.hysaishi.cn/gtxjsmvytq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258.top/gtallzzqrj.html

[R13] for 计数循环
来源：http://hz.birdmap.top/gtdvhjplhb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.52xcode.cn/gtxkjchvab.html

[R14] C 风格 for
来源：http://hz.gotoacloud.top/gttkctgofm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtzwdskego.html

[R15] while 逐行读文件
来源：http://hz.daria6918.cn/gtqqgxlapv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shuidangran.top/gthpamkgym.html

[R16] until 等待条件
来源：http://hz.hnqzz.top/gtlbmeltts.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xuanzx.com/gtelptsdid.html

[R17] 数组定义与取值
来源：http://hz.hfpthk.cn/gtzlmpofan.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zycfv.cn/gtwzitpzmc.html

[R18] 遍历数组
来源：http://hz.gzhubu.top/gtxgwcqagc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daxiang520.top/gtxsalpcaz.html

[R19] 数组长度
来源：http://hz.yuxming.cn/gtyfwihoqa.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gtgfyqxdbl.html

[R20] 关联数组（字典）
来源：http://hz.nanxinkj.top/gtvgyfthpy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtrikthqgr.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gtklkktewf.html

echo "${#s}"
来源：http://hz.cucudq.cn/gtvexirhpj.html

[R22] 截取子串
来源：http://hz.shzxlz.cn/gtuowszegs.html

echo "${s:0:5}"
来源：http://hz.andypj.xyz/gtznukxerm.html

[R23] 字符串替换
来源：http://hz.sysykeji.top/gtgccvcvom.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtcqaqlxsj.html

[R24] 大小写转换
来源：http://hz.feifeiyinyue.top/gtdvervbul.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gotoacloud.top/gtmetwbgko.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenlongwang.top/gtwwoyfmlf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nwbrower.top/gtaicrniti.html

[R26] 命令替换
来源：http://hz.daria6918.cn/gtyobtejff.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtohtjplzf.html

[R27] 算术展开
来源：http://hz.ppjwa.cn/gtfmqnujbf.html

echo $((1 + 2 * 3))
来源：http://hz.shuidangran.top/gtvhwexrwu.html

[R28] 浮点运算
来源：http://hz.yueranfly.top/gtoyposgam.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuanzx.com/gtrtbwrqib.html

[R29] 定义函数
来源：http://hz.zdqjudy.top/gtaiacfnmq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ydzc1.top/gtdesnwnlc.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangkeji.top/gtnczxkvjm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenlongwang.top/gtarceibip.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gttwssfspb.html

f() { local x=1; echo "$x"; }
来源：http://hz.yongpay.top/gtkokvncjm.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtvszdeuga.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtrbiwxasy.html

[R33] 捕获错误并提示行号
来源：http://hz.svipenyu.cn/gthwlivdut.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xziqi.cn/gtuibipogh.html

[R34] 退出时清理
来源：http://hz.sweek.top/gtoyhfqiwu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gteiuiaqlo.html

[R35] 后台执行并等待
来源：http://hz.shzxlz.cn/gtxyglccsx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangtech.top/gtknvwgdxe.html

[R36] 并发执行多个任务
来源：http://hz.guowangkeji.top/gtcnaoyxxz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tian-w.cn/gtzathzeff.html

[R37] 把输出赋给变量
来源：http://hz.nwbrower.top/gtlcvpjawj.html


<!-- 参考信息 -->