代发 wailian999

CREATE TABLE users (
来源：http://hz.haohaochexian.top/gtlidlnwes.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtasaswinn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yuxming.cn/gtzkciutzq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinghuilouyu.cn/gtshpxrxrh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhijiandao.cn/gthekqerag.html

);
来源：http://hz.hywenlv.cn/gtrrmdxndr.html

[Q02] 创建带外键的表
来源：http://hz.hongshengwenyu.top/gtvyatkqqi.html

CREATE TABLE orders (
来源：http://hz.zhijiandao.cn/gtbsjrkwho.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtsprasjfj.html

user_id INT NOT NULL,
来源：http://hz.yangfankeji.com/gtkgcfdphn.html

amount DECIMAL(10, 2),
来源：http://hz.wangshuangyany.cn/gtevmzvqbq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.feifeiyinyue.top/gteypnldps.html

);
来源：http://hz.quarkkingdee.top/gtjgojocpv.html

[Q03] 增加列
来源：http://hz.meibo888.top/gtxchzwdpy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhixingplan.top/gtdepejyra.html

[Q04] 修改列类型
来源：http://hz.cucudq.cn/gteamaxzld.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtyqtibkib.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtllyvyjyl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xuetiantiany.cn/gtahlriwub.html

[Q06] 删除列
来源：http://hz.havefunace.top/gtxcvsowoz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.0kj1m.cn/gtqsjokojp.html

[Q07] 删除表
来源：http://hz.hnqzz.top/gtjdyhhzph.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yongpay.top/gtdtjjbswx.html

[Q08] 创建普通索引
来源：http://hz.kuanghao11.cn/gtwhkvnmdq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xziqi.cn/gtdsqlepzy.html

[Q09] 创建唯一索引
来源：http://hz.guannengcc.top/gtqalgiufq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tian-w.cn/gtihyqmovo.html

[Q10] 插入单行
来源：http://hz.redwolf501.top/gtzjgypepr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jianghu66.top/gtuerkugej.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtbqwfpamq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xylfe.cn/gtlrxabdqp.html

[Q12] 插入后取自增 ID
来源：http://hz.dashuyun.cn/gtzalvildq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ehwqpu.com/gtxgvyhiua.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydjk.org.cn/gtpzwpsenw.html

[Q13] 忽略重复插入
来源：http://hz.jqgufenzy.top/gtyimhmrry.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.feifeiyinyue.top/gtcvgmrxzi.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj20258888.top/gtxrdkwxyx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ehwqpu.com/gtzqdvwcju.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gogol.net.cn/gtpelznnod.html

[Q15] 查询全部
来源：http://hz.yj20258.top/gtbzfflsre.html

SELECT * FROM users;
来源：http://hz.zhongyouzk.top/gtgrmdejjp.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtyklzaooz.html

SELECT id, name FROM users;
来源：http://hz.jqgfzy.top/gtsvywfeuh.html

[Q17] 条件查询
来源：http://hz.shanyushiyangkeji.top/gtjjrxprbc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.iojbl.cn/gtjdsgmumb.html

[Q18] 模糊匹配
来源：http://hz.svipenyu.cn/gtwjcgvnhy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gogol.net.cn/gteijkxlah.html

[Q19] 范围查询
来源：http://hz.fzhhl.top/gtrecazyng.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtkvvitibk.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gtfclemjrx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gogol.net.cn/gtsutukkpc.html

[Q21] 空值判断
来源：http://hz.gzhubu.top/gtxshzsaco.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shangyingyoupin.top/gtacexxkef.html

[Q22] 排序
来源：http://hz.yangfankeji.com/gthbvibtlk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guannengcc.top/gtrownutvv.html

[Q23] 分页
来源：http://hz.guowangkeji.top/gtgygrmbtx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cashguo.top/gtdfzrmmtt.html

[Q24] 去重
来源：http://hz.cdnleiting.top/gtfrkuvcnk.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gtqjwowxvy.html

[Q25] 只取前 N 条
来源：http://hz.aibaodan.cn/gtbzuokzhf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxuanxn.top/gtxuicscmi.html

[Q26] 计数
来源：http://hz.ywan-chungtsiang.top/gtjzsztjwo.html

