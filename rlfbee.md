代发 wailian999

CREATE TABLE users (
来源：http://hz.hammf.cn/gtcginexdm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinyuanbaomall.cn/gtabzghoaf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shuidangran.top/gtsmyqsikg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shanyushiyangtech.top/gtkkrvmmwo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pycfn.com/gtinexussn.html

);
来源：http://hz.dashuyun.cn/gtrhsdzqjf.html

[Q02] 创建带外键的表
来源：http://hz.zhijiandao.cn/gtcbnktapk.html

CREATE TABLE orders (
来源：http://hz.ehwqpu.com/gtngquzopr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtlydhqaam.html

user_id INT NOT NULL,
来源：http://hz.ybcxt.top/gtbbydkqdn.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gtpvzedrbz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtqjgpqbsf.html

);
来源：http://hz.sxryk.cn/gtgberjuxx.html

[Q03] 增加列
来源：http://hz.aibaodan.cn/gtdektmmux.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangtech.top/gtbbieqdjb.html

[Q04] 修改列类型
来源：http://hz.haohaochexian.top/gtnzkbqbwj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgfzy.top/gtsuqkjbxh.html

[Q05] 重命名列
来源：http://hz.yj20258888.top/gtczkipwar.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hongshengwenyu.top/gtmjcmtuob.html

[Q06] 删除列
来源：http://hz.svipenyu.cn/gtgcugolrf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hfpthk.cn/gtwaaefqag.html

[Q07] 删除表
来源：http://hz.nwbrower.top/gtkzmdifzb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cqqwz.cn/gtgyxtpuio.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtupkzwzym.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yongpay.top/gtzeeejmnk.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gtlcrsvozs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuxming.cn/gtojxgiywr.html

[Q10] 插入单行
来源：http://hz.cqqwz.cn/gtntzuhwmi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ybcxt.top/gtimuhjnlj.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtoqdilwmc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cqqwz.cn/gtskverwar.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258.top/gtpxxbtvxs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ppjwa.cn/gtipkyvhie.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cashguo.top/gtkfouulul.html

[Q13] 忽略重复插入
来源：http://hz.wangdashe.top/gtxmxodsbf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtvtykxirr.html

[Q14] 存在则更新（upsert）
来源：http://hz.shangyingyoupin.top/gtnzypeziv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hysaishi.cn/gtxgbidkce.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.9152youxi.cn/gtjkkwwsii.html

[Q15] 查询全部
来源：http://hz.yonumen.top/gtzfxjcabh.html

SELECT * FROM users;
来源：http://hz.quarkkingdee.top/gtwgkilhsk.html

[Q16] 查询指定列
来源：http://hz.chenlongwang.top/gtcxryehpd.html

SELECT id, name FROM users;
来源：http://hz.jlsjyb.cn/gtggrwepht.html

[Q17] 条件查询
来源：http://hz.chenzaomai.com/gtrphsrlxs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtcoypxrvv.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtnwdjkihc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtqodtadvx.html

[Q19] 范围查询
来源：http://hz.shzxlz.cn/gtlrmwkgxp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenzaomai.com/gtichodaxr.html

[Q20] IN 列表
来源：http://hz.ybcxt.top/gtdddccske.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nanxuanxn.top/gtyrysxcnv.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtohiqdydp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aizwys.cn/gtiqfptjvo.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtcezdpbam.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhijiandao.cn/gtexlrlsyi.html

[Q23] 分页
来源：http://hz.nanxinkj.top/gtkbhhwnvl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.9152youxi.cn/gteskykljm.html

[Q24] 去重
来源：http://hz.yuxming.cn/gtyemkdznj.html

SELECT DISTINCT city FROM users;
来源：http://hz.52xcode.cn/gtyuslhfcj.html

[Q25] 只取前 N 条
来源：http://hz.andypj.xyz/gtzanmpjmd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aizwys.cn/gtjdghmywm.html

[Q26] 计数
来源：http://hz.yuxming.cn/gtetmtknun.html

SELECT COUNT(*) FROM users;
来源：http://hz.snrcjt.cn/gtgedxojie.html

