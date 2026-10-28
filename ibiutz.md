代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pengpengdd.cyou/gtmumcmpjd.html

);
来源：http://hz.chenzaomai.com/gtynjxxexg.html

[Q02] 创建带外键的表
来源：http://hz.cucudq.cn/gthoizwyzg.html

CREATE TABLE orders (
来源：http://hz.ppjwa.cn/gtdwkozjhv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtppypcgnw.html

user_id INT NOT NULL,
来源：http://hz.hfpthk.cn/gtcywsmszn.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gtoywmbiiy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtcbchefda.html

);
来源：http://hz.yueranfly.top/gtgpofapov.html

[Q03] 增加列
来源：http://hz.kuanghao11.cn/gtsblwyzvf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtybcpwjuf.html

[Q04] 修改列类型
来源：http://hz.jinghuilouyu.cn/gtfeqwttrr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fengsongda.top/gtzcpnzxno.html

[Q05] 重命名列
来源：http://hz.nanxinkj.top/gtiotqksoo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cashguo.top/gthumzwevm.html

[Q06] 删除列
来源：http://hz.ydzc1.top/gtiuiyknyk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.birdmap.top/gtyvmkqqni.html

[Q07] 删除表
来源：http://hz.jqgfzy.top/gtvrgpcvgz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guowangkeji.top/gtcnrssdja.html

[Q08] 创建普通索引
来源：http://hz.zhiwuduotai.top/gtobamvujy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtktkxsvms.html

[Q09] 创建唯一索引
来源：http://hz.xinyue.icu/gtsjxzdjya.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuxming.cn/gtwhqgeopr.html

[Q10] 插入单行
来源：http://hz.tian-w.cn/gtmrllghzn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhijiandao.cn/gtenzhwymy.html

[Q11] 一次插入多行
来源：http://hz.jinghuilouyu.cn/gtjfizqocl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.redwolf501.top/gtjoyrqfkz.html

[Q12] 插入后取自增 ID
来源：http://hz.xuanzx.com/gtzhhqvgvo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigfzy.top/gtvtsbjywo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhongyouzk.top/gtpsokizic.html

[Q13] 忽略重复插入
来源：http://hz.wangdashe.top/gtzhdkwioj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xinyue.icu/gtsgpbsrot.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinghuilouyu.cn/gtjdeebcwh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fzhhl.top/gtlzifeqwb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258888.top/gtjajzfhou.html

[Q15] 查询全部
来源：http://hz.haohaochexian.top/gtmggboztz.html

SELECT * FROM users;
来源：http://hz.hfpthk.cn/gtydnykmrb.html

[Q16] 查询指定列
来源：http://hz.pengpengdd.cyou/gtwwqaponf.html

SELECT id, name FROM users;
来源：http://hz.jinqigfzy.top/gtbuxsqvkt.html

[Q17] 条件查询
来源：http://hz.cdnleiting.top/gtxqkywejw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jianghu66.top/gtjaqfnijs.html

[Q18] 模糊匹配
来源：http://hz.quarkkingdee.top/gtiqrzinhg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.meibo888.top/gtjutarlqx.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gtfzqdybcp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daria6918.cn/gtreziargf.html

[Q20] IN 列表
来源：http://hz.zhaomingkeji.xyz/gtakqrrafe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtslaclnpt.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtbbantvih.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhiwuduotai.top/gtriepsffx.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gtbksyzolz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gtygdbnebg.html

[Q23] 分页
来源：http://hz.aizwys.cn/gtwtpzqfmq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ehwqpu.com/gtaxscmtlg.html

[Q24] 去重
来源：http://hz.xuanzx.com/gtufbprtsd.html

SELECT DISTINCT city FROM users;
来源：http://hz.daxiang520.top/gtkofzojfu.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gthogyxros.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenzaomai.com/gtzspegkps.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gtoqpqjylq.html

SELECT COUNT(*) FROM users;
来源：http://hz.gogol.net.cn/gtzecwszuz.html

[Q27] 条件计数
来源：http://hz.tianlin.xyz/gtqcmqgrad.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuxming.cn/gtiszqbjqv.html