SELECT COUNT(*) FROM users;
来源：http://hz.cdnleiting.top/gtdesgqmol.html

[Q27] 条件计数
来源：http://hz.sufxvd.cn/gtdrlhaxqb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yangfankeji.com/gtbxsrxibr.html

[Q28] 求和与平均
来源：http://hz.cashguo.top/gtrspswatt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gtqwuyhscj.html

[Q29] 最大最小值
来源：http://hz.yuxming.cn/gtqdkerxly.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtjypyppmy.html

[Q30] 分组统计
来源：http://hz.daria6918.cn/gtexydubjv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtlsvyxhon.html

[Q31] 分组后过滤
来源：http://hz.yueranfly.top/gtyausckxi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zycfv.cn/gtyrlnwkpm.html

[Q32] 分组拼接字符串
来源：http://hz.aibaodan.cn/gtefkswovh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtuxdewtkn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zycfv.cn/gttttmyleb.html

[Q33] 多列分组
来源：http://hz.nanxuanxn.top/gttesvrdvq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yvedp.cn/gtshfbivin.html

[Q34] 每组取第一条
来源：http://hz.gzhubu.top/gtaohepksl.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtezmvegae.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gtnrfuztdr.html

) t WHERE rn = 1;
来源：http://hz.jinghuilouyu.cn/gtpuhhgyka.html

[Q35] 内连接
来源：http://hz.cdnleiting.top/gtenfkeefw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtlxnemyxh.html

[Q36] 左连接
来源：http://hz.zycfv.cn/gtklrmcoav.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtbxcnywkz.html

[Q37] 右连接
来源：http://hz.cqqwz.cn/gttfqurdfy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhengqikj.top/gtajftnldm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.redwolf501.top/gtaipkumkd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtyuepodqw.html

[Q39] 自连接（查上下级）
来源：http://hz.316326.xyz/gtczyifphk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtzqennyhm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtferqvnad.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gotoacloud.top/gtfztuxvqx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhaomingkeji.xyz/gttuxmzzgt.html

[Q41] 多表连接
来源：http://hz.zhijiandao.cn/gtjeevcqrj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenjidiqi.icu/gtvjwnyxca.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sufxvd.cn/gthrnlzjxm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuetiantiany.cn/gtgybxkygw.html

[Q42] 连接条件附加过滤
来源：http://hz.dianchejie.cn/gtetdeezzd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangdashe.top/gttbebjzej.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangkeji.top/gtyymauhuc.html

[Q43] 标量子查询
来源：http://hz.52xcode.cn/gtiejmlivr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtsbgguqeh.html

[Q44] IN 子查询
来源：http://hz.nanxuanxn.top/gthhoifgwy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hfpthk.cn/gtctsicixp.html

[Q45] EXISTS 判断存在
来源：http://hz.bjfxy.top/gtcdynuudz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtypxdkdba.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxinkj.top/gtdubxtvuo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jlsjyb.cn/gtljbqnfgp.html

[Q47] 与平均值比较
来源：http://hz.fzhhl.top/gtssaepkoh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gthnuitjvb.html

[Q48] CTE 公用表表达式
来源：http://hz.xuanzx.com/gterhyyeqb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hfpthk.cn/gtucefaoqs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.birdmap.top/gtdfkbrabp.html

[Q49] 更新单行
来源：http://hz.nanxuanxn.top/gtojpncwpd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtggsyfrlz.html

[Q50] 批量更新
来源：http://hz.daria6918.cn/gtpcpkzrjx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangtech.top/gtzrcwkreo.html

[Q51] 用子查询更新
来源：http://hz.yanxiufei.cn/gtjekevezy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtajagjksx.html

[Q52] 删除指定行
来源：http://hz.9152youxi.cn/gtdsodxjvk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangdashe.top/gtipqvwsuk.html

[Q53] 按条件删除
来源：http://hz.svipenyu.cn/gtwzyncpmp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxinkj.top/gtxogprtfg.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtfaspaauz.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtrgzulndr.html

[Q55] 排名（并列占位）
来源：http://hz.guannengcc.top/gtlyjcouxf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuanzx.com/gtmiqktlbk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtnernhvzy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gthqqucrtg.html