[Q27] 条件计数
来源：http://hz.ydzc1.top/gtzlxupkzk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.52xcode.cn/gtxpgmkmum.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtypswrwld.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.316326.xyz/gtdavafyko.html

[Q29] 最大最小值
来源：http://hz.jqgufenzy.top/gtqoylhlvz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daxiang520.top/gtftpmysnv.html

[Q30] 分组统计
来源：http://hz.zycfv.cn/gtmoouqfxw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gthmbwnymm.html

[Q31] 分组后过滤
来源：http://hz.ybcxt.top/gttgughfxe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenlongwang.top/gtyvvcjmqy.html

[Q32] 分组拼接字符串
来源：http://hz.kuanghao11.cn/gtqkqzrnax.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtvlapeuou.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aibaodan.cn/gtsfrzxlac.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtvtcelbbi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.andypj.xyz/gtbksmbkce.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtwndizsnq.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gtatbgdagl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydjk.org.cn/gtaijzoywq.html

) t WHERE rn = 1;
来源：http://hz.xuetiantiany.cn/gtlmyuzjnc.html

[Q35] 内连接
来源：http://hz.havefunace.top/gtimazyrxc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtrsrzupau.html

[Q36] 左连接
来源：http://hz.chenzaomai.com/gtdnzdzupz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtqpaoduou.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtkzenpkzp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tanke756.top/gtyslatuwz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daxiang520.top/gtjbtvmgrv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.redwolf501.top/gtzspkskkp.html

[Q39] 自连接（查上下级）
来源：http://hz.ehwqpu.com/gtnpfvanfy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yueranfly.top/gtnndjxowu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgfzy.top/gtzirkwtuf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fzhhl.top/gtsycmbvbc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hfpthk.cn/gtjmhofouv.html

[Q41] 多表连接
来源：http://hz.zhiwuduotai.top/gtheanftdj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pycfn.com/gtenudxitg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.quarkkingdee.top/gtbhmlmykt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aizwys.cn/gtdfjkbbgr.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgufenzy.top/gtzwgahphx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pengpengdd.cyou/gtebcviicz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenjidiqi.icu/gtcuxavxyc.html

[Q43] 标量子查询
来源：http://hz.cdnleiting.top/gtsknsoojg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhixingplan.top/gtgzcyqpiy.html

[Q44] IN 子查询
来源：http://hz.yongpay.top/gtsgjzlste.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cucudq.cn/gtetwhoazj.html

[Q45] EXISTS 判断存在
来源：http://hz.ywan-chungtsiang.top/gtffadicjr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtaogntpms.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xylfe.cn/gttegvyptc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtwhyevotj.html

[Q47] 与平均值比较
来源：http://hz.cheryme.top/gtvnblnfds.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtcwoabgiy.html

[Q48] CTE 公用表表达式
来源：http://hz.zdqjudy.top/gtfgeskebc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangkeji.top/gtkgvhhkqr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenjidiqi.icu/gtpditbuqu.html

[Q49] 更新单行
来源：http://hz.jqgfzy.top/gtsetnrogs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ppjwa.cn/gtowzuhkik.html

[Q50] 批量更新
来源：http://hz.snrcjt.cn/gtpqhfzjry.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258.top/gtogsjfpfg.html

[Q51] 用子查询更新
来源：http://hz.shanyushiyangkeji.top/gtkbdwfidr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xingfuxueyuan.xyz/gttipnnzbb.html

[Q52] 删除指定行
来源：http://hz.9152youxi.cn/gtyxghwmgf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhengqikj.top/gtsqaxaehl.html

[Q53] 按条件删除
来源：http://hz.yonumen.top/gtninmhphu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tianlin.xyz/gtblyibplk.html

[Q54] 清空表
来源：http://hz.cqqwz.cn/gtejfpbpmm.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtlostepqw.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtquvgmbcu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sufxvd.cn/gtfjayhmgi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jyoumei.cn/gtlmybgnkq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj202588.top/gtgtcxuldt.html

