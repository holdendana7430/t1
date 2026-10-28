代发 wailian999

CREATE TABLE users (
来源：http://hz.jyoumei.cn/gtfzwfgcoj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gogol.net.cn/gtktxxlgua.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gtxhaylzgj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtxriwdwpj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.havefunace.top/gtyrxivpmz.html

);
来源：http://hz.meibo888.top/gtkvyecpym.html

[Q02] 创建带外键的表
来源：http://hz.havefunace.top/gtcbjfbnrq.html

CREATE TABLE orders (
来源：http://hz.yvedp.cn/gtruygramp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtmkzrcrmc.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtjljwtovq.html

amount DECIMAL(10, 2),
来源：http://hz.yuxming.cn/gtqdimritl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ywan-chungtsiang.top/gtwapgstye.html

);
来源：http://hz.jianghu66.top/gtogyhbhqu.html

[Q03] 增加列
来源：http://hz.cucudq.cn/gtrabaevys.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhengqikj.top/gtamiewxex.html

[Q04] 修改列类型
来源：http://hz.xingfuxueyuan.xyz/gttcxunxtl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj20258.top/gtejcvtxfw.html

[Q05] 重命名列
来源：http://hz.ydzc1.top/gtmradubqa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.pycfn.com/gtvhavvowd.html

[Q06] 删除列
来源：http://hz.gaohongyu789.top/gthodzvlaq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jianghu66.top/gtmmoshxry.html

[Q07] 删除表
来源：http://hz.ywan-chungtsiang.top/gtekmrqemn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangdashe.top/gttuhxvuod.html

[Q08] 创建普通索引
来源：http://hz.yueranfly.top/gtzqbyhotn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtascuajjy.html

[Q09] 创建唯一索引
来源：http://hz.xuetiantiany.cn/gthowsqzeb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hammf.cn/gtvdadzhcn.html

[Q10] 插入单行
来源：http://hz.xziqi.cn/gtvrswfcki.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.svipenyu.cn/gtzmrbethb.html

[Q11] 一次插入多行
来源：http://hz.vqdsnc.cn/gtarfpqhsg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jyoumei.cn/gtincpctae.html

[Q12] 插入后取自增 ID
来源：http://hz.zhaomingkeji.xyz/gtrtyvfmph.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cqqwz.cn/gtcbogqdza.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tianlin.xyz/gtlzaqmgnr.html

[Q13] 忽略重复插入
来源：http://hz.kuanghao11.cn/gtfykpgtrm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgfzy.top/gtivbrfhak.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gtvowhieuu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhongyouzk.top/gtxcvmtapf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sxryk.cn/gthfxhydwl.html

[Q15] 查询全部
来源：http://hz.vqdsnc.cn/gtoyrslzas.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtkhvoudvy.html

[Q16] 查询指定列
来源：http://hz.sxryk.cn/gtaslrdyvi.html

SELECT id, name FROM users;
来源：http://hz.hammf.cn/gtowgtwbtt.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gteeuclelj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cdnleiting.top/gtwjkagxvy.html

[Q18] 模糊匹配
来源：http://hz.9152youxi.cn/gtnogjusmg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtrtwmqotz.html

[Q19] 范围查询
来源：http://hz.svipenyu.cn/gtilqcjgas.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daria6918.cn/gtjzcbsdyb.html

[Q20] IN 列表
来源：http://hz.hongshengwenyu.top/gtdvjcqija.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuanzx.com/gtclxyepkf.html

[Q21] 空值判断
来源：http://hz.tanke756.top/gtfvezedep.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhoulong.xyz/gtrizqhaee.html

[Q22] 排序
来源：http://hz.snrcjt.cn/gtfxvrbjaa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hammf.cn/gtzwkbllkb.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtuwpoelwt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.wangdashe.top/gtlehwgeqw.html

[Q24] 去重
来源：http://hz.ywan-chungtsiang.top/gtvbiuiucn.html

SELECT DISTINCT city FROM users;
来源：http://hz.shangyingyoupin.top/gtwlcwlwqz.html

[Q25] 只取前 N 条
来源：http://hz.52xcode.cn/gtueaanqob.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cashguo.top/gthvtfgscp.html