[Q57] 行号
来源：http://hz.jiagoushi.top/gtchgrrhrw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yj20258.top/gtbcgijmff.html

[Q58] 累计求和
来源：http://hz.xuanzx.com/gtaxlnoekh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgfzy.top/gtwbsrkipp.html

[Q59] 分组内累计
来源：http://hz.shzxlz.cn/gtmwrdxpcc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tanke756.top/gtejulabzp.html

[Q60] 取上一行 / 下一行
来源：http://hz.ehwqpu.com/gtknngmosv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhongyouzk.top/gtgpbkagho.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.andypj.xyz/gtpxikcrqs.html

[Q61] 移动平均
来源：http://hz.sxryk.cn/gtbnrdoefm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.haohaochexian.top/gtxchkjmic.html

[Q62] 分组占比
来源：http://hz.hnqzz.top/gtpqmalvpv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtwbtuqcsn.html

[Q63] 开启事务
来源：http://hz.birdmap.top/gtugcmpvsf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258.top/gtsririofq.html

[Q64] 提交事务
来源：http://hz.birdmap.top/gtrnoggxkd.html

COMMIT;
来源：http://hz.jyoumei.cn/gtbuqqqlnl.html

[Q65] 回滚事务
来源：http://hz.xuetiantiany.cn/gtglmnacgj.html

ROLLBACK;
来源：http://hz.zhijiandao.cn/gtuofhfhaz.html

[Q66] 行锁查询
来源：http://hz.sxryk.cn/gtuttdgrsc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgufenzy.top/gtvftmvskz.html

[Q67] 设置隔离级别
来源：http://hz.hnqzz.top/gtacdxgovd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtyjjdybdy.html

[Q68] 保存点
来源：http://hz.nanxinkj.top/gtjskrlvoe.html

SAVEPOINT sp1;
来源：http://hz.hysaishi.cn/gtbsyhoely.html

ROLLBACK TO sp1;
来源：http://hz.zhongyouzk.top/gtostsilzg.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtsqcwpuie.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.haohaochexian.top/gtlmlwuyvw.html

[Q70] 更新统计信息
来源：http://hz.zhiwuduotai.top/gtgzboukcx.html

ANALYZE TABLE users;
来源：http://hz.jiagoushi.top/gtolrvazhc.html

[Q71] 查看建表语句
来源：http://hz.gzhubu.top/gtlewwipzi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258.top/gtturzqcmq.html

[Q72] 查看索引
来源：http://hz.hfpthk.cn/gtugocogha.html

SHOW INDEX FROM users;
来源：http://hz.zhengqikj.top/gtvfhefjqc.html

[Q73] 查看表状态
来源：http://hz.sxryk.cn/gtxjkgplql.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.0kj1m.cn/gtpmffcfvk.html

[Q74] 强制使用索引
来源：http://hz.jiagoushi.top/gtsvvmywdj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cdnleiting.top/gttwzfnqza.html

[Q75] 日期格式化
来源：http://hz.snrcjt.cn/gtcbkpstka.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hammf.cn/gtbxhyxtrm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gtadfdiire.html

[Q76] 按天统计
来源：http://hz.zhiwuduotai.top/gtzggmykus.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtemuckqdl.html

[Q77] 时间加减
来源：http://hz.jiagoushi.top/gtqzwqgrxe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dianchejie.cn/gtayciwlmz.html

[Q78] 当前时间
来源：http://hz.gotoacloud.top/gtaargrlvb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hywenlv.cn/gtstvbkote.html

[Q79] 字符串拼接
来源：http://hz.jinqigufen.top/gtzfsjckkq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nwbrower.top/gtdvahkcfh.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gtbapviwvf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.feifeiyinyue.top/gtomysbwpt.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtqgvncxvg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhixingplan.top/gtvnrnnujf.html

[Q82] 字符长度与字节长度
来源：http://hz.zhijiandao.cn/gtidwzdnht.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nwbrower.top/gtlcknykal.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtbwarjpvh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.quarkkingdee.top/gtilfpdlue.html

[Q84] 去除首尾空格
来源：http://hz.jinghuilouyu.cn/gtexurpinh.html

SELECT TRIM(name) FROM users;
来源：http://hz.cucudq.cn/gttcpbjhxd.html