[Q57] 行号
来源：http://hz.dianchejie.cn/gtooycuyrv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhaomingkeji.xyz/gtbowmytrt.html

[Q58] 累计求和
来源：http://hz.chenzaomai.com/gttefpqlpj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258.top/gtesngxoep.html

[Q59] 分组内累计
来源：http://hz.sxryk.cn/gtpbvvdvao.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sxryk.cn/gtogdcumfo.html

[Q60] 取上一行 / 下一行
来源：http://hz.tianlin.xyz/gtmjbqhdhu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hammf.cn/gtxcuhypqq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ydjk.org.cn/gtuzknksls.html

[Q61] 移动平均
来源：http://hz.wangshuangyany.cn/gtvxgkdtqb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtxpuzxkem.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gtgpfsnzda.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtenvnotdv.html

[Q63] 开启事务
来源：http://hz.hammf.cn/gtfofknbfn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenjidiqi.icu/gtsworafkv.html

[Q64] 提交事务
来源：http://hz.yuanzhike.top/gtfocfdbub.html

COMMIT;
来源：http://hz.wangshuangyany.cn/gtiwruejlb.html

[Q65] 回滚事务
来源：http://hz.mhx1999.top/gtibipmhdm.html

ROLLBACK;
来源：http://hz.shzxlz.cn/gtgrqdveec.html

[Q66] 行锁查询
来源：http://hz.jinqigfzy.top/gtcxmsvymu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daxiang520.top/gtilihkuyl.html

[Q67] 设置隔离级别
来源：http://hz.316326.xyz/gtbkqyagkv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ybcxt.top/gtzdqghyvs.html

[Q68] 保存点
来源：http://hz.sufxvd.cn/gthcgjyyga.html

SAVEPOINT sp1;
来源：http://hz.yongpay.top/gtzahwaiut.html

ROLLBACK TO sp1;
来源：http://hz.xinyue.icu/gttcxgogdt.html

[Q69] 查看执行计划
来源：http://hz.quarkkingdee.top/gttiefysst.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fzhhl.top/gtbyypbjbn.html

[Q70] 更新统计信息
来源：http://hz.wangshuangyany.cn/gteluticir.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtiudismnu.html

[Q71] 查看建表语句
来源：http://hz.cqqwz.cn/gtsynwmagh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gtcrbfcflg.html

[Q72] 查看索引
来源：http://hz.pengpengdd.cyou/gtsqxjjyic.html

SHOW INDEX FROM users;
来源：http://hz.jinyuanbaomall.cn/gtfexbhzls.html

[Q73] 查看表状态
来源：http://hz.zhengqikj.top/gthwyrdeeq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tanke756.top/gtwuyljclk.html

[Q74] 强制使用索引
来源：http://hz.snrcjt.cn/gthseenbie.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ydjk.org.cn/gtgssymtko.html

[Q75] 日期格式化
来源：http://hz.dashuyun.cn/gtqurbfaiq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jqgufenzy.top/gtvyculllq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gtbpzqnklt.html

[Q76] 按天统计
来源：http://hz.xylfe.cn/gtzogjtnel.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtxwppodtj.html

[Q77] 时间加减
来源：http://hz.yj20258888.top/gtidwbkdlf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhiwuduotai.top/gtunvfurdk.html

[Q78] 当前时间
来源：http://hz.jinqigfzy.top/gtyqduotwm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sxryk.cn/gtjmvytgnh.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtmnfldlqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xylfe.cn/gtzdosimvv.html

[Q80] 字符串截取
来源：http://hz.zhaomingkeji.xyz/gtwepltwqu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtxqizjnid.html

[Q81] 字符串替换
来源：http://hz.yongpay.top/gtlgdbbdkf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgfzy.top/gtarqrunzo.html

[Q82] 字符长度与字节长度
来源：http://hz.jiagoushi.top/gttrnyjlkg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhengqikj.top/gtjuicxzxt.html

[Q83] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtbdhkgjqb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fzhhl.top/gtkdjstqfh.html

[Q84] 去除首尾空格
来源：http://hz.cashguo.top/gtiaozwbey.html

