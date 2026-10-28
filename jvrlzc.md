代发 wailian999

================================================================================
来源：http://hz.shangyingyoupin.top/gtvxtjgepy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.smart0.xyz/gthyfruswh.html

================================================================================
来源：http://hz.cdnleiting.top/gtueihnjlz.html

[Q01] 创建表
来源：http://hz.shangyingyoupin.top/gtftprgqve.html

CREATE TABLE users (
来源：http://hz.ydzc1.top/gtomqmswiv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtmrtseypw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gaohongyu789.top/gtmsqnywpv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigfzy.top/gtznbzsvod.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxinkj.top/gtfhputars.html

);
来源：http://hz.c1oappe.top/gtnxmrfzdz.html

[Q02] 创建带外键的表
来源：http://hz.jqgfzy.top/gtgoiymmyc.html

CREATE TABLE orders (
来源：http://hz.tanke756.top/gtewtlyoro.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yonumen.top/gtretyfjix.html

user_id INT NOT NULL,
来源：http://hz.sxryk.cn/gtwmolnutp.html

amount DECIMAL(10, 2),
来源：http://hz.hfpthk.cn/gtgldieauf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cashguo.top/gtlizpfkry.html

);
来源：http://hz.zdqjudy.top/gtcnkbxxvi.html

[Q03] 增加列
来源：http://hz.quarkkingdee.top/gtvtajrzrt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.mhx1999.top/gtcciaeeqf.html

[Q04] 修改列类型
来源：http://hz.tanke756.top/gtnfmizibh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhoulong.xyz/gtgqxfoopf.html

[Q05] 重命名列
来源：http://hz.smart0.xyz/gtilltlmsz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shuidangran.top/gtcbulftdp.html

[Q06] 删除列
来源：http://hz.yj20258.top/gtozavqdnh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ybcxt.top/gthfqcfjww.html

[Q07] 删除表
来源：http://hz.yuanzhike.top/gtpsabjhnk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yvedp.cn/gtwtixdvjn.html

[Q08] 创建普通索引
来源：http://hz.andypj.xyz/gtntjbdshf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtftotwder.html

[Q09] 创建唯一索引
来源：http://hz.yanxiufei.cn/gtispuyzit.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtvsuudvlw.html

[Q10] 插入单行
来源：http://hz.yj20258.top/gtkvldqork.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhengqikj.top/gtpmyizijl.html

[Q11] 一次插入多行
来源：http://hz.gzhubu.top/gtnwanrtwk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nwbrower.top/gtmqxndmyd.html

[Q12] 插入后取自增 ID
来源：http://hz.dianchejie.cn/gtuoxbhtut.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.c1oappe.top/gtuselxrte.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daxiang520.top/gtpzuburra.html

[Q13] 忽略重复插入
来源：http://hz.nanxinkj.top/gtayupefbn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cdnleiting.top/gtgpivceho.html

[Q14] 存在则更新（upsert）
来源：http://hz.snrcjt.cn/gtcgvkpuph.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hysaishi.cn/gtzgnqzlvq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yuanzhike.top/gtdfqcnwxs.html

[Q15] 查询全部
来源：http://hz.zhoulong.xyz/gtmpfwhbdi.html

SELECT * FROM users;
来源：http://hz.redwolf501.top/gtumqmrrjc.html

[Q16] 查询指定列
来源：http://hz.ppjwa.cn/gtrpyylkbe.html

SELECT id, name FROM users;
来源：http://hz.yonumen.top/gtwzlqvcpj.html

[Q17] 条件查询
来源：http://hz.jianghu66.top/gtvnuhvphe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.bjfxy.top/gtwhnrqpdd.html

[Q18] 模糊匹配
来源：http://hz.nanxinkj.top/gtfmdxcfsr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.svipenyu.cn/gtrxjjmbtl.html

[Q19] 范围查询
来源：http://hz.haohaochexian.top/gtflsmasuh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hongshengwenyu.top/gtaugitvqw.html

[Q20] IN 列表
来源：http://hz.zhongyouzk.top/gttvctwhtg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gtpirtegwl.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtwuqwdfct.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtrniqisvm.html

