代发 wailian999

================================================================================
来源：http://hz.0kj1m.cn/gtfgifeyin.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhaomingkeji.xyz/gtovnqkpyp.html

================================================================================
来源：http://hz.yonumen.top/gtxtjhundl.html

[Q01] 创建表
来源：http://hz.yvedp.cn/gtzkcqtssb.html

CREATE TABLE users (
来源：http://hz.shanyushiyangkeji.top/gtadejyjmy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtgeorivuj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sxryk.cn/gttqdziwvq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jiagoushi.top/gtxpagmiew.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.svipenyu.cn/gtfawzqdhw.html

);
来源：http://hz.jyoumei.cn/gtdsnyetea.html

[Q02] 创建带外键的表
来源：http://hz.daria6918.cn/gtxoqzwwsg.html

CREATE TABLE orders (
来源：http://hz.iojbl.cn/gtphnoxhec.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtctrggwws.html

user_id INT NOT NULL,
来源：http://hz.quarkkingdee.top/gtvnzhirkd.html

amount DECIMAL(10, 2),
来源：http://hz.tian-w.cn/gtlewqlugk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenlongwang.top/gtnqoxuceg.html

);
来源：http://hz.xziqi.cn/gtjyxktsrn.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gtogtoxemf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cqqwz.cn/gtrhnsvzhn.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtoxqiwkao.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtjgokhwtz.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtdvmqqsha.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zdqjudy.top/gtyghnoltv.html

[Q06] 删除列
来源：http://hz.pengpengdd.cyou/gtbimthssu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shanyushiyangtech.top/gtidfjjiye.html

[Q07] 删除表
来源：http://hz.daxiang520.top/gttoctezlk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.daria6918.cn/gtroaglesu.html

[Q08] 创建普通索引
来源：http://hz.jinqigufen.top/gtornimmjw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.havefunace.top/gtljejxprg.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gtccvyvrxh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtehjhcska.html

[Q10] 插入单行
来源：http://hz.zhiwuduotai.top/gthdarcdbf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhiwuduotai.top/gtvvykdkri.html

[Q11] 一次插入多行
来源：http://hz.hywenlv.cn/gtvqxhcycw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jiagoushi.top/gtfqnybetm.html

[Q12] 插入后取自增 ID
来源：http://hz.zhijiandao.cn/gtbeflqpox.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtsyuuvfmz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ehwqpu.com/gtjrckshwe.html

[Q13] 忽略重复插入
来源：http://hz.jinyuanbaomall.cn/gtlypficiw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hysaishi.cn/gtwmcbecmu.html

[Q14] 存在则更新（upsert）
来源：http://hz.316326.xyz/gthqcughyp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daria6918.cn/gthoehydcx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhiwuduotai.top/gtqyfupbig.html

[Q15] 查询全部
来源：http://hz.sxryk.cn/gtbwfeopen.html

SELECT * FROM users;
来源：http://hz.jlsjyb.cn/gtiejinczi.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gtktzqepbw.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangkeji.top/gthkqvwowq.html

[Q17] 条件查询
来源：http://hz.bjfxy.top/gtonoxejkn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yongpay.top/gtrprepsbo.html

[Q18] 模糊匹配
来源：http://hz.ydjk.org.cn/gtzmazchrl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hammf.cn/gtucjsfusj.html

[Q19] 范围查询
来源：http://hz.hongshengwenyu.top/gttptsdbka.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.52xcode.cn/gtaocrleuk.html

[Q20] IN 列表
来源：http://hz.gogol.net.cn/gtqybfntan.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nanxinkj.top/gtnahclvgo.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtbgrsdiwv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sufxvd.cn/gtltjyamaq.html

[Q22] 排序
来源：http://hz.cashguo.top/gtlnqwgity.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yanxiufei.cn/gtopvnifcc.html

[Q23] 分页
来源：http://hz.jinqigfzy.top/gtrduqyfml.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shuidangran.top/gteoskkwci.html

[Q24] 去重
来源：http://hz.zdqjudy.top/gtosdxtyja.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gttfxlmauz.html

