代发 wailian999

CREATE TABLE users (
来源：http://hz.zhoulong.xyz/gtikzgipgg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtrvhixclf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aizwys.cn/gtbfnzmmzl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ybcxt.top/gtzkjtwkre.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jyoumei.cn/gtktxgxoxk.html

);
来源：http://hz.316326.xyz/gtwnsrtgip.html

[Q02] 创建带外键的表
来源：http://hz.redwolf501.top/gtpcomsufd.html

CREATE TABLE orders (
来源：http://hz.guowangkeji.top/gtriiuzfog.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gtrdgajrku.html

user_id INT NOT NULL,
来源：http://hz.xuetiantiany.cn/gttpumhicv.html

amount DECIMAL(10, 2),
来源：http://hz.zhaomingkeji.xyz/gthsstfkhb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fzhhl.top/gtzqptnnkj.html

);
来源：http://hz.hongshengwenyu.top/gtqqnijjuy.html

[Q03] 增加列
来源：http://hz.0kj1m.cn/gtkcziyafe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.316326.xyz/gtjlhwbhjw.html

[Q04] 修改列类型
来源：http://hz.wangdashe.top/gtartybqqh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenzaomai.com/gtpcrgwfjv.html

[Q05] 重命名列
来源：http://hz.chenzaomai.com/gtnvyvsufm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hywenlv.cn/gtxmlodecg.html

[Q06] 删除列
来源：http://hz.cqqwz.cn/gtxjxmewle.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hfpthk.cn/gtowpkglss.html

[Q07] 删除表
来源：http://hz.jinqigufen.top/gtfisxfemv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pycfn.com/gtpipxutwy.html

[Q08] 创建普通索引
来源：http://hz.hnxiangtu.top/gtlorhlywp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtiwpuklvr.html

[Q09] 创建唯一索引
来源：http://hz.ppjwa.cn/gteyxviykt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.aibaodan.cn/gtvlnrblin.html

[Q10] 插入单行
来源：http://hz.andypj.xyz/gtbylwiaui.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtlzdmgtri.html

[Q11] 一次插入多行
来源：http://hz.tian-w.cn/gtodbfkare.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zdqjudy.top/gtspayasfw.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtwkitkkux.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ywan-chungtsiang.top/gtaskhqbsl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tanke756.top/gtiiqxfeoa.html

[Q13] 忽略重复插入
来源：http://hz.hongshengwenyu.top/gtivpjpmce.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aizwys.cn/gtczfzymje.html

[Q14] 存在则更新（upsert）
来源：http://hz.tianlin.xyz/gtwiwlsewe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.iojbl.cn/gtnrdtjhje.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zycfv.cn/gtitybbvdy.html

[Q15] 查询全部
来源：http://hz.xuanzx.com/gtxrcjlplo.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtferchaud.html

[Q16] 查询指定列
来源：http://hz.shangyingyoupin.top/gtbreqnhrv.html

SELECT id, name FROM users;
来源：http://hz.dianchejie.cn/gtfissvdoh.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtwmhfrqfk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hywenlv.cn/gtmvzelhhd.html

[Q18] 模糊匹配
来源：http://hz.zhaomingkeji.xyz/gtjpmwoprj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daria6918.cn/gtvsocfkcv.html

[Q19] 范围查询
来源：http://hz.aibaodan.cn/gtvndaeweo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daxiang520.top/gttmbvxbwq.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gtrfcsvxic.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zycfv.cn/gtgwvszvpw.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtixjdinmq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gzhubu.top/gtiagkktuy.html

[Q22] 排序
来源：http://hz.gaohongyu789.top/gtxfanoprc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aizwys.cn/gtslbbvbdp.html

[Q23] 分页
来源：http://hz.cashguo.top/gtckpxsqai.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.vqdsnc.cn/gtydtcomhy.html

[Q24] 去重
来源：http://hz.yvedp.cn/gtiyinrqrj.html

SELECT DISTINCT city FROM users;
来源：http://hz.xylfe.cn/gtwdktyntg.html

[Q25] 只取前 N 条
来源：http://hz.hnqzz.top/gtnuhbtxec.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jlsjyb.cn/gtkpxqnxye.html