[Q22] 排序
来源：http://hz.xuanzx.com/gtcmpcwjrs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hywenlv.cn/gthrgctfpw.html

[Q23] 分页
来源：http://hz.fengsongda.top/gtimuirati.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gzhubu.top/gtzwlfboog.html

[Q24] 去重
来源：http://hz.fengsongda.top/gtflxnyfvg.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhaomingkeji.xyz/gtztugovdq.html

[Q25] 只取前 N 条
来源：http://hz.yvedp.cn/gtcnimpbia.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gtyytcqxor.html

[Q26] 计数
来源：http://hz.havefunace.top/gttekmjzqn.html

SELECT COUNT(*) FROM users;
来源：http://hz.ehwqpu.com/gtacvmtchq.html

[Q27] 条件计数
来源：http://hz.daxiang520.top/gtxztudbwj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxuanxn.top/gtpknukhez.html

[Q28] 求和与平均
来源：http://hz.zhongyouzk.top/gtrvkoukcv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xinyue.icu/gtfdrdbrwj.html

[Q29] 最大最小值
来源：http://hz.xuanzx.com/gtnxdiwgtf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xuanzx.com/gtrqlkrxsf.html

[Q30] 分组统计
来源：http://hz.hongshengwenyu.top/gtggdopxqb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtzxfzmhif.html

[Q31] 分组后过滤
来源：http://hz.jiagoushi.top/gtuxgpkioj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nanxuanxn.top/gtjfobufof.html

[Q32] 分组拼接字符串
来源：http://hz.meibo888.top/gtpkkqspln.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtybbdoxey.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenlongwang.top/gtsodvmdwy.html

[Q33] 多列分组
来源：http://hz.cdnleiting.top/gtbjomrlnm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daxiang520.top/gtxiychsyv.html

[Q34] 每组取第一条
来源：http://hz.cqqwz.cn/gtugomhtpv.html

SELECT * FROM (
来源：http://hz.9152youxi.cn/gtvvxneqhe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gtyymwowvp.html

) t WHERE rn = 1;
来源：http://hz.iojbl.cn/gthpmjrnsx.html

[Q35] 内连接
来源：http://hz.xylfe.cn/gtnazpofso.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtkphejrld.html

[Q36] 左连接
来源：http://hz.svipenyu.cn/gtqhvsrcvr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtgijcfqtb.html

[Q37] 右连接
来源：http://hz.yj20258888.top/gtwfvkbtax.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtkyvjfsje.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtobbprusc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dianchejie.cn/gtshwhwqpp.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtnxpuowre.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sufxvd.cn/gtkhnhvxpm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shuidangran.top/gtzvpbqznk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gogol.net.cn/gtfskeaywl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yueranfly.top/gtjyylfufb.html

[Q41] 多表连接
来源：http://hz.guannengcc.top/gtyaervpif.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhijiandao.cn/gtavsulygc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jianghu66.top/gtyazlsodm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.feifeiyinyue.top/gtwvphsogy.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtppiducds.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydjk.org.cn/gtmnoegprq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cqqwz.cn/gtiuhcnvdv.html

[Q43] 标量子查询
来源：http://hz.jinyuanbaomall.cn/gtbflkcfuf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ehwqpu.com/gtomxdxqjy.html

[Q44] IN 子查询
来源：http://hz.feifeiyinyue.top/gtopiqqoor.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtzwbcmcll.html

[Q45] EXISTS 判断存在
来源：http://hz.cqqwz.cn/gtfghrerrj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtsyibpiwm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tianlin.xyz/gtrnsddrfc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtxccznjuh.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangtech.top/gtpoqnisxp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xziqi.cn/gtwwiybjmv.html

[Q48] CTE 公用表表达式
来源：http://hz.yj202588.top/gttyreniin.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gtobfxcwzx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.smart0.xyz/gtxkdaolea.html

[Q49] 更新单行
来源：http://hz.snrcjt.cn/gtdmndvglb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cqqwz.cn/gtczrzrdpd.html

[Q50] 批量更新
来源：http://hz.kuanghao11.cn/gtglxdcahm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtwgoeppjd.html