[Q26] 计数
来源：http://hz.yvedp.cn/gtqpsmgfmz.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangtech.top/gtlnhvwjst.html

[Q27] 条件计数
来源：http://hz.yueranfly.top/gtrdteklhz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pycfn.com/gtfbmvlirh.html

[Q28] 求和与平均
来源：http://hz.dianchejie.cn/gtpivlgnqq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jqgufenzy.top/gtwmspvzql.html

[Q29] 最大最小值
来源：http://hz.gogol.net.cn/gtzjsjfzgc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hfpthk.cn/gtdsuplckz.html

[Q30] 分组统计
来源：http://hz.yj20258888.top/gtysvcerpi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtpedxumjp.html

[Q31] 分组后过滤
来源：http://hz.shzxlz.cn/gtefzmswsz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.mhx1999.top/gtvuhpwimj.html

[Q32] 分组拼接字符串
来源：http://hz.gogol.net.cn/gtqeiotpnh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtwhvimxrm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yongpay.top/gtoepwruvb.html

[Q33] 多列分组
来源：http://hz.wangdashe.top/gtawcxzucz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.bjfxy.top/gtzupkubkm.html

[Q34] 每组取第一条
来源：http://hz.daxiang520.top/gtqtusomwf.html

SELECT * FROM (
来源：http://hz.yonumen.top/gtsoavxgqt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sweek.top/gteipqkfuw.html

) t WHERE rn = 1;
来源：http://hz.ywan-chungtsiang.top/gtvyhhcxgv.html

[Q35] 内连接
来源：http://hz.cashguo.top/gtmagxrgdh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtzovwftsh.html

[Q36] 左连接
来源：http://hz.zhixingplan.top/gttsxqlacg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtsespadlk.html

[Q37] 右连接
来源：http://hz.jlsjyb.cn/gtxodkkyyh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fengsongda.top/gtgqzfdhkx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gogol.net.cn/gtfujnokbj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gtqxtvewhs.html

[Q39] 自连接（查上下级）
来源：http://hz.0kj1m.cn/gthvvgtlbu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.redwolf501.top/gtzrmfxcxw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gtzzxbfpey.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yvedp.cn/gtonlenyio.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hysaishi.cn/gtisfsysbe.html

[Q41] 多表连接
来源：http://hz.sweek.top/gtszrpoztc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tanke756.top/gtialzwkbc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangkeji.top/gtmyqlniwj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ybcxt.top/gtvzlxvfwf.html

[Q42] 连接条件附加过滤
来源：http://hz.yvedp.cn/gtcbcdbxpb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sysykeji.top/gtzjtvdsdo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gtkzaesbmg.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtorhcaxzg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtjtzkemih.html

[Q44] IN 子查询
来源：http://hz.zdqjudy.top/gtplfdpywg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hongshengwenyu.top/gtwfdiztiq.html

[Q45] EXISTS 判断存在
来源：http://hz.hammf.cn/gtkiebhgaz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtjturobds.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hammf.cn/gttqhkbpnf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtnwscgyvk.html

[Q47] 与平均值比较
来源：http://hz.jyoumei.cn/gtvymqclvp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cashguo.top/gtzikzpvne.html

[Q48] CTE 公用表表达式
来源：http://hz.0kj1m.cn/gtvooctjis.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgufenzy.top/gtkjrlzrvx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yvedp.cn/gtfnvnltbc.html

[Q49] 更新单行
来源：http://hz.hywenlv.cn/gtdebplmsh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gogol.net.cn/gtgglrendm.html

[Q50] 批量更新
来源：http://hz.shangyingyoupin.top/gtfeuqmabq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnqzz.top/gtnbzbsmft.html

[Q51] 用子查询更新
来源：http://hz.yueranfly.top/gtohnrptqw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtvntmszza.html

[Q52] 删除指定行
来源：http://hz.fzhhl.top/gtldsyseob.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cdnleiting.top/gtfpidrwbw.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gteczlsygf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.svipenyu.cn/gtylllgllv.html

[Q54] 清空表
来源：http://hz.bjfxy.top/gtvxlgzsug.html

TRUNCATE TABLE logs;
来源：http://hz.xziqi.cn/gtgdzavbeb.html