[Q25] 只取前 N 条
来源：http://hz.ydzc1.top/gtquuksssq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtmehyombs.html

[Q26] 计数
来源：http://hz.jinqigfzy.top/gttzuriqop.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gtmdhqvajx.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gtneddrlae.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangkeji.top/gtacishlug.html

[Q28] 求和与平均
来源：http://hz.shuidangran.top/gtiikzsoin.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gtvhkwamdb.html

[Q29] 最大最小值
来源：http://hz.quarkkingdee.top/gtvaneerun.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gotoacloud.top/gtqyvwnjbr.html

[Q30] 分组统计
来源：http://hz.hysaishi.cn/gtjhpzpifu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtrbflzdhk.html

[Q31] 分组后过滤
来源：http://hz.316326.xyz/gtekpydfmd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuxming.cn/gtboxghwpj.html

[Q32] 分组拼接字符串
来源：http://hz.0kj1m.cn/gtfxeheezn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtzosrtofe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.haohaochexian.top/gtrastizcv.html

[Q33] 多列分组
来源：http://hz.cheryme.top/gtfgqkneot.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258888.top/gteqotvrel.html

[Q34] 每组取第一条
来源：http://hz.snrcjt.cn/gtuvdpzmmy.html

SELECT * FROM (
来源：http://hz.chenlongwang.top/gtvuekljac.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jyoumei.cn/gtzfwzssxw.html

) t WHERE rn = 1;
来源：http://hz.jiagoushi.top/gtcdbfhlso.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gtndrmzlwn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.mhx1999.top/gtoqkyuqve.html

[Q36] 左连接
来源：http://hz.shuidangran.top/gtusfwklws.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtkzdwoatx.html

[Q37] 右连接
来源：http://hz.wangdashe.top/gtlwwvzapj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gtuqfuqlsm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hysaishi.cn/gtprruailc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtxlsvinqc.html

[Q39] 自连接（查上下级）
来源：http://hz.sysykeji.top/gtrkrfrcsk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuanzhike.top/gtqfdxilmb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gaohongyu789.top/gtlrulfgvf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jianghu66.top/gtjzctutwl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangshuangyany.cn/gtwckhgsmw.html

[Q41] 多表连接
来源：http://hz.tianlin.xyz/gtcjmnhtho.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtcqkpmklc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shangyingyoupin.top/gtxziulabp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhijiandao.cn/gtgehkdveg.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtjcbhnivu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhengqikj.top/gtwlnpctup.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenjidiqi.icu/gtzauvczcn.html

[Q43] 标量子查询
来源：http://hz.shanyushiyangkeji.top/gtrthpfzub.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gtdfyeagow.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangkeji.top/gtlbstuoey.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenjidiqi.icu/gtygsfltsf.html

[Q45] EXISTS 判断存在
来源：http://hz.cdnleiting.top/gtqhkjbjxr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gttnqneigh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuxming.cn/gtxihfmlpw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtavffwtlu.html

[Q47] 与平均值比较
来源：http://hz.havefunace.top/gtpmfbnhyn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dianchejie.cn/gthdufflyb.html

[Q48] CTE 公用表表达式
来源：http://hz.cashguo.top/gtetndsamg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtnepngpsw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtyejctzmm.html

[Q49] 更新单行
来源：http://hz.svipenyu.cn/gtehkefqjm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sysykeji.top/gtuufjrvet.html

[Q50] 批量更新
来源：http://hz.yuanzhike.top/gtowpcweqa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.snrcjt.cn/gtqnlrevje.html

[Q51] 用子查询更新
来源：http://hz.zhengqikj.top/gtkgjhsahf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinyuanbaomall.cn/gtphemoyga.html

[Q52] 删除指定行
来源：http://hz.cucudq.cn/gtxzmdyaos.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dianchejie.cn/gtpwzgaxjk.html

[Q53] 按条件删除
来源：http://hz.yj20258888.top/gtdzwcsunx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj202588.top/gtnxfqqthg.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gtuvehroqh.html

TRUNCATE TABLE logs;
来源：http://hz.xinyue.icu/gtdjlluopo.html