[Q51] 用子查询更新
来源：http://hz.yj20258.top/gtatmxliqh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sysykeji.top/gthxxlrdxc.html

[Q52] 删除指定行
来源：http://hz.jinyuanbaomall.cn/gtcssuzhkp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yongpay.top/gtvegcjcxt.html

[Q53] 按条件删除
来源：http://hz.pengpengdd.cyou/gteagjlqvv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hongshengwenyu.top/gtxdsuctgs.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtsclciovj.html

TRUNCATE TABLE logs;
来源：http://hz.yonumen.top/gtzwlcipho.html

[Q55] 排名（并列占位）
来源：http://hz.yangfankeji.com/gtubaognkz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhengqikj.top/gtljyardty.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydjk.org.cn/gtxnbwmhxc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.mhx1999.top/gtnqjahjlq.html

[Q57] 行号
来源：http://hz.yueranfly.top/gtyndpulmq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgfzy.top/gtmapfbtfs.html

[Q58] 累计求和
来源：http://hz.hammf.cn/gtrtboavxq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuetiantiany.cn/gtohdptvps.html

[Q59] 分组内累计
来源：http://hz.52xcode.cn/gtskvhkrjf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pycfn.com/gtbfdyaqiz.html

[Q60] 取上一行 / 下一行
来源：http://hz.9152youxi.cn/gtzzfdqaex.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tianlin.xyz/gtqfibinze.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gttbjbdbph.html

[Q61] 移动平均
来源：http://hz.zhijiandao.cn/gtqgkmcrgg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aibaodan.cn/gtunajzyhk.html

[Q62] 分组占比
来源：http://hz.xinyue.icu/gtncxepktd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtsyexkswl.html

[Q63] 开启事务
来源：http://hz.jinghuilouyu.cn/gtyyxeowvm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hywenlv.cn/gtraxtnjzh.html

[Q64] 提交事务
来源：http://hz.cqqwz.cn/gtdsznlfvp.html

COMMIT;
来源：http://hz.haohaochexian.top/gtsvuyeled.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtrtvsbiym.html

ROLLBACK;
来源：http://hz.xingfuxueyuan.xyz/gtojxquvlw.html

[Q66] 行锁查询
来源：http://hz.gzhubu.top/gtzwaimnrj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gtrbbgepfw.html

[Q67] 设置隔离级别
来源：http://hz.zhijiandao.cn/gtnkluzbsb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pengpengdd.cyou/gtvodcnijy.html

[Q68] 保存点
来源：http://hz.yuxming.cn/gtswylctbk.html

SAVEPOINT sp1;
来源：http://hz.wangshuangyany.cn/gtyuzivach.html

ROLLBACK TO sp1;
来源：http://hz.zhiwuduotai.top/gtvhrdvfzh.html

[Q69] 查看执行计划
来源：http://hz.andypj.xyz/gtzhxkdbph.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtztqzheyj.html

[Q70] 更新统计信息
来源：http://hz.xuetiantiany.cn/gtswadhfbg.html

ANALYZE TABLE users;
来源：http://hz.xziqi.cn/gtduzdtuev.html

[Q71] 查看建表语句
来源：http://hz.hongshengwenyu.top/gtqgycftvx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cucudq.cn/gtuykkwikt.html

[Q72] 查看索引
来源：http://hz.tanke756.top/gtbwahffdr.html

SHOW INDEX FROM users;
来源：http://hz.tian-w.cn/gtouqtxbhv.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtdpvkgelu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnqzz.top/gtokbtcfit.html

[Q74] 强制使用索引
来源：http://hz.shuidangran.top/gtgelmcnhe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258888.top/gtivllnlnz.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gtkdnqbzme.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangdashe.top/gtfqndgvpx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gtgrtgjsyq.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtetzzejyq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.quarkkingdee.top/gtyjyorszo.html

[Q77] 时间加减
来源：http://hz.ywan-chungtsiang.top/gtzekucdka.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gtaddqstqv.html

[Q78] 当前时间
来源：http://hz.dashuyun.cn/gtlfgldekz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuanzx.com/gteshwhoie.html

[Q79] 字符串拼接
来源：http://hz.mhx1999.top/gtanlnufah.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gtyslxuuqe.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtcgjkredl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtvhnjpesw.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtadxvzsvi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgfzy.top/gtgshxytri.html