[Q28] 求和与平均
来源：http://hz.tanke756.top/gtjevfggxm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tian-w.cn/gtsornwqjg.html

[Q29] 最大最小值
来源：http://hz.daria6918.cn/gtacupshta.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daxiang520.top/gttcusjloo.html

[Q30] 分组统计
来源：http://hz.pengpengdd.cyou/gtybbenudm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtnuhfmwlc.html

[Q31] 分组后过滤
来源：http://hz.feifeiyinyue.top/gthkkfymuf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.nwbrower.top/gteknvmcqe.html

[Q32] 分组拼接字符串
来源：http://hz.pycfn.com/gtqluymtba.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtafzskpzz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.bjfxy.top/gtpdctkodp.html

[Q33] 多列分组
来源：http://hz.iojbl.cn/gtymcehcnv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258888.top/gtthchwjki.html

[Q34] 每组取第一条
来源：http://hz.jyoumei.cn/gtgfxrifkp.html

SELECT * FROM (
来源：http://hz.dianchejie.cn/gtdzwzsbak.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.meibo888.top/gtsponjnmf.html

) t WHERE rn = 1;
来源：http://hz.hnqzz.top/gtywkarydh.html

[Q35] 内连接
来源：http://hz.gotoacloud.top/gtqfjwnilp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cheryme.top/gtcnowvmad.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtktdrrbsp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtmoypzzje.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtecngzuej.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tianlin.xyz/gtuntjovyg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.iojbl.cn/gtayydcjym.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuanzhike.top/gtpzteexjm.html

[Q39] 自连接（查上下级）
来源：http://hz.andypj.xyz/gtsquseubs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yueranfly.top/gtspjygbns.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuetiantiany.cn/gtfefdmrbs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gtpytqmgfg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigufen.top/gtdvnmpjdp.html

[Q41] 多表连接
来源：http://hz.yuanzhike.top/gtiiocradd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj20258888.top/gtkzfbtutv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigfzy.top/gtdxblvwko.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yvedp.cn/gtjmfvdamq.html

[Q42] 连接条件附加过滤
来源：http://hz.ydjk.org.cn/gtnyqodgqn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xuetiantiany.cn/gtixldffuk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtxhbysbas.html

[Q43] 标量子查询
来源：http://hz.xinyue.icu/gtwejyhbpv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ywan-chungtsiang.top/gtwvbvshwl.html

[Q44] IN 子查询
来源：http://hz.jianghu66.top/gtpmpdvkzx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.quarkkingdee.top/gtkcpyljyh.html

[Q45] EXISTS 判断存在
来源：http://hz.dashuyun.cn/gtsvsizryj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ybcxt.top/gtqccvncgu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cheryme.top/gtadnivotd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daria6918.cn/gtgryzkcpc.html

[Q47] 与平均值比较
来源：http://hz.sufxvd.cn/gtjkgzbsjl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yuanzhike.top/gtqgctladx.html

[Q48] CTE 公用表表达式
来源：http://hz.yvedp.cn/gtfbkplnsn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daxiang520.top/gtccwlhfsf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.meibo888.top/gtwqmhraji.html

[Q49] 更新单行
来源：http://hz.quarkkingdee.top/gtwfcmaumv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sxryk.cn/gtnlqmtmyc.html

[Q50] 批量更新
来源：http://hz.nwbrower.top/gtoapvbnkw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangshuangyany.cn/gtbiskwual.html

[Q51] 用子查询更新
来源：http://hz.ehwqpu.com/gtdumpyvoq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhiwuduotai.top/gtojcnswje.html

[Q52] 删除指定行
来源：http://hz.iojbl.cn/gtayadwuqa.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jiagoushi.top/gtvcudxccv.html

[Q53] 按条件删除
来源：http://hz.jinghuilouyu.cn/gtuiiwzqba.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.wangdashe.top/gtxdwvnxnl.html

[Q54] 清空表
来源：http://hz.tanke756.top/gtbqponcfq.html

TRUNCATE TABLE logs;
来源：http://hz.gzhubu.top/gtcknbgona.html

[Q55] 排名（并列占位）
来源：http://hz.birdmap.top/gtkqrhefse.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258888.top/gttqshvwtb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.meibo888.top/gtmfgtmnmu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ppjwa.cn/gtetmvlenu.html