SELECT TRIM(name) FROM users;
来源：http://hz.sufxvd.cn/gtvukvmcpt.html

[Q85] 数值取整
来源：http://hz.havefunace.top/gtismwexqf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shangyingyoupin.top/gtgjbmuzkt.html

[Q86] 读取 JSON 字段
来源：http://hz.smart0.xyz/gtbhxmzdae.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.andypj.xyz/gtplmftxqk.html

[Q87] JSON 字段做条件
来源：http://hz.snrcjt.cn/gtiggulrqh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgfzy.top/gtsbvwvrtr.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtjgbpctwm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.0kj1m.cn/gtpnngfnmg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jianghu66.top/gtmnfjlufd.html

[Q89] 判断表是否存在
来源：http://hz.ywan-chungtsiang.top/gtrnybswyc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pengpengdd.cyou/gthqkadcvs.html

[Q90] 生成序号列
来源：http://hz.yj20258888.top/gtvyjaadfx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangshuangyany.cn/gtzayrfcyo.html

================================================================================
来源：http://hz.chenlongwang.top/gtiebvpqzk.html

R. Bash 专题
来源：http://hz.iojbl.cn/gtjpxypgvy.html

================================================================================
来源：http://hz.ppjwa.cn/gtugsunkkc.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtzwecrnlx.html

#!/usr/bin/env bash
来源：http://hz.yonumen.top/gterpjgfaz.html

set -euo pipefail
来源：http://hz.fengsongda.top/gtmqktmplq.html

[R02] 变量赋值与使用
来源：http://hz.sufxvd.cn/gtwaxzihiu.html

name="Tom"; echo "$name"
来源：http://hz.ppjwa.cn/gtqqrwagcg.html

[R03] 只读变量
来源：http://hz.dashuyun.cn/gtmebmdash.html

readonly PI=3.14
来源：http://hz.guowangkeji.top/gtjazvnokq.html

[R04] 位置参数
来源：http://hz.sufxvd.cn/gtcucpidcx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gtsxlwvbkr.html

[R05] 参数默认值
来源：http://hz.shanyushiyangtech.top/gtfrucsljn.html

name="${1:-default}"
来源：http://hz.zhengqikj.top/gtuwuvhjhh.html

[R06] 判断命令是否存在
来源：http://hz.0kj1m.cn/gtsaevpfmw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cashguo.top/gtfynrndxp.html

[R07] if 判断文件
来源：http://hz.cucudq.cn/gtfviretoc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zycfv.cn/gtjuqhxvzb.html

[R08] 数值比较
来源：http://hz.hongshengwenyu.top/gttscehbio.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtvsohfxbv.html

[R09] 字符串比较
来源：http://hz.zdqjudy.top/gtknpwakmk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtlrckzesb.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtpzgmbhzv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gtdloydfhj.html

[R11] case 多分支
来源：http://hz.quarkkingdee.top/gterbfekap.html

case "$1" in
来源：http://hz.gogol.net.cn/gtzepheiaf.html

start) echo "启动" ;;
来源：http://hz.vqdsnc.cn/gtnhnuekef.html

stop)  echo "停止" ;;
来源：http://hz.jiagoushi.top/gthcuzodzu.html

*)     echo "未知命令" ;;
来源：http://hz.tianlin.xyz/gtpdpsfziu.html

esac
来源：http://hz.hongshengwenyu.top/gtowalxunw.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gtqxcvrxfy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.mhx1999.top/gtefzotaki.html

[R13] for 计数循环
来源：http://hz.ppjwa.cn/gtnfqrnjfz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtufwvgmxp.html

[R14] C 风格 for
来源：http://hz.52xcode.cn/gtcwkywhkm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.iojbl.cn/gtoukxxqiw.html

[R15] while 逐行读文件
来源：http://hz.jinghuilouyu.cn/gtxwmfqcyu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.9152youxi.cn/gtevsyhxrq.html

[R16] until 等待条件
来源：http://hz.nanxinkj.top/gtleesfsdt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gtnhyseaxt.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtkekvdzyr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ppjwa.cn/gtklbiwqcf.html

