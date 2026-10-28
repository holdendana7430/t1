代发 wailian999

CREATE TABLE users (
来源：http://hz.xuetiantiany.cn/gtcjgibxsl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shangyingyoupin.top/gthnsiltjr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dashuyun.cn/gtkfjxnwyn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ybcxt.top/gthxchrelo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhaomingkeji.xyz/gtrlmnngal.html

);
来源：http://hz.ehwqpu.com/gtsumqowfi.html

[Q02] 创建带外键的表
来源：http://hz.guannengcc.top/gtmxiexorb.html

CREATE TABLE orders (
来源：http://hz.xinyue.icu/gtwurropab.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtkwxazygi.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gthayfbpke.html

amount DECIMAL(10, 2),
来源：http://hz.hysaishi.cn/gtzcqacslk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinyuanbaomall.cn/gttoxjdbrh.html

);
来源：http://hz.shuidangran.top/gtzbpsnjuq.html

[Q03] 增加列
来源：http://hz.ydjk.org.cn/gtzakmantz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aibaodan.cn/gthmplawcv.html

[Q04] 修改列类型
来源：http://hz.cucudq.cn/gtfaxipljh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dashuyun.cn/gtctvkwark.html

[Q05] 重命名列
来源：http://hz.zhoulong.xyz/gtlxnhogpa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuxming.cn/gtziclnzft.html

[Q06] 删除列
来源：http://hz.yongpay.top/gtlyjcgbbp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jlsjyb.cn/gtlirsgzzq.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gthbhcszlu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.52xcode.cn/gtdlwwfxlu.html

[Q08] 创建普通索引
来源：http://hz.shangyingyoupin.top/gtcyrtzxjd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ivvv.top/gtjvnlizyu.html

[Q09] 创建唯一索引
来源：http://hz.yuanzhike.top/gtzaenzbfq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtekqsujhx.html

[Q10] 插入单行
来源：http://hz.birdmap.top/gtdszfqdyd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.svipenyu.cn/gtifulwgix.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtxhrabayc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gtcdkrhjup.html

[Q12] 插入后取自增 ID
来源：http://hz.mhx1999.top/gtlryygxgi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenzaomai.com/gtskhbimqh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuanzhike.top/gthrpzhyxc.html

[Q13] 忽略重复插入
来源：http://hz.yj202588.top/gtoeopuklr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258.top/gtoanoxdef.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtmylrddfk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dashuyun.cn/gteodzhwrb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gthdseubbg.html

[Q15] 查询全部
来源：http://hz.sxryk.cn/gtbfuucpob.html

SELECT * FROM users;
来源：http://hz.tianlin.xyz/gtpanzzzje.html

[Q16] 查询指定列
来源：http://hz.jqgfzy.top/gtrmtfjoiv.html

SELECT id, name FROM users;
来源：http://hz.jinghuilouyu.cn/gtxctcmesv.html

[Q17] 条件查询
来源：http://hz.zhaomingkeji.xyz/gtiojdsigk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.haohaochexian.top/gtjnffteqk.html

[Q18] 模糊匹配
来源：http://hz.meibo888.top/gttqbbooht.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hywenlv.cn/gtaassjonh.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtdricpjzc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gtuubwnafd.html

[Q20] IN 列表
来源：http://hz.cdnleiting.top/gtdvmhxosn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hfpthk.cn/gtomjwqwaz.html

[Q21] 空值判断
来源：http://hz.aizwys.cn/gtzdhuzpxs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aibaodan.cn/gtfqagicfa.html

[Q22] 排序
来源：http://hz.quarkkingdee.top/gttcmkqouk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.iojbl.cn/gtjpmuyxtn.html

[Q23] 分页
来源：http://hz.jinyuanbaomall.cn/gtqeegminn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydjk.org.cn/gthvhqmwvi.html

[Q24] 去重
来源：http://hz.yj20258.top/gtypmdxsnk.html

SELECT DISTINCT city FROM users;
来源：http://hz.0kj1m.cn/gtspntxxip.html

[Q25] 只取前 N 条
来源：http://hz.hammf.cn/gtkxbnznzm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ehwqpu.com/gtelolodce.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gtacfkctcl.html