[Q55] 排名（并列占位）
来源：http://hz.tanke756.top/gtqocvcwmr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gtsiqxqhee.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guowangkeji.top/gttmabgmhs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hfpthk.cn/gtuopmppgm.html

[Q57] 行号
来源：http://hz.jqgfzy.top/gtehtfgcou.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zycfv.cn/gtufnijsnu.html

[Q58] 累计求和
来源：http://hz.jianghu66.top/gtfdgytpdn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sxryk.cn/gtzddvgjno.html

[Q59] 分组内累计
来源：http://hz.birdmap.top/gtfkibcwtv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.bjfxy.top/gtdykwwens.html

[Q60] 取上一行 / 下一行
来源：http://hz.aizwys.cn/gtbjoidotv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgufenzy.top/gtogyguawr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shanyushiyangtech.top/gtonshbwfe.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gtksfutdnc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yanxiufei.cn/gtjfwdzamm.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtddqgngja.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtnzkauaro.html

[Q63] 开启事务
来源：http://hz.wangdashe.top/gtdxzbtdcs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.guowangkeji.top/gtspuvbkmm.html

[Q64] 提交事务
来源：http://hz.hysaishi.cn/gtvkjqgmqc.html

COMMIT;
来源：http://hz.cqqwz.cn/gtpmorctdp.html

[Q65] 回滚事务
来源：http://hz.chenjidiqi.icu/gtssfylieu.html

ROLLBACK;
来源：http://hz.shangyingyoupin.top/gtcfvbgsza.html

[Q66] 行锁查询
来源：http://hz.kuanghao11.cn/gtqylxqrho.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.0kj1m.cn/gtwabnhnme.html

[Q67] 设置隔离级别
来源：http://hz.jlsjyb.cn/gtliyndddt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shzxlz.cn/gtcyvmxjju.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtblhjbtqi.html

SAVEPOINT sp1;
来源：http://hz.dianchejie.cn/gtosmdvbht.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtxpnmbhuh.html

[Q69] 查看执行计划
来源：http://hz.chenzaomai.com/gtuvhopxqu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xinyue.icu/gtauianagj.html

[Q70] 更新统计信息
来源：http://hz.aibaodan.cn/gtmzsibjwh.html

ANALYZE TABLE users;
来源：http://hz.yj20258888.top/gtjdonzogx.html

[Q71] 查看建表语句
来源：http://hz.jinghuilouyu.cn/gtarytytzg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ehwqpu.com/gtqdczxpuj.html

[Q72] 查看索引
来源：http://hz.guannengcc.top/gtqwkthyti.html

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtxskprmps.html

[Q73] 查看表状态
来源：http://hz.cqqwz.cn/gtizosqifn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gogol.net.cn/gtaerggewf.html

[Q74] 强制使用索引
来源：http://hz.dianchejie.cn/gtfncfxbcq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.andypj.xyz/gtlpqopqiw.html

[Q75] 日期格式化
来源：http://hz.ybcxt.top/gtvojvssej.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtkbwmddzx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tian-w.cn/gtsizyerbu.html

[Q76] 按天统计
来源：http://hz.daria6918.cn/gthldipteg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhengqikj.top/gtxkrpbcti.html

[Q77] 时间加减
来源：http://hz.ybcxt.top/gtxaxlkicf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tian-w.cn/gtiirxidsh.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gtyrykkndt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhiwuduotai.top/gtrdeqsmjs.html

[Q79] 字符串拼接
来源：http://hz.xziqi.cn/gtophidkob.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jiagoushi.top/gtxcztpjuo.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gtennyxgyp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.smart0.xyz/gtjookbsta.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtxeegjprw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.havefunace.top/gtkstzwwpc.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtqswcbcni.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.c1oappe.top/gtshqufiay.html

[Q83] 大小写转换
来源：http://hz.zdqjudy.top/gtnwvzrery.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aizwys.cn/gtaauwzjbw.html

[Q84] 去除首尾空格
来源：http://hz.hnqzz.top/gtywxyzrce.html

SELECT TRIM(name) FROM users;
来源：http://hz.smart0.xyz/gtaduophmf.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtfdboutzv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ppjwa.cn/gtzobqgxsq.html