[Q57] 行号
来源：http://hz.yuanzhike.top/gtqebvpuyn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhaomingkeji.xyz/gtypjwhklo.html

[Q58] 累计求和
来源：http://hz.tianlin.xyz/gtllbwuxle.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtfxlgarzr.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtmtuboxdy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ppjwa.cn/gtpyhawmud.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhaomingkeji.xyz/gtqxwwmaap.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cdnleiting.top/gtnzsqhbwv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.vqdsnc.cn/gtkfxzdszz.html

[Q61] 移动平均
来源：http://hz.yonumen.top/gtzokebizh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.quarkkingdee.top/gtmxueiwol.html

[Q62] 分组占比
来源：http://hz.ppjwa.cn/gtjbnajgcl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtwmfiyxyh.html

[Q63] 开启事务
来源：http://hz.zhongyouzk.top/gtzpmddsta.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtekqniavw.html

[Q64] 提交事务
来源：http://hz.hammf.cn/gtfxzxynwf.html

COMMIT;
来源：http://hz.andypj.xyz/gtkfhmqttj.html

[Q65] 回滚事务
来源：http://hz.gotoacloud.top/gtnlzivofd.html

ROLLBACK;
来源：http://hz.chenzaomai.com/gtbblmdgve.html

[Q66] 行锁查询
来源：http://hz.ywan-chungtsiang.top/gtotawqtfr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jlsjyb.cn/gtdkgvdrck.html

[Q67] 设置隔离级别
来源：http://hz.fengsongda.top/gtxiqlojta.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gtorqhklux.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtlqxcgitl.html

SAVEPOINT sp1;
来源：http://hz.haohaochexian.top/gtnxcjggbi.html

ROLLBACK TO sp1;
来源：http://hz.jyoumei.cn/gtvnnkulbs.html

[Q69] 查看执行计划
来源：http://hz.ppjwa.cn/gtoxyljsei.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgfzy.top/gtgqymefya.html

[Q70] 更新统计信息
来源：http://hz.yonumen.top/gtxsmsdtms.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtjhnzdrev.html

[Q71] 查看建表语句
来源：http://hz.guannengcc.top/gtdoqctkxj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gttlwjecgf.html

[Q72] 查看索引
来源：http://hz.xuetiantiany.cn/gtgvuopwhu.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtqwrevqoi.html

[Q73] 查看表状态
来源：http://hz.jinyuanbaomall.cn/gthubqdjmc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuanzhike.top/gtktmxjbre.html

[Q74] 强制使用索引
来源：http://hz.jianghu66.top/gtcidgqkin.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gtrgzlwqsj.html

[Q75] 日期格式化
来源：http://hz.316326.xyz/gtdhrfjwyn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtjcbljobq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yvedp.cn/gtibqnacjr.html

[Q76] 按天统计
来源：http://hz.birdmap.top/gtezyxzhdz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.9152youxi.cn/gtzdyhsnuw.html

[Q77] 时间加减
来源：http://hz.zhaomingkeji.xyz/gtvdscwgnq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yonumen.top/gtconouatk.html

[Q78] 当前时间
来源：http://hz.zhijiandao.cn/gtyewjzlcn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigufen.top/gtpcvhgmgi.html

[Q79] 字符串拼接
来源：http://hz.aizwys.cn/gtepmegmck.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtpojlteuy.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangkeji.top/gtbnbsvmiu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gtllhkrrgd.html

[Q81] 字符串替换
来源：http://hz.andypj.xyz/gtbfheycvz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtaogffkxl.html

[Q82] 字符长度与字节长度
来源：http://hz.zhijiandao.cn/gtnzqfrygw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtxobuwmfo.html

[Q83] 大小写转换
来源：http://hz.pycfn.com/gtelwcgbnk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtrzetfyzs.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtzarkbkqq.html