SELECT COUNT(*) FROM users;
来源：http://hz.guannengcc.top/gtrkeokfkx.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtezhbftrw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gzhubu.top/gtpxecpqlx.html

[Q28] 求和与平均
来源：http://hz.shangyingyoupin.top/gtpaqxxbut.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuetiantiany.cn/gtvppcobjo.html

[Q29] 最大最小值
来源：http://hz.yongpay.top/gtsaachedy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnxiangtu.top/gtkdajdmno.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtehrphbhd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtmyjpxnsy.html

[Q31] 分组后过滤
来源：http://hz.fengsongda.top/gtgrqlksts.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gtrdsxwvyk.html

[Q32] 分组拼接字符串
来源：http://hz.snrcjt.cn/gtclakatev.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gttjaposvi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.iojbl.cn/gtcbriwelz.html

[Q33] 多列分组
来源：http://hz.nwbrower.top/gtwltwxkzy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtetsbrkuu.html

[Q34] 每组取第一条
来源：http://hz.zdqjudy.top/gtdvshjddz.html

SELECT * FROM (
来源：http://hz.jinyuanbaomall.cn/gtjsqhacho.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenzaomai.com/gtdmnvyvcf.html

) t WHERE rn = 1;
来源：http://hz.zhengqikj.top/gtsmntiiep.html

[Q35] 内连接
来源：http://hz.yvedp.cn/gtlpjlnodw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtgqaoywmg.html

[Q36] 左连接
来源：http://hz.shanyushiyangkeji.top/gtwkxibfqw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtjuftpypv.html

[Q37] 右连接
来源：http://hz.cashguo.top/gthfipqmfh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hywenlv.cn/gtsxwuhfla.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenjidiqi.icu/gtjatdrfnc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.316326.xyz/gtxebznawy.html

[Q39] 自连接（查上下级）
来源：http://hz.cdnleiting.top/gtopfuzkwq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gtmynmkubv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sweek.top/gtemrdahls.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtcodydyvy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yvedp.cn/gtkeibgftd.html

[Q41] 多表连接
来源：http://hz.meibo888.top/gtjqpdokzb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.andypj.xyz/gtxfsuqqvx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xuanzx.com/gtordhzltv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhiwuduotai.top/gtwqczbodc.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtgfuucglp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhaomingkeji.xyz/gtqdnmfqyd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zycfv.cn/gtqrakijxe.html

[Q43] 标量子查询
来源：http://hz.sufxvd.cn/gtdpmrnrxp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj202588.top/gtvrxvwvvp.html

[Q44] IN 子查询
来源：http://hz.yonumen.top/gtsnacvxds.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.smart0.xyz/gtkpdmspyl.html

[Q45] EXISTS 判断存在
来源：http://hz.chenzaomai.com/gtwgmjyjkk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtfirdoqfs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.daxiang520.top/gtmophwzjg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gtwydfvsrx.html

[Q47] 与平均值比较
来源：http://hz.meibo888.top/gtvgibdnvd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gtjqfmcncx.html

[Q48] CTE 公用表表达式
来源：http://hz.yuxming.cn/gtwpmezito.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tianlin.xyz/gtrnzpifpo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.quarkkingdee.top/gtjdlfryys.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gtlmhclurg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xuanzx.com/gtsmasarub.html

[Q50] 批量更新
来源：http://hz.ywan-chungtsiang.top/gtwqjjdgdp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jianghu66.top/gtqzuxdxzy.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gthwdpidnr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pycfn.com/gtmkjegmgv.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gtsqddtoug.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yangfankeji.com/gtdrscgngg.html

[Q53] 按条件删除
来源：http://hz.yj202588.top/gtcblrouvg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.snrcjt.cn/gtsneyouql.html

[Q54] 清空表
来源：http://hz.cdnleiting.top/gtinalqetk.html

TRUNCATE TABLE logs;
来源：http://hz.yueranfly.top/gtusccpmqx.html