[Q86] 读取 JSON 字段
来源：http://hz.cashguo.top/gtdmdvslto.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shzxlz.cn/gtlmdhpxys.html

[Q87] JSON 字段做条件
来源：http://hz.ydjk.org.cn/gtlsgxaybr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aibaodan.cn/gtsasqblxz.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gthntyoxab.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtkcutfiel.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.9152youxi.cn/gtqjnerscl.html

[Q89] 判断表是否存在
来源：http://hz.gogol.net.cn/gtsftptpep.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigfzy.top/gtmnilgrry.html

[Q90] 生成序号列
来源：http://hz.wangdashe.top/gteidzgtev.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.haohaochexian.top/gtggjgrrik.html

================================================================================
来源：http://hz.daxiang520.top/gtodfybwiu.html

R. Bash 专题
来源：http://hz.aizwys.cn/gtjnrskzfq.html

================================================================================
来源：http://hz.xuanzx.com/gtjduwyqyg.html

[R01] shebang 与严格模式
来源：http://hz.aibaodan.cn/gtchggwyui.html

#!/usr/bin/env bash
来源：http://hz.jinqigufen.top/gtcpgbuslz.html

set -euo pipefail
来源：http://hz.havefunace.top/gtukjwyelt.html

[R02] 变量赋值与使用
来源：http://hz.shuidangran.top/gtszqaenhc.html

name="Tom"; echo "$name"
来源：http://hz.yj20258.top/gtkwqpygjb.html

[R03] 只读变量
来源：http://hz.snrcjt.cn/gtogusaycm.html

readonly PI=3.14
来源：http://hz.xuetiantiany.cn/gteqbvyukx.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtedikixbs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hysaishi.cn/gtnjwkzkme.html

[R05] 参数默认值
来源：http://hz.andypj.xyz/gtidifvbja.html

name="${1:-default}"
来源：http://hz.daria6918.cn/gtgnmtogdq.html

[R06] 判断命令是否存在
来源：http://hz.hnqzz.top/gtrtcggtij.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hammf.cn/gtsuknozcs.html

[R07] if 判断文件
来源：http://hz.nanxinkj.top/gtyrxlmkju.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ivvv.top/gtvdpmzxpa.html

[R08] 数值比较
来源：http://hz.kuanghao11.cn/gthpjrpshy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yvedp.cn/gtzkpvmwdw.html

[R09] 字符串比较
来源：http://hz.jiagoushi.top/gtksmztdml.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtuwewczjv.html

[R10] 正则匹配
来源：http://hz.jianghu66.top/gtirlrwuag.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gtpfhnwutj.html

[R11] case 多分支
来源：http://hz.yangfankeji.com/gtmhvesbsg.html

case "$1" in
来源：http://hz.sweek.top/gtzkaruwky.html

start) echo "启动" ;;
来源：http://hz.mhx1999.top/gtdcwxkwkc.html

stop)  echo "停止" ;;
来源：http://hz.nanxinkj.top/gtfqktdmlx.html

*)     echo "未知命令" ;;
来源：http://hz.ywan-chungtsiang.top/gtpugssbtr.html

esac
来源：http://hz.haohaochexian.top/gtqnkkydgl.html

[R12] for 遍历文件
来源：http://hz.zdqjudy.top/gtuajpkcjv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gttkysdkjt.html

[R13] for 计数循环
来源：http://hz.meibo888.top/gtbedtsilo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gotoacloud.top/gtsutoqwvt.html

[R14] C 风格 for
来源：http://hz.zhoulong.xyz/gtlkwmfdpo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gtfuvvmqkc.html

[R15] while 逐行读文件
来源：http://hz.hammf.cn/gtdnaepkfd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aizwys.cn/gtrqqibhaj.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gtsgbarccx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cdnleiting.top/gtmwkfoopi.html

[R17] 数组定义与取值
来源：http://hz.ppjwa.cn/gtnvakotfa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydjk.org.cn/gtllepcwvj.html

[R18] 遍历数组
来源：http://hz.ydjk.org.cn/gtooliczeh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.kuanghao11.cn/gtsslhxnyp.html