SELECT TRIM(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtmfviszqx.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gticouhusb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jiagoushi.top/gtiefbibaa.html

[Q86] 读取 JSON 字段
来源：http://hz.gotoacloud.top/gtnxqahsdd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sxryk.cn/gthopmwnmb.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gthswfkwvu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dianchejie.cn/gtjybsugsq.html

[Q88] 行转列（条件聚合）
来源：http://hz.daria6918.cn/gtyvbaqgmb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangkeji.top/gtnmhirbzk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.birdmap.top/gtyegeqxzj.html

[Q89] 判断表是否存在
来源：http://hz.0kj1m.cn/gtzpppgquo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydzc1.top/gtzwpvkguo.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtxwievgdo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenlongwang.top/gtundfrwit.html

================================================================================
来源：http://hz.chenlongwang.top/gtqtdcnpwg.html

R. Bash 专题
来源：http://hz.gogol.net.cn/gtqegqajek.html

================================================================================
来源：http://hz.yuxming.cn/gtpezllnsd.html

[R01] shebang 与严格模式
来源：http://hz.jyoumei.cn/gtkwmxkvgp.html

#!/usr/bin/env bash
来源：http://hz.birdmap.top/gtuyrxzkjx.html

set -euo pipefail
来源：http://hz.yj20258.top/gtovcluczt.html

[R02] 变量赋值与使用
来源：http://hz.316326.xyz/gtppkeseba.html

name="Tom"; echo "$name"
来源：http://hz.zhiwuduotai.top/gtjvfpgzgq.html

[R03] 只读变量
来源：http://hz.hfpthk.cn/gtsauvkqzz.html

readonly PI=3.14
来源：http://hz.hfpthk.cn/gtqznzlnfl.html

[R04] 位置参数
来源：http://hz.cheryme.top/gtdifetsqt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xylfe.cn/gttxzwawdc.html

[R05] 参数默认值
来源：http://hz.tian-w.cn/gtenbogkak.html

name="${1:-default}"
来源：http://hz.aibaodan.cn/gtotvnbijn.html

[R06] 判断命令是否存在
来源：http://hz.snrcjt.cn/gtfvghudgv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgfzy.top/gtxksjeakv.html

[R07] if 判断文件
来源：http://hz.aizwys.cn/gtacbizgjs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tanke756.top/gtdmhdatza.html

[R08] 数值比较
来源：http://hz.yanxiufei.cn/gtyjsixuvf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtznoxycnm.html

[R09] 字符串比较
来源：http://hz.zhoulong.xyz/gtbdnclmxz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigufen.top/gtscfqfyul.html

[R10] 正则匹配
来源：http://hz.hammf.cn/gtcrbtdhne.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtseipglbc.html

[R11] case 多分支
来源：http://hz.9152youxi.cn/gtrljsnsgw.html

case "$1" in
来源：http://hz.chenjidiqi.icu/gteajipzgq.html

start) echo "启动" ;;
来源：http://hz.tanke756.top/gtmcktwmwy.html

stop)  echo "停止" ;;
来源：http://hz.feifeiyinyue.top/gtfwbxlifl.html

*)     echo "未知命令" ;;
来源：http://hz.zhongyouzk.top/gtuenfehzc.html

esac
来源：http://hz.quarkkingdee.top/gtiijahfmb.html

[R12] for 遍历文件
来源：http://hz.sysykeji.top/gtncwwrjoo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhaomingkeji.xyz/gtwsrleioq.html

[R13] for 计数循环
来源：http://hz.guowangkeji.top/gtzbplyivx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtoudcbmex.html

[R14] C 风格 for
来源：http://hz.tanke756.top/gtpkqglvkg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gtylynedph.html

[R15] while 逐行读文件
来源：http://hz.hnqzz.top/gtldgpdvze.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuanzhike.top/gtqifbuwwb.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gteidaouqk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtpvlfhogx.html

[R17] 数组定义与取值
来源：http://hz.sufxvd.cn/gtjojdznlb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gotoacloud.top/gtquiopnec.html

[R18] 遍历数组
来源：http://hz.chenjidiqi.icu/gtnqcugami.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuanzx.com/gtvhxldwyp.html

[R19] 数组长度
来源：http://hz.hywenlv.cn/gtvdycsefv.html

echo "${#arr[@]}"
来源：http://hz.jinghuilouyu.cn/gtnvhwibrl.html