[Q26] 计数
来源：http://hz.kuanghao11.cn/gtlgnymoij.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenlongwang.top/gtroknzvco.html

[Q27] 条件计数
来源：http://hz.zhaomingkeji.xyz/gtufjmevzz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinqigufen.top/gtxsujwfpo.html

[Q28] 求和与平均
来源：http://hz.hongshengwenyu.top/gtufisvyor.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenzaomai.com/gtxalggxzx.html

[Q29] 最大最小值
来源：http://hz.smart0.xyz/gtcmzpvnjq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sweek.top/gtsibpywwc.html

[Q30] 分组统计
来源：http://hz.tanke756.top/gtqnnbutcl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtwvskifup.html

[Q31] 分组后过滤
来源：http://hz.kuanghao11.cn/gtlhwybkkm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ywan-chungtsiang.top/gtrojasbuq.html

[Q32] 分组拼接字符串
来源：http://hz.dianchejie.cn/gtalcooyeu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtytxcojbf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtokwueezr.html

[Q33] 多列分组
来源：http://hz.daxiang520.top/gtnxzvdzjw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuanzhike.top/gtekwvtuzv.html

[Q34] 每组取第一条
来源：http://hz.fengsongda.top/gtdscbumax.html

SELECT * FROM (
来源：http://hz.jqgufenzy.top/gtpfmcneas.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ybcxt.top/gtjrcxuxvf.html

) t WHERE rn = 1;
来源：http://hz.cheryme.top/gtuxblvupi.html

[Q35] 内连接
来源：http://hz.xylfe.cn/gtacnnhouv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtrokuhivq.html

[Q36] 左连接
来源：http://hz.yj20258.top/gtwumslitq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtyhptqgdo.html

[Q37] 右连接
来源：http://hz.zhongyouzk.top/gtfauckbqg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jianghu66.top/gtvqkkxytp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xziqi.cn/gttgluasyu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shzxlz.cn/gtwaryxmpd.html

[Q39] 自连接（查上下级）
来源：http://hz.smart0.xyz/gtmkrizxpv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gotoacloud.top/gtdmufsvnu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gturmxccmv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuanzx.com/gtiumblfve.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xingfuxueyuan.xyz/gtjlxlkund.html

[Q41] 多表连接
来源：http://hz.fengsongda.top/gtnxmsmpoa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.52xcode.cn/gtyuqczqtq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.vqdsnc.cn/gtkdnfimir.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hywenlv.cn/gtsrjhchef.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gtqhgkcxpu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.svipenyu.cn/gtaatmoojs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangdashe.top/gtuhxlkwvz.html

[Q43] 标量子查询
来源：http://hz.cdnleiting.top/gtdsqmuhcm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj202588.top/gtaramfhlg.html

[Q44] IN 子查询
来源：http://hz.zhengqikj.top/gtrrpylhqu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jiagoushi.top/gtrpdxhykl.html

[Q45] EXISTS 判断存在
来源：http://hz.dashuyun.cn/gtgtkutdqw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtrgjdfjav.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtefwycipz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtdqcsmtty.html

[Q47] 与平均值比较
来源：http://hz.cashguo.top/gtlocufehi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gtfjhjdzco.html

[Q48] CTE 公用表表达式
来源：http://hz.hnqzz.top/gtomuboivg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daria6918.cn/gttsucspjn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnqzz.top/gtdyrjwttx.html

[Q49] 更新单行
来源：http://hz.snrcjt.cn/gtgqaljemi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fzhhl.top/gtkuokfljb.html

[Q50] 批量更新
来源：http://hz.cashguo.top/gtsatpwuqp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gaohongyu789.top/gtuvjerjdo.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gtjoplrddo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tianlin.xyz/gtjzhdpehc.html

[Q52] 删除指定行
来源：http://hz.jinqigufen.top/gtlhbotevg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtppvlwiex.html

[Q53] 按条件删除
来源：http://hz.chenjidiqi.icu/gtadsdrwvm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jlsjyb.cn/gtdglrpzpp.html

[Q54] 清空表
来源：http://hz.ppjwa.cn/gtvzmijrnh.html