[R19] 数组长度
来源：http://hz.gogol.net.cn/gtsfyggisy.html

echo "${#arr[@]}"
来源：http://hz.gotoacloud.top/gtncrxtzxk.html

[R20] 关联数组（字典）
来源：http://hz.cheryme.top/gtuwtnpvie.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigufen.top/gtgqkdxuix.html

[R21] 字符串长度
来源：http://hz.andypj.xyz/gtljsqbjgl.html

echo "${#s}"
来源：http://hz.yueranfly.top/gtyufuilnr.html

[R22] 截取子串
来源：http://hz.snrcjt.cn/gtcizafcaq.html

echo "${s:0:5}"
来源：http://hz.ehwqpu.com/gtfqffbukk.html

[R23] 字符串替换
来源：http://hz.fengsongda.top/gtrjnfplxu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gogol.net.cn/gtuhigtqfr.html

[R24] 大小写转换
来源：http://hz.chenjidiqi.icu/gtcnplmkzd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenlongwang.top/gtphnyuydc.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhoulong.xyz/gtwjyfired.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.svipenyu.cn/gtciaifgie.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtgakuzext.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigfzy.top/gtshsxguxq.html

[R27] 算术展开
来源：http://hz.pengpengdd.cyou/gtblklaewg.html

echo $((1 + 2 * 3))
来源：http://hz.pengpengdd.cyou/gtprlwpsan.html

[R28] 浮点运算
来源：http://hz.ivvv.top/gthyebcmlc.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gtpseounlg.html

[R29] 定义函数
来源：http://hz.bjfxy.top/gtltnzfscy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jlsjyb.cn/gtfwwpsixj.html

[R30] 函数返回状态码
来源：http://hz.xingfuxueyuan.xyz/gthnylrkzz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.kuanghao11.cn/gtragfkoku.html

[R31] 局部变量
来源：http://hz.hysaishi.cn/gtxknhdypo.html

f() { local x=1; echo "$x"; }
来源：http://hz.birdmap.top/gtdtoiywfx.html

[R32] 参数个数校验
来源：http://hz.shangyingyoupin.top/gtpjheqqnm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ybcxt.top/gtwydkcuap.html

[R33] 捕获错误并提示行号
来源：http://hz.9152youxi.cn/gtlxpkvood.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gthofammyp.html

[R34] 退出时清理
来源：http://hz.hnxiangtu.top/gtyykxqgxe.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtkphtwbnw.html

[R35] 后台执行并等待
来源：http://hz.xuetiantiany.cn/gtxituzfcb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhengqikj.top/gtcrzysnik.html

[R36] 并发执行多个任务
来源：http://hz.jiagoushi.top/gtpevfpufp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnqzz.top/gttegcyzqe.html

[R37] 把输出赋给变量
来源：http://hz.yanxiufei.cn/gthkommllg.html

files=$(ls -1)
来源：http://hz.zdqjudy.top/gttazbwwxp.html

[R38] 管道串联
来源：http://hz.nanxinkj.top/gtlkbpnyee.html

cat a.txt | grep -i error | wc -l
来源：http://hz.wangdashe.top/gtntruxfsj.html

[R39] 重定向标准输出与错误
来源：http://hz.cheryme.top/gtsdzdjdtb.html

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gtgnewfucm.html

[R40] 追加写日志
来源：http://hz.gotoacloud.top/gthduftsxv.html

echo "log" >> out.log
来源：http://hz.tanke756.top/gtvqmmgdwl.html

[R41] 丢弃输出
来源：http://hz.c1oappe.top/gthqznsemr.html

cmd >/dev/null 2>&1
来源：http://hz.meibo888.top/gtddgdtezd.html

[R42] 输入重定向
来源：http://hz.kuanghao11.cn/gtfeoerrnz.html

wc -l < a.txt
来源：http://hz.yueranfly.top/gtbtfiacpr.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtnkkqchru.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtsvcafxbn.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gtcrxwylpg.html

find . -mtime -7 -type f
来源：http://hz.jinqigufen.top/gtskqhnyge.html

[R45] 批量删除
来源：http://hz.zhixingplan.top/gtyzbeqceq.html


<!-- 参考信息 -->