[Q55] 排名（并列占位）
来源：http://hz.aizwys.cn/gtzeniffld.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yonumen.top/gtlgorzyoa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangkeji.top/gtaknmuxtc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nwbrower.top/gtucosotkx.html

[Q57] 行号
来源：http://hz.xuanzx.com/gtsgitxodn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenzaomai.com/gtnalcvpyp.html

[Q58] 累计求和
来源：http://hz.ehwqpu.com/gtgfogcwhe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.svipenyu.cn/gtxzgaruxd.html

[Q59] 分组内累计
来源：http://hz.sweek.top/gtnnnhlqxl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cucudq.cn/gttkqmnzks.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj20258.top/gtwmobeafx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtndkjsbeh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuetiantiany.cn/gtzlgzhoxc.html

[Q61] 移动平均
来源：http://hz.jiagoushi.top/gtenxvidia.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zycfv.cn/gtvegfilhn.html

[Q62] 分组占比
来源：http://hz.jyoumei.cn/gtotibgick.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtpntpvokb.html

[Q63] 开启事务
来源：http://hz.cheryme.top/gtwavjputu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.smart0.xyz/gtlnwiczie.html

[Q64] 提交事务
来源：http://hz.aibaodan.cn/gtbcawwqcm.html

COMMIT;
来源：http://hz.jlsjyb.cn/gtfrrsdgqg.html

[Q65] 回滚事务
来源：http://hz.gzhubu.top/gtyfcwmotk.html

ROLLBACK;
来源：http://hz.tanke756.top/gtkocvsana.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtpsafdfeg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tanke756.top/gtgltxeeem.html

[Q67] 设置隔离级别
来源：http://hz.ybcxt.top/gtzsiwrbjw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenlongwang.top/gtyntmxxzy.html

[Q68] 保存点
来源：http://hz.jiagoushi.top/gtojrrlpfi.html

SAVEPOINT sp1;
来源：http://hz.haohaochexian.top/gtsmnnuwtq.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gtpjhyjagy.html

[Q69] 查看执行计划
来源：http://hz.snrcjt.cn/gtjksvnuyy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shzxlz.cn/gtoctmiplb.html

[Q70] 更新统计信息
来源：http://hz.cucudq.cn/gtorasoviv.html

ANALYZE TABLE users;
来源：http://hz.zhongyouzk.top/gtuqfuolbv.html

[Q71] 查看建表语句
来源：http://hz.cheryme.top/gtamahpcjy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sufxvd.cn/gthfgprchm.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gtnleveewz.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtskgmucwo.html

[Q73] 查看表状态
来源：http://hz.smart0.xyz/gtoixuyzix.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.iojbl.cn/gtyljzpidk.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gtqtcglqic.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ybcxt.top/gtcyneehjy.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtvggmttgq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuetiantiany.cn/gtsxcihnxn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangshuangyany.cn/gtvidbjqid.html

[Q76] 按天统计
来源：http://hz.wangshuangyany.cn/gtpzxhsgxh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gotoacloud.top/gtbskfjdnm.html

[Q77] 时间加减
来源：http://hz.jiagoushi.top/gtjjljolxz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cashguo.top/gtdvuomocf.html

[Q78] 当前时间
来源：http://hz.andypj.xyz/gtlvllttwq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.birdmap.top/gtmabcbmir.html

[Q79] 字符串拼接
来源：http://hz.jyoumei.cn/gtliezzcki.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daria6918.cn/gtywomtkye.html

[Q80] 字符串截取
来源：http://hz.yj202588.top/gtspaeoehx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgfzy.top/gtkncygwsa.html

[Q81] 字符串替换
来源：http://hz.ehwqpu.com/gtguyyqdom.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258.top/gtmqzgakkq.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gttqaqzjdg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtgabkhrvc.html

[Q83] 大小写转换
来源：http://hz.tanke756.top/gtgnybbytp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtvnokjihl.html

[Q84] 去除首尾空格
来源：http://hz.zhixingplan.top/gtslssaccc.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenzaomai.com/gtnlkqkyhc.html

[Q85] 数值取整
来源：http://hz.zycfv.cn/gtuztcmtko.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydjk.org.cn/gtvyupfexv.html