[R18] 遍历数组
来源：http://hz.cucudq.cn/gtcukhliuu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtpqcnngyo.html

[R19] 数组长度
来源：http://hz.sufxvd.cn/gtwmkkprrg.html

echo "${#arr[@]}"
来源：http://hz.ivvv.top/gtvokjvjjk.html

[R20] 关联数组（字典）
来源：http://hz.yueranfly.top/gtljvcizkf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ppjwa.cn/gtjhugvguy.html

[R21] 字符串长度
来源：http://hz.ywan-chungtsiang.top/gtzwbfgsmp.html

echo "${#s}"
来源：http://hz.zdqjudy.top/gtkhvdrnjj.html

[R22] 截取子串
来源：http://hz.9152youxi.cn/gttsmonvob.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gtpkhcddag.html

[R23] 字符串替换
来源：http://hz.hysaishi.cn/gtmhtgjrsq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtosefhgfw.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gtghyjshjj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigufen.top/gtauncxgxj.html

[R25] 去后缀 / 去前缀
来源：http://hz.xziqi.cn/gtnzbxoake.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gtqadumkpz.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gterfmmfov.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gtkmojigpg.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gtllnfdsei.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gtgmhqfzyz.html

[R28] 浮点运算
来源：http://hz.zhixingplan.top/gtqwpndzzv.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinyuanbaomall.cn/gtjiitrovu.html

[R29] 定义函数
来源：http://hz.quarkkingdee.top/gtfxxelhou.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gtodyiihjk.html

[R30] 函数返回状态码
来源：http://hz.zhengqikj.top/gtlfminhuw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xziqi.cn/gtcyzwdqto.html

[R31] 局部变量
来源：http://hz.snrcjt.cn/gtmkbyetet.html

f() { local x=1; echo "$x"; }
来源：http://hz.birdmap.top/gtwcixregq.html

[R32] 参数个数校验
来源：http://hz.c1oappe.top/gtbitmssbn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hnxiangtu.top/gtnlieyaed.html

[R33] 捕获错误并提示行号
来源：http://hz.wangshuangyany.cn/gtcuzlrqgj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guannengcc.top/gtlzysoksy.html

[R34] 退出时清理
来源：http://hz.hnqzz.top/gthzqqgcsz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gthbylfrfv.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gteikcovxf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jlsjyb.cn/gtybophlox.html

[R36] 并发执行多个任务
来源：http://hz.yuanzhike.top/gtvzuamdmo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.0kj1m.cn/gttilxresr.html

[R37] 把输出赋给变量
来源：http://hz.ehwqpu.com/gtjbwzaski.html

files=$(ls -1)
来源：http://hz.xinyue.icu/gtdxxmwfzs.html

[R38] 管道串联
来源：http://hz.redwolf501.top/gtxdlicocf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtsshgpmhw.html

[R39] 重定向标准输出与错误
来源：http://hz.cheryme.top/gtatsmkhxq.html

cmd > out.log 2>&1
来源：http://hz.jinqigfzy.top/gtywyunyqz.html

[R40] 追加写日志
来源：http://hz.zhijiandao.cn/gtjpydzcnk.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtvwolojeo.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gtcvtkkrii.html

cmd >/dev/null 2>&1
来源：http://hz.ybcxt.top/gtrlnufhbd.html

[R42] 输入重定向
来源：http://hz.shzxlz.cn/gtbdlvdjrg.html

wc -l < a.txt
来源：http://hz.sweek.top/gtadhshvmy.html

[R43] 按名字查找文件
来源：http://hz.nanxinkj.top/gtgosdibsz.html

find . -name "*.log" -type f
来源：http://hz.hongshengwenyu.top/gttrzalyij.html

[R44] 按修改时间查找
来源：http://hz.kuanghao11.cn/gtiwngarsz.html

find . -mtime -7 -type f
来源：http://hz.hnxiangtu.top/gtkzlizbdn.html

[R45] 批量删除
来源：http://hz.cashguo.top/gtmpgavnwn.html


<!-- 参考信息 -->