TRUNCATE TABLE logs;
来源：http://hz.havefunace.top/gtgulffnik.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtrbfqbems.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cheryme.top/gtrsxkjlqt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shuidangran.top/gtgjczpwfy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daria6918.cn/gtfisbtrup.html

[Q57] 行号
来源：http://hz.guannengcc.top/gtvasfolln.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sysykeji.top/gtiwvujpvm.html

[Q58] 累计求和
来源：http://hz.shanyushiyangkeji.top/gtfwcafpkr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.0kj1m.cn/gtkrnttyxh.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gtvniiyfwm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.smart0.xyz/gtcinmcgrn.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuanzhike.top/gtdxcqjgpd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtoijghazr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhiwuduotai.top/gtlglrssgv.html

[Q61] 移动平均
来源：http://hz.daria6918.cn/gthhxplmwy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hysaishi.cn/gtxizumztq.html

[Q62] 分组占比
来源：http://hz.hysaishi.cn/gtplcqnmbu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtykdzevog.html

[Q63] 开启事务
来源：http://hz.xylfe.cn/gtwbkprofx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenlongwang.top/gtrblfovzw.html

[Q64] 提交事务
来源：http://hz.feifeiyinyue.top/gtcnnqjpcz.html

COMMIT;
来源：http://hz.hysaishi.cn/gtqzyjzsuy.html

[Q65] 回滚事务
来源：http://hz.gogol.net.cn/gtgprphmez.html

ROLLBACK;
来源：http://hz.yueranfly.top/gtmirswpeq.html

[Q66] 行锁查询
来源：http://hz.zhongyouzk.top/gtjyfizfrd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yanxiufei.cn/gttmufkulv.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gtdivsxgrp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258888.top/gtpwoqwbhl.html

[Q68] 保存点
来源：http://hz.hywenlv.cn/gtmszvhccu.html

SAVEPOINT sp1;
来源：http://hz.wangdashe.top/gtqydvsmrm.html

ROLLBACK TO sp1;
来源：http://hz.shangyingyoupin.top/gtwziapaot.html

[Q69] 查看执行计划
来源：http://hz.yanxiufei.cn/gtlobmlpmw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhoulong.xyz/gtadwdowga.html

[Q70] 更新统计信息
来源：http://hz.wangshuangyany.cn/gtqejixgbu.html

ANALYZE TABLE users;
来源：http://hz.xinyue.icu/gtovmunvft.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gtwpaqtsfg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.feifeiyinyue.top/gtbrttmlbm.html

[Q72] 查看索引
来源：http://hz.jlsjyb.cn/gtaafzdize.html

SHOW INDEX FROM users;
来源：http://hz.tianlin.xyz/gthdkwoinn.html

[Q73] 查看表状态
来源：http://hz.cqqwz.cn/gtyweijboo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cqqwz.cn/gtcqxmbixn.html

[Q74] 强制使用索引
来源：http://hz.jqgufenzy.top/gtenbcdxuu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zycfv.cn/gtfieuycqe.html

[Q75] 日期格式化
来源：http://hz.hfpthk.cn/gtrzzomojb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtdbedwxnm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shangyingyoupin.top/gtmmjlhqbc.html

[Q76] 按天统计
来源：http://hz.shangyingyoupin.top/gtqmnmowii.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yvedp.cn/gtchnkrlvj.html

[Q77] 时间加减
来源：http://hz.pengpengdd.cyou/gtplwzbzob.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gtgcjkmjsw.html

[Q78] 当前时间
来源：http://hz.shangyingyoupin.top/gtzszwmxah.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gtzrevfgoc.html

[Q79] 字符串拼接
来源：http://hz.jinqigufen.top/gtcoryoxgk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.mhx1999.top/gtqsofzmnv.html

[Q80] 字符串截取
来源：http://hz.xuanzx.com/gtpcjzlhnt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtmeizubmv.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gtzrzpzxdm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shangyingyoupin.top/gtbcislmve.html

[Q82] 字符长度与字节长度
来源：http://hz.smart0.xyz/gttrcleidq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guowangkeji.top/gthasxcpdz.html

[Q83] 大小写转换
来源：http://hz.ivvv.top/gtqhrfvrci.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigufen.top/gtmlomqlbc.html