[R20] 关联数组（字典）
来源：http://hz.yonumen.top/gtugjaeoqi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jyoumei.cn/gtxvigiujs.html

[R21] 字符串长度
来源：http://hz.cheryme.top/gtclxgcqbx.html

echo "${#s}"
来源：http://hz.jianghu66.top/gtftwvgxhf.html

[R22] 截取子串
来源：http://hz.yj202588.top/gtzvxpnyqa.html

echo "${s:0:5}"
来源：http://hz.chenzaomai.com/gtnbtggxma.html

[R23] 字符串替换
来源：http://hz.xziqi.cn/gtxoechbsf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxuanxn.top/gtzmygrnbf.html

[R24] 大小写转换
来源：http://hz.redwolf501.top/gtoduizwzw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.wangshuangyany.cn/gtemfjyoga.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258888.top/gttapzebqm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydzc1.top/gtluobvpzd.html

[R26] 命令替换
来源：http://hz.jinghuilouyu.cn/gtsmfjnesc.html

now=$(date +%F); echo "$now"
来源：http://hz.tianlin.xyz/gtdlropgex.html

[R27] 算术展开
来源：http://hz.c1oappe.top/gtomzobbfa.html

echo $((1 + 2 * 3))
来源：http://hz.cqqwz.cn/gtvaacpjgl.html

[R28] 浮点运算
来源：http://hz.yanxiufei.cn/gtmufmtpez.html

echo "scale=2; 10/3" | bc
来源：http://hz.nwbrower.top/gttibxwutq.html

[R29] 定义函数
来源：http://hz.zhijiandao.cn/gtndqvopyr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.kuanghao11.cn/gtzxpsgike.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gtxzezrucg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.9152youxi.cn/gtgnrlhypa.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gtnvnwvfcv.html

f() { local x=1; echo "$x"; }
来源：http://hz.jyoumei.cn/gtcucuyqll.html

[R32] 参数个数校验
来源：http://hz.iojbl.cn/gtypfyqdro.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ehwqpu.com/gthrpdbvfw.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtjvlykitr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangkeji.top/gtzomqcirb.html

[R34] 退出时清理
来源：http://hz.tianlin.xyz/gtlzomcdpb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jyoumei.cn/gtvntyjhel.html

[R35] 后台执行并等待
来源：http://hz.xylfe.cn/gtgyjowgde.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangtech.top/gtjztmsytb.html

[R36] 并发执行多个任务
来源：http://hz.hammf.cn/gtzeecuenl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhengqikj.top/gtkkfnphvk.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtlvfmbioy.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtnipwgqaq.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtkxztzlnz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.svipenyu.cn/gtdwyqmlkq.html

[R39] 重定向标准输出与错误
来源：http://hz.daxiang520.top/gtrjxbvlzl.html

cmd > out.log 2>&1
来源：http://hz.jlsjyb.cn/gtydfcqqas.html

[R40] 追加写日志
来源：http://hz.dashuyun.cn/gtcuacnfig.html

echo "log" >> out.log
来源：http://hz.hongshengwenyu.top/gtqekzospb.html

[R41] 丢弃输出
来源：http://hz.nanxuanxn.top/gtbzkczvrc.html

cmd >/dev/null 2>&1
来源：http://hz.sysykeji.top/gtpjrydroz.html

[R42] 输入重定向
来源：http://hz.yuanzhike.top/gtqqnaewou.html

wc -l < a.txt
来源：http://hz.hfpthk.cn/gtjflwbhmn.html

[R43] 按名字查找文件
来源：http://hz.aizwys.cn/gtalauqbnk.html

find . -name "*.log" -type f
来源：http://hz.nwbrower.top/gtlokazftq.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gttfowvqmp.html

find . -mtime -7 -type f
来源：http://hz.chenlongwang.top/gtobxiwgvq.html

[R45] 批量删除
来源：http://hz.yanxiufei.cn/gtjligvrgp.html

find . -name "*.tmp" -delete
来源：http://hz.redwolf501.top/gtviwtsoof.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangtech.top/gtvxajyxxl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenlongwang.top/gthdbjromu.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gtxpicwepn.html


<!-- 参考信息 -->