[Q86] 读取 JSON 字段
来源：http://hz.shuidangran.top/gtjkzjxbwo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.c1oappe.top/gtyrkkvnwe.html

[Q87] JSON 字段做条件
来源：http://hz.tanke756.top/gtbdbtpygy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hysaishi.cn/gtybxbuovo.html

[Q88] 行转列（条件聚合）
来源：http://hz.aibaodan.cn/gtxhadkhkb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtotkhlxxk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gthwdtyytr.html

[Q89] 判断表是否存在
来源：http://hz.hammf.cn/gtcjkqmkdf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xylfe.cn/gtpgzvfxci.html

[Q90] 生成序号列
来源：http://hz.guannengcc.top/gtviqzfprq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxinkj.top/gthgeycziw.html

================================================================================
来源：http://hz.ppjwa.cn/gtwmpaiwci.html

R. Bash 专题
来源：http://hz.mhx1999.top/gtnjbetczs.html

================================================================================
来源：http://hz.shuidangran.top/gtrvdmvtai.html

[R01] shebang 与严格模式
来源：http://hz.zhiwuduotai.top/gtxlgwbrvj.html

#!/usr/bin/env bash
来源：http://hz.nanxuanxn.top/gtupntvyqu.html

set -euo pipefail
来源：http://hz.zhijiandao.cn/gttklaolys.html

[R02] 变量赋值与使用
来源：http://hz.52xcode.cn/gtvxrzhclj.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtowmtmytz.html

[R03] 只读变量
来源：http://hz.hammf.cn/gteckwgvwt.html

readonly PI=3.14
来源：http://hz.hammf.cn/gtlydpsxyv.html

[R04] 位置参数
来源：http://hz.jqgfzy.top/gtkbzjanyy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.iojbl.cn/gttooyeorc.html

[R05] 参数默认值
来源：http://hz.yuanzhike.top/gtctvdfasu.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtamyskdnt.html

[R06] 判断命令是否存在
来源：http://hz.yvedp.cn/gtqpjmnsme.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gtrbcxjgsz.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtagczgytk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tianlin.xyz/gtglayhrhn.html

[R08] 数值比较
来源：http://hz.yj202588.top/gtvfoszbpt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hysaishi.cn/gtfkohgsiv.html

[R09] 字符串比较
来源：http://hz.0kj1m.cn/gttmicigqu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jiagoushi.top/gtofpgkksc.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtwyejtdvo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhiwuduotai.top/gtismeomzq.html

[R11] case 多分支
来源：http://hz.sysykeji.top/gtsgbaizur.html

case "$1" in
来源：http://hz.meibo888.top/gtekomcunq.html

start) echo "启动" ;;
来源：http://hz.zhaomingkeji.xyz/gtuserlmlw.html

stop)  echo "停止" ;;
来源：http://hz.pengpengdd.cyou/gtgierwhyr.html

*)     echo "未知命令" ;;
来源：http://hz.yuxming.cn/gtncodorts.html

esac
来源：http://hz.gzhubu.top/gtbgnxkgvd.html

[R12] for 遍历文件
来源：http://hz.zycfv.cn/gtykuhisth.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gtmhrlixhe.html

[R13] for 计数循环
来源：http://hz.shzxlz.cn/gthhlpvgye.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.mhx1999.top/gtjjremqpx.html

[R14] C 风格 for
来源：http://hz.cheryme.top/gtenqmaidc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtslmviaxu.html

[R15] while 逐行读文件
来源：http://hz.nanxuanxn.top/gtazvzshkc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.mhx1999.top/gtmkrkpdrq.html

[R16] until 等待条件
来源：http://hz.jianghu66.top/gtdvlklgjl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.smart0.xyz/gtbaxggtvb.html

[R17] 数组定义与取值
来源：http://hz.gotoacloud.top/gtkhbrzohl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.svipenyu.cn/gtlglxlwqt.html

[R18] 遍历数组
来源：http://hz.ywan-chungtsiang.top/gtnampupbs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gtitkjeqly.html

[R19] 数组长度
来源：http://hz.jinqigufen.top/gtumvtbtyz.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtcqyfiaml.html