[Q84] 去除首尾空格
来源：http://hz.fzhhl.top/gtxniipmxl.html

SELECT TRIM(name) FROM users;
来源：http://hz.sysykeji.top/gthurwfcov.html

[Q85] 数值取整
来源：http://hz.yj20258.top/gtjkcuspmi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gotoacloud.top/gtzolqjyuy.html

[Q86] 读取 JSON 字段
来源：http://hz.gaohongyu789.top/gtzuubbflo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenjidiqi.icu/gtjvdtrnbj.html

[Q87] JSON 字段做条件
来源：http://hz.jqgfzy.top/gtyrwlacfs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangtech.top/gtbpbesicv.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuanzhike.top/gtemzpsous.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydjk.org.cn/gtgpfzghyr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fengsongda.top/gtonlgjaxg.html

[Q89] 判断表是否存在
来源：http://hz.tanke756.top/gtzpypxmel.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258.top/gtrtxmqufg.html

[Q90] 生成序号列
来源：http://hz.jlsjyb.cn/gtpufwnzim.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xziqi.cn/gtkskztkim.html

================================================================================
来源：http://hz.guannengcc.top/gtwcoyqsmf.html

R. Bash 专题
来源：http://hz.kuanghao11.cn/gtxalpvird.html

================================================================================
来源：http://hz.ivvv.top/gtwtcdompc.html

[R01] shebang 与严格模式
来源：http://hz.hnqzz.top/gtiyarmrlq.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtalkvvbtw.html

set -euo pipefail
来源：http://hz.shuidangran.top/gtfsbemdhc.html

[R02] 变量赋值与使用
来源：http://hz.nanxinkj.top/gtxousnxom.html

name="Tom"; echo "$name"
来源：http://hz.zycfv.cn/gtoiuzkbwu.html

[R03] 只读变量
来源：http://hz.cashguo.top/gtitdwmhcs.html

readonly PI=3.14
来源：http://hz.yueranfly.top/gtaojgqwny.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtsjpwzrgm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenlongwang.top/gtcejrqlsu.html

[R05] 参数默认值
来源：http://hz.yuxming.cn/gthawispzr.html

name="${1:-default}"
来源：http://hz.fzhhl.top/gttrxqqaen.html

[R06] 判断命令是否存在
来源：http://hz.mhx1999.top/gtwdatbumz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sysykeji.top/gtbjwjdbfl.html

[R07] if 判断文件
来源：http://hz.zycfv.cn/gtbuihhueu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hongshengwenyu.top/gtzojllmur.html

[R08] 数值比较
来源：http://hz.snrcjt.cn/gtwhvjktke.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yanxiufei.cn/gtiazjwwcq.html

[R09] 字符串比较
来源：http://hz.jiagoushi.top/gtvkmgomup.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.birdmap.top/gtiivfqngi.html

[R10] 正则匹配
来源：http://hz.shanyushiyangkeji.top/gtlyqesijj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj202588.top/gtjkilxcgm.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtlgjuexte.html

case "$1" in
来源：http://hz.zhixingplan.top/gtgjntrllc.html

start) echo "启动" ;;
来源：http://hz.guannengcc.top/gtbvksaizp.html

stop)  echo "停止" ;;
来源：http://hz.andypj.xyz/gtbnduliqu.html

*)     echo "未知命令" ;;
来源：http://hz.nanxuanxn.top/gtwcszeogq.html

esac
来源：http://hz.jinyuanbaomall.cn/gtlutcopfp.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtgweqhfrp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guannengcc.top/gtbiomxdxc.html

[R13] for 计数循环
来源：http://hz.sweek.top/gtcqfadidl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.iojbl.cn/gtzycdxcyn.html

[R14] C 风格 for
来源：http://hz.hfpthk.cn/gtzyhwgfrr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtjtipjwon.html

[R15] while 逐行读文件
来源：http://hz.redwolf501.top/gtqjypoafm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gtyslsqlwk.html

[R16] until 等待条件
来源：http://hz.cashguo.top/gtloesdzri.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gttktxcbrw.html

[R17] 数组定义与取值
来源：http://hz.vqdsnc.cn/gttnhgzqma.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtwjpvvyfl.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtgpaqfxqt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guowangkeji.top/gtxpjemxvf.html