[Q85] 数值取整
来源：http://hz.jqgfzy.top/gtvvcvcrlg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtorgwrkdj.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxuanxn.top/gtkuuduiwp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yanxiufei.cn/gtzwlthnqq.html

[Q87] JSON 字段做条件
来源：http://hz.shuidangran.top/gtjolqsxcw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.havefunace.top/gtseubrikv.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxinkj.top/gtprqcsrbl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tianlin.xyz/gtuqmchgnt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.feifeiyinyue.top/gtaefvhvya.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gtrsucohmy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pycfn.com/gtrefvdjkr.html

[Q90] 生成序号列
来源：http://hz.yuanzhike.top/gtzldmrwzd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuetiantiany.cn/gtxihzthvw.html

================================================================================
来源：http://hz.daria6918.cn/gtykflvuen.html

R. Bash 专题
来源：http://hz.zdqjudy.top/gtydsmlpyn.html

================================================================================
来源：http://hz.52xcode.cn/gtudatgodn.html

[R01] shebang 与严格模式
来源：http://hz.svipenyu.cn/gtpvevqwhj.html

#!/usr/bin/env bash
来源：http://hz.cqqwz.cn/gtwmmslabe.html

set -euo pipefail
来源：http://hz.gzhubu.top/gtjbhwcwzf.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtasppeote.html

name="Tom"; echo "$name"
来源：http://hz.9152youxi.cn/gtiftlyqxa.html

[R03] 只读变量
来源：http://hz.daxiang520.top/gthvafqozp.html

readonly PI=3.14
来源：http://hz.ywan-chungtsiang.top/gtpgzljymk.html

[R04] 位置参数
来源：http://hz.ywan-chungtsiang.top/gtuphlrvjx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xylfe.cn/gtxsbdhrgx.html

[R05] 参数默认值
来源：http://hz.316326.xyz/gtplcpfvmt.html

name="${1:-default}"
来源：http://hz.tian-w.cn/gtpxklidpe.html

[R06] 判断命令是否存在
来源：http://hz.sxryk.cn/gtiaangsjz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daria6918.cn/gtlpqdaieq.html

[R07] if 判断文件
来源：http://hz.nwbrower.top/gtwlfheiqj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shuidangran.top/gtfhukgwkg.html

[R08] 数值比较
来源：http://hz.mhx1999.top/gtbuonmziq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhoulong.xyz/gtnstfwuxi.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtuogcsipy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnqzz.top/gttwscwocw.html

[R10] 正则匹配
来源：http://hz.ywan-chungtsiang.top/gtyzkcfvsd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtuuhvgtws.html

[R11] case 多分支
来源：http://hz.zhaomingkeji.xyz/gtoegcyvjf.html

case "$1" in
来源：http://hz.aibaodan.cn/gteudfckuc.html

start) echo "启动" ;;
来源：http://hz.cdnleiting.top/gtzkhxubeb.html

stop)  echo "停止" ;;
来源：http://hz.jianghu66.top/gttapkpiie.html

*)     echo "未知命令" ;;
来源：http://hz.shuidangran.top/gtvwzlmuxz.html

esac
来源：http://hz.52xcode.cn/gtixubsdtu.html

[R12] for 遍历文件
来源：http://hz.sysykeji.top/gtbmohnrjh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cdnleiting.top/gthowmievy.html

[R13] for 计数循环
来源：http://hz.cqqwz.cn/gtwvewoxlg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtnpguangw.html

[R14] C 风格 for
来源：http://hz.fengsongda.top/gtqjkbrrss.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtflaqkuuv.html

[R15] while 逐行读文件
来源：http://hz.nanxinkj.top/gtvwymuips.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.mhx1999.top/gtcpfuwjbn.html

[R16] until 等待条件
来源：http://hz.bjfxy.top/gttlzeldnt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jiagoushi.top/gtujbxndwm.html

[R17] 数组定义与取值
来源：http://hz.316326.xyz/gtbbskajwe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shangyingyoupin.top/gthcrftrxd.html

[R18] 遍历数组
来源：http://hz.bjfxy.top/gtekpylrrq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtclsxlfdl.html

[R19] 数组长度
来源：http://hz.yj20258888.top/gtnpobidez.html