[Q82] 字符长度与字节长度
来源：http://hz.xuanzx.com/gturgfblay.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydjk.org.cn/gtqazqixqh.html

[Q83] 大小写转换
来源：http://hz.xuanzx.com/gtmlhygkkb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gaohongyu789.top/gtshltokil.html

[Q84] 去除首尾空格
来源：http://hz.316326.xyz/gtduriybbf.html

SELECT TRIM(name) FROM users;
来源：http://hz.quarkkingdee.top/gtoomegwtn.html

[Q85] 数值取整
来源：http://hz.yj20258.top/gtkuvmpmyc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gturkeicvq.html

[Q86] 读取 JSON 字段
来源：http://hz.0kj1m.cn/gtgwdcwiho.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yonumen.top/gtoyghwqwp.html

[Q87] JSON 字段做条件
来源：http://hz.chenlongwang.top/gtaqjtcrqy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hysaishi.cn/gtsjsgtnem.html

[Q88] 行转列（条件聚合）
来源：http://hz.hywenlv.cn/gtxnxplsdm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydzc1.top/gtvzhmjbju.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.redwolf501.top/gtrznuklkl.html

[Q89] 判断表是否存在
来源：http://hz.chenzaomai.com/gtywdidpyh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yongpay.top/gtjjzgzvwu.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangtech.top/gtwafjwgfx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pycfn.com/gteshbtrfm.html

================================================================================
来源：http://hz.jyoumei.cn/gtgkabvzib.html

R. Bash 专题
来源：http://hz.jqgufenzy.top/gtcsomnkcx.html

================================================================================
来源：http://hz.ehwqpu.com/gtjjffvqky.html

[R01] shebang 与严格模式
来源：http://hz.jyoumei.cn/gtybaslwok.html

#!/usr/bin/env bash
来源：http://hz.316326.xyz/gtdqaycugx.html

set -euo pipefail
来源：http://hz.cdnleiting.top/gthbdesxmd.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gtxkackomj.html

name="Tom"; echo "$name"
来源：http://hz.ybcxt.top/gtfecbmbsy.html

[R03] 只读变量
来源：http://hz.sxryk.cn/gtxhcqysvn.html

readonly PI=3.14
来源：http://hz.jinqigufen.top/gtlqxjtybl.html

[R04] 位置参数
来源：http://hz.ehwqpu.com/gtcuydohbx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtutwjxpkh.html

[R05] 参数默认值
来源：http://hz.cdnleiting.top/gtkwmlynvc.html

name="${1:-default}"
来源：http://hz.316326.xyz/gtlfebnpyk.html

[R06] 判断命令是否存在
来源：http://hz.tanke756.top/gtbhcxkrgr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtflktdjlf.html

[R07] if 判断文件
来源：http://hz.feifeiyinyue.top/gttnktvmaa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ywan-chungtsiang.top/gtqodzvgbj.html

[R08] 数值比较
来源：http://hz.chenlongwang.top/gtrzzukrxk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtohnvbovg.html

[R09] 字符串比较
来源：http://hz.shuidangran.top/gtzmihhwal.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cashguo.top/gtyggkcnkc.html

[R10] 正则匹配
来源：http://hz.nanxuanxn.top/gtatbcslbn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtivvywszh.html

[R11] case 多分支
来源：http://hz.jyoumei.cn/gtxlyowbma.html

case "$1" in
来源：http://hz.yanxiufei.cn/gthwsblfbb.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gtdmuwsopk.html

stop)  echo "停止" ;;
来源：http://hz.zycfv.cn/gtnfevacih.html

*)     echo "未知命令" ;;
来源：http://hz.tian-w.cn/gtigzokxab.html

esac
来源：http://hz.jinqigufen.top/gtzqfhlgme.html

[R12] for 遍历文件
来源：http://hz.tian-w.cn/gtfetahfgg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jyoumei.cn/gtefjvopqq.html

[R13] for 计数循环
来源：http://hz.jyoumei.cn/gtqtckdyay.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hywenlv.cn/gtahdroswh.html