[Q55] 排名（并列占位）
来源：http://hz.xylfe.cn/gtjlybfvgp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yanxiufei.cn/gtwvkodrkn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuanzhike.top/gtdbprquhd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtadekymrb.html

[Q57] 行号
来源：http://hz.chenzaomai.com/gtzritdvat.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgufenzy.top/gtsmicsysw.html

[Q58] 累计求和
来源：http://hz.hnxiangtu.top/gthnmyzrxm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guowangkeji.top/gtnlzfmxep.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gtcbyrxpcu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgfzy.top/gtxoqjnfpk.html

[Q60] 取上一行 / 下一行
来源：http://hz.birdmap.top/gtlrgijsej.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gaohongyu789.top/gtqqalkxym.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yonumen.top/gtcinzckpu.html

[Q61] 移动平均
来源：http://hz.hnqzz.top/gtybzwoqvc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shuidangran.top/gtluufpwbv.html

[Q62] 分组占比
来源：http://hz.yj20258.top/gtkuqvfmrx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtdadodiid.html

[Q63] 开启事务
来源：http://hz.ydzc1.top/gtrghivitf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yonumen.top/gtsesciujj.html

[Q64] 提交事务
来源：http://hz.ywan-chungtsiang.top/gtrauclpks.html

COMMIT;
来源：http://hz.shuidangran.top/gtnpjeehgy.html

[Q65] 回滚事务
来源：http://hz.ppjwa.cn/gtrywkwtye.html

ROLLBACK;
来源：http://hz.zhixingplan.top/gtuuyiwpoc.html

[Q66] 行锁查询
来源：http://hz.yuanzhike.top/gtsjiyfnak.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.0kj1m.cn/gtqwobngow.html

[Q67] 设置隔离级别
来源：http://hz.sysykeji.top/gtudyedhuy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hfpthk.cn/gtbbwsxezs.html

[Q68] 保存点
来源：http://hz.gzhubu.top/gtbdzjfnlk.html

SAVEPOINT sp1;
来源：http://hz.hysaishi.cn/gthdpqsfkf.html

ROLLBACK TO sp1;
来源：http://hz.daria6918.cn/gtuhkvghhv.html

[Q69] 查看执行计划
来源：http://hz.jinyuanbaomall.cn/gtvhuhwbgm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tianlin.xyz/gtwgehbyje.html

[Q70] 更新统计信息
来源：http://hz.yanxiufei.cn/gtqskeawmp.html

ANALYZE TABLE users;
来源：http://hz.jiagoushi.top/gtmesotuen.html

[Q71] 查看建表语句
来源：http://hz.tanke756.top/gtugzyfvkg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ywan-chungtsiang.top/gtwylmgkgx.html

[Q72] 查看索引
来源：http://hz.sxryk.cn/gtkowsbcwj.html

SHOW INDEX FROM users;
来源：http://hz.yj20258888.top/gtzsihhmyb.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangkeji.top/gtczsohhce.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pengpengdd.cyou/gtltuunlmv.html

[Q74] 强制使用索引
来源：http://hz.redwolf501.top/gtaygtluld.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtleqhrmju.html

[Q75] 日期格式化
来源：http://hz.hfpthk.cn/gtcttyhntu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guowangkeji.top/gtmzcjipxi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.52xcode.cn/gtiztnxnkz.html

[Q76] 按天统计
来源：http://hz.jinqigufen.top/gteuyxnkrp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuanzx.com/gttsxttmrz.html

[Q77] 时间加减
来源：http://hz.yj20258888.top/gtxgnlxlyi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtbsdfcoki.html

[Q78] 当前时间
来源：http://hz.daria6918.cn/gtulhqboqu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhixingplan.top/gtfjfgwwrh.html

[Q79] 字符串拼接
来源：http://hz.zhengqikj.top/gtxpeutcfb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dashuyun.cn/gtkzbzajae.html

[Q80] 字符串截取
来源：http://hz.aibaodan.cn/gtznyrlzdy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hysaishi.cn/gtxmbykbxe.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtslzdkzre.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gotoacloud.top/gtsfkiwats.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtnsbgnace.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtfhjeqwnt.html