echo "${#arr[@]}"
来源：http://hz.xziqi.cn/gtgbnmzguw.html

[R20] 关联数组（字典）
来源：http://hz.hnxiangtu.top/gtlqszqawm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yongpay.top/gtrneowwol.html

[R21] 字符串长度
来源：http://hz.hysaishi.cn/gttjpisjvm.html

echo "${#s}"
来源：http://hz.ywan-chungtsiang.top/gtujlevmsx.html

[R22] 截取子串
来源：http://hz.redwolf501.top/gtrcrbkpzl.html

echo "${s:0:5}"
来源：http://hz.wangshuangyany.cn/gtqtqhupfx.html

[R23] 字符串替换
来源：http://hz.yongpay.top/gtusjzljpg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gtomsbnmzo.html

[R24] 大小写转换
来源：http://hz.jinqigfzy.top/gtgxjyfjqd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigfzy.top/gtpukutyjw.html

[R25] 去后缀 / 去前缀
来源：http://hz.cdnleiting.top/gtybvoeead.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hfpthk.cn/gtrahmrroj.html

[R26] 命令替换
来源：http://hz.dianchejie.cn/gtkhqkxyga.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gtwtpnspzi.html

[R27] 算术展开
来源：http://hz.ybcxt.top/gtnzvesboy.html

echo $((1 + 2 * 3))
来源：http://hz.tianlin.xyz/gtjslmrtil.html

[R28] 浮点运算
来源：http://hz.sysykeji.top/gtqeitwyvi.html

echo "scale=2; 10/3" | bc
来源：http://hz.zdqjudy.top/gtnwppepop.html

[R29] 定义函数
来源：http://hz.kuanghao11.cn/gtskaxlxdr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jiagoushi.top/gttumithes.html

[R30] 函数返回状态码
来源：http://hz.cashguo.top/gtvnsioygf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tian-w.cn/gtflxsbyzc.html

[R31] 局部变量
来源：http://hz.sweek.top/gtzuepwbfg.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj202588.top/gtfecopjip.html

[R32] 参数个数校验
来源：http://hz.shzxlz.cn/gtmfdkperx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gtkpuxonsy.html

[R33] 捕获错误并提示行号
来源：http://hz.cdnleiting.top/gtdqpxwdys.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258888.top/gtzxbhmkms.html

[R34] 退出时清理
来源：http://hz.ydzc1.top/gtypvcigoj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtokfhhwfi.html

[R35] 后台执行并等待
来源：http://hz.sxryk.cn/gtorstgwwl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtiladmjvx.html

[R36] 并发执行多个任务
来源：http://hz.gaohongyu789.top/gtcalkuwzu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tianlin.xyz/gtpjablzvq.html

[R37] 把输出赋给变量
来源：http://hz.9152youxi.cn/gtrsxwnpva.html

files=$(ls -1)
来源：http://hz.gzhubu.top/gtvtstfcca.html

[R38] 管道串联
来源：http://hz.hysaishi.cn/gtfsexegfs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jyoumei.cn/gtibktmohn.html

[R39] 重定向标准输出与错误
来源：http://hz.cheryme.top/gtxnfmiura.html

cmd > out.log 2>&1
来源：http://hz.chenjidiqi.icu/gtxxgdgudd.html

[R40] 追加写日志
来源：http://hz.vqdsnc.cn/gttheoftam.html

echo "log" >> out.log
来源：http://hz.9152youxi.cn/gtfexfnvce.html

[R41] 丢弃输出
来源：http://hz.sysykeji.top/gtwcpismfh.html

cmd >/dev/null 2>&1
来源：http://hz.zhijiandao.cn/gtrzsevwql.html

[R42] 输入重定向
来源：http://hz.ydzc1.top/gtuimqczph.html

wc -l < a.txt
来源：http://hz.jqgfzy.top/gtviccpaiw.html

[R43] 按名字查找文件
来源：http://hz.yuxming.cn/gtvnelulxj.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtemnpqexj.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gtoojcdovk.html

find . -mtime -7 -type f
来源：http://hz.haohaochexian.top/gtrawhmpjz.html

[R45] 批量删除
来源：http://hz.xinyue.icu/gtyjzrxftz.html


<!-- 参考信息 -->