[R14] C 风格 for
来源：http://hz.redwolf501.top/gtvkdhzuxx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gtoykzalhx.html

[R15] while 逐行读文件
来源：http://hz.yj20258888.top/gtasnzeurb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shuidangran.top/gtbllhrxwy.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtqdfbtlkr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtrjmaciwc.html

[R17] 数组定义与取值
来源：http://hz.bjfxy.top/gtpnfznqyu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.vqdsnc.cn/gtnoorcvgi.html

[R18] 遍历数组
来源：http://hz.c1oappe.top/gthavftigo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtqfmlcbom.html

[R19] 数组长度
来源：http://hz.yj202588.top/gtkjygusjz.html

echo "${#arr[@]}"
来源：http://hz.dashuyun.cn/gtgxjjjitm.html

[R20] 关联数组（字典）
来源：http://hz.ydzc1.top/gtgrjwklqv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtrfwdclzw.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtejdfehyv.html

echo "${#s}"
来源：http://hz.nanxuanxn.top/gtarxycewx.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gtdwdptqbw.html

echo "${s:0:5}"
来源：http://hz.jinqigfzy.top/gtlokcnmzb.html

[R23] 字符串替换
来源：http://hz.andypj.xyz/gtlerlmlop.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuanzhike.top/gtcuvjynbt.html

[R24] 大小写转换
来源：http://hz.ydjk.org.cn/gtmzucivhk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.feifeiyinyue.top/gtnkhrbxfw.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinyuanbaomall.cn/gtgsuxovva.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gtzmumuojk.html

[R26] 命令替换
来源：http://hz.52xcode.cn/gtqzrxcgfg.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gtmufvbfkq.html

[R27] 算术展开
来源：http://hz.daria6918.cn/gtwsgjvavh.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangkeji.top/gtzyyfpvyb.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtklfnrscs.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhengqikj.top/gtdfjwhqfc.html

[R29] 定义函数
来源：http://hz.hnqzz.top/gtphxpoore.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yueranfly.top/gtwaikmivg.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtpwzlgjfl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hongshengwenyu.top/gtozlvfrdk.html

[R31] 局部变量
来源：http://hz.zhaomingkeji.xyz/gtgsjiqqbe.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhixingplan.top/gtbhnvhhjd.html

[R32] 参数个数校验
来源：http://hz.wangdashe.top/gtlgxidfrd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtbuodznwk.html

[R33] 捕获错误并提示行号
来源：http://hz.daria6918.cn/gttdagdcdf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hywenlv.cn/gtabhanmxs.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gtjrhpybvf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gttsvutmwb.html

[R35] 后台执行并等待
来源：http://hz.jiagoushi.top/gtjcublxpd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangkeji.top/gtxdfavkcy.html

[R36] 并发执行多个任务
来源：http://hz.ywan-chungtsiang.top/gttbmnhokd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guannengcc.top/gthiiiskvu.html

[R37] 把输出赋给变量
来源：http://hz.redwolf501.top/gtmshwhqeb.html

files=$(ls -1)
来源：http://hz.hammf.cn/gtkrzqlfbs.html

[R38] 管道串联
来源：http://hz.nanxinkj.top/gtkcxyzeww.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xingfuxueyuan.xyz/gthaxomfiq.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangtech.top/gtnofhwmwy.html

cmd > out.log 2>&1
来源：http://hz.jqgufenzy.top/gtbkzbfcup.html

[R40] 追加写日志
来源：http://hz.dashuyun.cn/gtdfbmsdog.html

echo "log" >> out.log
来源：http://hz.yvedp.cn/gticdmykoz.html

[R41] 丢弃输出
来源：http://hz.tianlin.xyz/gtkfrygzyl.html

cmd >/dev/null 2>&1
来源：http://hz.yangfankeji.com/gtybesqhfm.html

[R42] 输入重定向
来源：http://hz.shanyushiyangtech.top/gtrmiobstn.html

wc -l < a.txt
来源：http://hz.ehwqpu.com/gtvxrpkzwr.html

[R43] 按名字查找文件
来源：http://hz.jinqigfzy.top/gtzgetfnxe.html


<!-- 参考信息 -->