[Q83] 大小写转换
来源：http://hz.hysaishi.cn/gtihhdygkt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgfzy.top/gtdxiqlfhk.html

[Q84] 去除首尾空格
来源：http://hz.gaohongyu789.top/gtmjcsqamb.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnqzz.top/gtchtsxfdm.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gtpjbemakt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangtech.top/gtbmotnnut.html

[Q86] 读取 JSON 字段
来源：http://hz.shangyingyoupin.top/gtupnlsjyr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aibaodan.cn/gthitqyvvh.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gthlnpxzti.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.iojbl.cn/gtmuziqyol.html

[Q88] 行转列（条件聚合）
来源：http://hz.sweek.top/gtamycntzl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtnnvdkttj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fengsongda.top/gtaramaqqx.html

[Q89] 判断表是否存在
来源：http://hz.nwbrower.top/gtiuxuysza.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.haohaochexian.top/gtklxktzhn.html

[Q90] 生成序号列
来源：http://hz.gaohongyu789.top/gtvqfkwseo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.mhx1999.top/gtqtuoxbst.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtkxajwqsw.html

R. Bash 专题
来源：http://hz.zhiwuduotai.top/gtdgkxefnz.html

================================================================================
来源：http://hz.cucudq.cn/gtdwiojqat.html

[R01] shebang 与严格模式
来源：http://hz.svipenyu.cn/gtffxumvvh.html

#!/usr/bin/env bash
来源：http://hz.tanke756.top/gtavdmvfzj.html

set -euo pipefail
来源：http://hz.shangyingyoupin.top/gtedvzagvs.html

[R02] 变量赋值与使用
来源：http://hz.ivvv.top/gtyafoypra.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtgunnhthj.html

[R03] 只读变量
来源：http://hz.9152youxi.cn/gttuwfowpr.html

readonly PI=3.14
来源：http://hz.pengpengdd.cyou/gtqojyqqhi.html

[R04] 位置参数
来源：http://hz.cheryme.top/gtxckhfvds.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.feifeiyinyue.top/gtwknqzltg.html

[R05] 参数默认值
来源：http://hz.zhaomingkeji.xyz/gtgczlcinv.html

name="${1:-default}"
来源：http://hz.yuxming.cn/gtcabjocds.html

[R06] 判断命令是否存在
来源：http://hz.tanke756.top/gtfozyelqw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigfzy.top/gtukejlmcr.html

[R07] if 判断文件
来源：http://hz.yongpay.top/gtzphkmrug.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenjidiqi.icu/gtlbxrdjxs.html

[R08] 数值比较
来源：http://hz.ydzc1.top/gtoisdupjb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xylfe.cn/gtjajtrvhq.html

[R09] 字符串比较
来源：http://hz.birdmap.top/gtkefrpide.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shanyushiyangkeji.top/gtdpsommob.html

[R10] 正则匹配
来源：http://hz.gaohongyu789.top/gtxcoijzdw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtsihkufvf.html

[R11] case 多分支
来源：http://hz.zhongyouzk.top/gthltexzwx.html

case "$1" in
来源：http://hz.ywan-chungtsiang.top/gtwspjbaei.html

start) echo "启动" ;;
来源：http://hz.nanxinkj.top/gtzntypehh.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangkeji.top/gtghrcaqhd.html

*)     echo "未知命令" ;;
来源：http://hz.jqgufenzy.top/gtmbtkbybd.html

esac
来源：http://hz.gogol.net.cn/gthvakfclp.html

[R12] for 遍历文件
来源：http://hz.dianchejie.cn/gtezpnehxl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinghuilouyu.cn/gtqrstgvnp.html

[R13] for 计数循环
来源：http://hz.iojbl.cn/gtoxpjxevm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtojofqkbv.html

[R14] C 风格 for
来源：http://hz.fengsongda.top/gtpwkrfogw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xinyue.icu/gtazxtlxbw.html

[R15] while 逐行读文件
来源：http://hz.gaohongyu789.top/gtuqvchzyr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yvedp.cn/gttnqfvpgw.html