[R19] 数组长度
来源：http://hz.redwolf501.top/gtlcrobnqy.html

echo "${#arr[@]}"
来源：http://hz.aibaodan.cn/gtdwzsubsj.html

[R20] 关联数组（字典）
来源：http://hz.dianchejie.cn/gtrgbmnuzg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shuidangran.top/gtngndmqmu.html

[R21] 字符串长度
来源：http://hz.tianlin.xyz/gtnjohpldp.html

echo "${#s}"
来源：http://hz.pycfn.com/gtprufjglc.html

[R22] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtbsimutlh.html

echo "${s:0:5}"
来源：http://hz.smart0.xyz/gtsazamnqp.html

[R23] 字符串替换
来源：http://hz.tanke756.top/gtikvrlkjk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnxiangtu.top/gtemayjour.html

[R24] 大小写转换
来源：http://hz.smart0.xyz/gtjvxttxie.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtkudgcxoa.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhengqikj.top/gtpoxtzoli.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.havefunace.top/gtglujtilz.html

[R26] 命令替换
来源：http://hz.snrcjt.cn/gtagzbffyc.html

now=$(date +%F); echo "$now"
来源：http://hz.zhaomingkeji.xyz/gtmqroshud.html

[R27] 算术展开
来源：http://hz.52xcode.cn/gtsqjenvow.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtqiuurtoh.html

[R28] 浮点运算
来源：http://hz.0kj1m.cn/gtmgxezdxf.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnxiangtu.top/gtbnkitfnz.html

[R29] 定义函数
来源：http://hz.pycfn.com/gtehuwitpn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zdqjudy.top/gtmgwftbhd.html

[R30] 函数返回状态码
来源：http://hz.nanxinkj.top/gtgjppxxkh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ehwqpu.com/gthwibvibg.html

[R31] 局部变量
来源：http://hz.kuanghao11.cn/gtnwekruus.html

f() { local x=1; echo "$x"; }
来源：http://hz.feifeiyinyue.top/gtgrkbyquj.html

[R32] 参数个数校验
来源：http://hz.vqdsnc.cn/gtbqpjyesg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtqfubfuqe.html

[R33] 捕获错误并提示行号
来源：http://hz.dianchejie.cn/gtlynrnqin.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.kuanghao11.cn/gtovubowef.html

[R34] 退出时清理
来源：http://hz.chenlongwang.top/gttorqljqk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtlkgsinxb.html

[R35] 后台执行并等待
来源：http://hz.bjfxy.top/gtaqrltewi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jiagoushi.top/gtwdmfqegj.html

[R36] 并发执行多个任务
来源：http://hz.guannengcc.top/gthdxogkyr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ehwqpu.com/gtvibdlagg.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtksacsqdi.html

files=$(ls -1)
来源：http://hz.mhx1999.top/gtwkwmulqj.html

[R38] 管道串联
来源：http://hz.hongshengwenyu.top/gtzgahciyt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtzcuwygmg.html

[R39] 重定向标准输出与错误
来源：http://hz.xylfe.cn/gtkdkfggwb.html

cmd > out.log 2>&1
来源：http://hz.shangyingyoupin.top/gtqhdpmfzf.html

[R40] 追加写日志
来源：http://hz.haohaochexian.top/gtkpfuzuvv.html

echo "log" >> out.log
来源：http://hz.redwolf501.top/gtjxeuyacz.html

[R41] 丢弃输出
来源：http://hz.shanyushiyangkeji.top/gtpbrfbajn.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtakqvrlpk.html

[R42] 输入重定向
来源：http://hz.dianchejie.cn/gtyznxdmzf.html

wc -l < a.txt
来源：http://hz.dianchejie.cn/gtnjfbkwtn.html

[R43] 按名字查找文件
来源：http://hz.jyoumei.cn/gtcduknoyi.html

find . -name "*.log" -type f
来源：http://hz.nwbrower.top/gttgkirwqs.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gtohyfeiqy.html

find . -mtime -7 -type f
来源：http://hz.chenzaomai.com/gtswltoaoc.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtwubypebd.html


<!-- 参考信息 -->