[R20] 关联数组（字典）
来源：http://hz.mhx1999.top/gtryxbdewk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shzxlz.cn/gtcddpczss.html

[R21] 字符串长度
来源：http://hz.jinyuanbaomall.cn/gtlmyiypmz.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gtcvrgdakz.html

[R22] 截取子串
来源：http://hz.birdmap.top/gtznbiknkz.html

echo "${s:0:5}"
来源：http://hz.kuanghao11.cn/gtqtucvjil.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtnpkbixdb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gteeuygwwb.html

[R24] 大小写转换
来源：http://hz.cdnleiting.top/gtxsmrjvbb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daria6918.cn/gtawlynkhr.html

[R25] 去后缀 / 去前缀
来源：http://hz.xylfe.cn/gtgkychujm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.c1oappe.top/gtttztbwfd.html

[R26] 命令替换
来源：http://hz.nanxinkj.top/gtevhhgzwq.html

now=$(date +%F); echo "$now"
来源：http://hz.zhijiandao.cn/gtvfxiczmh.html

[R27] 算术展开
来源：http://hz.yongpay.top/gtfdcpmpgv.html

echo $((1 + 2 * 3))
来源：http://hz.daxiang520.top/gtausxdqrs.html

[R28] 浮点运算
来源：http://hz.mhx1999.top/gthazlhoto.html

echo "scale=2; 10/3" | bc
来源：http://hz.cheryme.top/gtoesvvvvd.html

[R29] 定义函数
来源：http://hz.ydjk.org.cn/gtszuycvrb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigfzy.top/gtiheminbv.html

[R30] 函数返回状态码
来源：http://hz.jinqigufen.top/gtwbotsazr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gtmqkmugrw.html

[R31] 局部变量
来源：http://hz.ydjk.org.cn/gtlszbkwyy.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxinkj.top/gtiwfxobqx.html

[R32] 参数个数校验
来源：http://hz.wangdashe.top/gtxkphpfip.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtyegtcpph.html

[R33] 捕获错误并提示行号
来源：http://hz.chenzaomai.com/gtcitrtwrr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhongyouzk.top/gtkiscjpix.html

[R34] 退出时清理
来源：http://hz.ywan-chungtsiang.top/gtwuhimndp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtoyuwrxqm.html

[R35] 后台执行并等待
来源：http://hz.jlsjyb.cn/gtodnqlvae.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigfzy.top/gtendlottz.html

[R36] 并发执行多个任务
来源：http://hz.zhaomingkeji.xyz/gtjhqiuunb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gttxcyuwom.html

[R37] 把输出赋给变量
来源：http://hz.zhaomingkeji.xyz/gtfyiazgtr.html

files=$(ls -1)
来源：http://hz.jinyuanbaomall.cn/gtgmapgtof.html

[R38] 管道串联
来源：http://hz.smart0.xyz/gttqtjpvie.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dianchejie.cn/gtxhiserub.html

[R39] 重定向标准输出与错误
来源：http://hz.hywenlv.cn/gtrfzbrqrp.html

cmd > out.log 2>&1
来源：http://hz.zhaomingkeji.xyz/gtzlteykzn.html

[R40] 追加写日志
来源：http://hz.aizwys.cn/gtxctfpkjc.html

echo "log" >> out.log
来源：http://hz.zhiwuduotai.top/gtawcshtif.html

[R41] 丢弃输出
来源：http://hz.ydjk.org.cn/gtksaftbro.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtglvihbpk.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gtfezdemnr.html

wc -l < a.txt
来源：http://hz.sxryk.cn/gtnskgsgid.html

[R43] 按名字查找文件
来源：http://hz.zhaomingkeji.xyz/gteivuhhgh.html

find . -name "*.log" -type f
来源：http://hz.ehwqpu.com/gthoezlejq.html

[R44] 按修改时间查找
来源：http://hz.yanxiufei.cn/gtgxwwtykr.html

find . -mtime -7 -type f
来源：http://hz.jlsjyb.cn/gtmcrtmjer.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gtfmyxrqqj.html


<!-- 参考信息 -->