[R16] until 等待条件
来源：http://hz.hywenlv.cn/gtqfmjhygf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangshuangyany.cn/gtnauqkjvw.html

[R17] 数组定义与取值
来源：http://hz.zdqjudy.top/gtrftwoulx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258.top/gtjbnwzzcm.html

[R18] 遍历数组
来源：http://hz.cdnleiting.top/gtlerlyqhb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydzc1.top/gthsvprtka.html

[R19] 数组长度
来源：http://hz.ppjwa.cn/gtpwvethbz.html

echo "${#arr[@]}"
来源：http://hz.sweek.top/gtnqqdoucp.html

[R20] 关联数组（字典）
来源：http://hz.nanxinkj.top/gtffjaoqxd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shangyingyoupin.top/gtojhcnbzh.html

[R21] 字符串长度
来源：http://hz.cucudq.cn/gtiwqgztnu.html

echo "${#s}"
来源：http://hz.jqgfzy.top/gtxvpetukf.html

[R22] 截取子串
来源：http://hz.shzxlz.cn/gtgzpvuvol.html

echo "${s:0:5}"
来源：http://hz.bjfxy.top/gtyboqwymm.html

[R23] 字符串替换
来源：http://hz.ehwqpu.com/gtocyifevs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ppjwa.cn/gtkztkzswb.html

[R24] 大小写转换
来源：http://hz.hnqzz.top/gtpfujgwpn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guowangkeji.top/gticfvmugd.html

[R25] 去后缀 / 去前缀
来源：http://hz.ehwqpu.com/gtjplbuyrt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nanxinkj.top/gtxygiiqoa.html

[R26] 命令替换
来源：http://hz.0kj1m.cn/gtxtcsskzt.html

now=$(date +%F); echo "$now"
来源：http://hz.hywenlv.cn/gtsckirmwf.html

[R27] 算术展开
来源：http://hz.ppjwa.cn/gtewbhjyxp.html

echo $((1 + 2 * 3))
来源：http://hz.tanke756.top/gtthnqiuvk.html

[R28] 浮点运算
来源：http://hz.dashuyun.cn/gtewpkucwx.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtvxpbppzi.html

[R29] 定义函数
来源：http://hz.cheryme.top/gtxwlzdhqm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenlongwang.top/gtwwekqjwf.html

[R30] 函数返回状态码
来源：http://hz.redwolf501.top/gtdurrpaxz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtcqhwzuhd.html

[R31] 局部变量
来源：http://hz.redwolf501.top/gtdbraabrz.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtbwduksif.html

[R32] 参数个数校验
来源：http://hz.snrcjt.cn/gtovzitlro.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtsfipiole.html

[R33] 捕获错误并提示行号
来源：http://hz.nanxuanxn.top/gtrivfcpoq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtowuwtvol.html

[R34] 退出时清理
来源：http://hz.tian-w.cn/gtsikdohtp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtildxsemg.html

[R35] 后台执行并等待
来源：http://hz.tianlin.xyz/gtmdasqrqg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cqqwz.cn/gtvmebvqhb.html

[R36] 并发执行多个任务
来源：http://hz.redwolf501.top/gtjwwfiikz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.aibaodan.cn/gtstmodwcz.html

[R37] 把输出赋给变量
来源：http://hz.xylfe.cn/gtitmplvaa.html

files=$(ls -1)
来源：http://hz.cucudq.cn/gtnwjfdufx.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtuyrccdmq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhijiandao.cn/gtiennijfs.html

[R39] 重定向标准输出与错误
来源：http://hz.iojbl.cn/gtlnyawjgx.html

cmd > out.log 2>&1
来源：http://hz.tanke756.top/gtkstlrlpf.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gtyuybqmer.html

echo "log" >> out.log
来源：http://hz.wangshuangyany.cn/gtymkkhtps.html

[R41] 丢弃输出
来源：http://hz.yj20258888.top/gtwppckrme.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtwiyrthkz.html

[R42] 输入重定向
来源：http://hz.0kj1m.cn/gtdczqytnp.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtvzlhegad.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtmogwczwo.html


<!-- 参考信息 -->