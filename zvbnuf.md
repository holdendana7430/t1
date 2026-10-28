代发 wailian999

CREATE TABLE users (
来源：http://hz.jqgufenzy.top/gteclaknyv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtrqtdchub.html

name VARCHAR(50) NOT NULL,
来源：http://hz.snrcjt.cn/gttsqkaxec.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj20258.top/gtimbujagj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenjidiqi.icu/gtafivugwe.html

);
来源：http://hz.sweek.top/gtcgnhudgs.html

[Q02] 创建带外键的表
来源：http://hz.hysaishi.cn/gthrsnoinq.html

CREATE TABLE orders (
来源：http://hz.svipenyu.cn/gtibfwkvwd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtujkhkimt.html

user_id INT NOT NULL,
来源：http://hz.cheryme.top/gtqzooczky.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gtzetqgkxo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuanzhike.top/gtswfjcwru.html

);
来源：http://hz.hysaishi.cn/gtajpcxscl.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtaqskbbnl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hysaishi.cn/gtnvhfhauf.html

[Q04] 修改列类型
来源：http://hz.cucudq.cn/gtpyxdqhlm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yanxiufei.cn/gtissbkvpk.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtqftoqcmd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtacbovwtm.html

[Q06] 删除列
来源：http://hz.ivvv.top/gtbeavsilz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnxiangtu.top/gtcghlxvhn.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gtjperpsfl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dashuyun.cn/gtjrunaaiz.html

[Q08] 创建普通索引
来源：http://hz.yongpay.top/gtuiaxfzjc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gzhubu.top/gtapngadhu.html

[Q09] 创建唯一索引
来源：http://hz.xylfe.cn/gtnepgkysd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuanzhike.top/gtcnzmgtdi.html

[Q10] 插入单行
来源：http://hz.sweek.top/gtuxsrpekt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sufxvd.cn/gteazwzlkr.html

[Q11] 一次插入多行
来源：http://hz.yanxiufei.cn/gtolscjxcf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuanzx.com/gtaynxubhj.html

[Q12] 插入后取自增 ID
来源：http://hz.tanke756.top/gtqdlyeims.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.0kj1m.cn/gtjoclxkzw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yvedp.cn/gtyanmkuyi.html

[Q13] 忽略重复插入
来源：http://hz.yuxming.cn/gtxcmkeiqa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhiwuduotai.top/gtjfnvtqfm.html

[Q14] 存在则更新（upsert）
来源：http://hz.quarkkingdee.top/gtqlwcqpdb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenjidiqi.icu/gtjlnjjgvm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cdnleiting.top/gtrmnjpilh.html

[Q15] 查询全部
来源：http://hz.redwolf501.top/gtdpofobim.html

SELECT * FROM users;
来源：http://hz.xylfe.cn/gtkbhjkrjk.html

[Q16] 查询指定列
来源：http://hz.sxryk.cn/gtfdipkxiv.html

SELECT id, name FROM users;
来源：http://hz.yj20258.top/gtamzpsltn.html

[Q17] 条件查询
来源：http://hz.ppjwa.cn/gtkkzvrnid.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gtthdepttt.html

[Q18] 模糊匹配
来源：http://hz.c1oappe.top/gtwkaqbmys.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hysaishi.cn/gtvycrzkzl.html

[Q19] 范围查询
来源：http://hz.yonumen.top/gtewbhwjgu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtiwpmarqc.html

[Q20] IN 列表
来源：http://hz.zhixingplan.top/gtmdpakjzw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj20258888.top/gtuzjggfzr.html

[Q21] 空值判断
来源：http://hz.yueranfly.top/gtbdotkrtc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tian-w.cn/gtwuaxqaxg.html

[Q22] 排序
来源：http://hz.snrcjt.cn/gtokhcjfao.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydjk.org.cn/gtjganneqf.html

[Q23] 分页
来源：http://hz.xuetiantiany.cn/gtcyiizelp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hywenlv.cn/gtdyxasdxn.html

[Q24] 去重
来源：http://hz.gzhubu.top/gtuagijmdv.html

SELECT DISTINCT city FROM users;
来源：http://hz.316326.xyz/gtkwpulwwt.html

[Q25] 只取前 N 条
来源：http://hz.nanxuanxn.top/gtoggmgqec.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hysaishi.cn/gtatnudcfq.html

[Q26] 计数
来源：http://hz.pycfn.com/gtxdtgxifl.html

SELECT COUNT(*) FROM users;
来源：http://hz.52xcode.cn/gtosicpavj.html

[Q27] 条件计数
来源：http://hz.9152youxi.cn/gtmdcfhagl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangkeji.top/gtkiluymzl.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtyczlfxkf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gteoqysiqy.html

[Q29] 最大最小值
来源：http://hz.zhoulong.xyz/gtwqpdzgpj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtmulmfsyp.html

[Q30] 分组统计
来源：http://hz.yueranfly.top/gtklujuwjf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtvkotjfzd.html

[Q31] 分组后过滤
来源：http://hz.zhongyouzk.top/gtcrtixqrj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yangfankeji.com/gtostnwfax.html

[Q32] 分组拼接字符串
来源：http://hz.xylfe.cn/gtcboxwkzh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtmetebyjk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtoqdnhtue.html

[Q33] 多列分组
来源：http://hz.aibaodan.cn/gthiczyobs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtthdkjjez.html

[Q34] 每组取第一条
来源：http://hz.daria6918.cn/gtetenaaaj.html

SELECT * FROM (
来源：http://hz.daria6918.cn/gtmcnjwwsw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxuanxn.top/gtipzaujwp.html

) t WHERE rn = 1;
来源：http://hz.yj202588.top/gtktmxdvtf.html

[Q35] 内连接
来源：http://hz.yj20258.top/gtbztwxslj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtnvprjftp.html

[Q36] 左连接
来源：http://hz.chenzaomai.com/gtptcjwxog.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jiagoushi.top/gtfslfkhjh.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gtgjboiipq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258.top/gtyzaujdzr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.iojbl.cn/gtjijjartc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhengqikj.top/gtvxjtecgz.html

[Q39] 自连接（查上下级）
来源：http://hz.sufxvd.cn/gtdrxborew.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pengpengdd.cyou/gtgnzrgjuz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yanxiufei.cn/gtlfngjbed.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.snrcjt.cn/gtpjjtxsbx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jiagoushi.top/gtjtsvyydp.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtrcmnnouz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daxiang520.top/gtzqroqibb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xylfe.cn/gtbqcokhbc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.dianchejie.cn/gtipejkbhd.html

[Q42] 连接条件附加过滤
来源：http://hz.jinghuilouyu.cn/gtndqkbtmq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sysykeji.top/gtcwtifmll.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daria6918.cn/gtwqeljkam.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtilalzvxk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtdyaltnvk.html

[Q44] IN 子查询
来源：http://hz.feifeiyinyue.top/gtlygmbker.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pengpengdd.cyou/gtyswkjvjh.html

[Q45] EXISTS 判断存在
来源：http://hz.redwolf501.top/gtrtvuekdm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtinznoitp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangkeji.top/gtijbvhooc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtzwfcftkk.html

[Q47] 与平均值比较
来源：http://hz.jinghuilouyu.cn/gtkltakeco.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gthrhfiabp.html

[Q48] CTE 公用表表达式
来源：http://hz.zhaomingkeji.xyz/gtqziukiiq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ybcxt.top/gtsjteqnjx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cqqwz.cn/gtohqacrez.html

[Q49] 更新单行
来源：http://hz.guowangkeji.top/gtonhyhtqc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ivvv.top/gtyzgrvoup.html

[Q50] 批量更新
来源：http://hz.pengpengdd.cyou/gtzwxlacki.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guannengcc.top/gtgdjizfqa.html

[Q51] 用子查询更新
来源：http://hz.iojbl.cn/gtvszwtkgs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenzaomai.com/gtgkybgdbn.html

[Q52] 删除指定行
来源：http://hz.kuanghao11.cn/gtygedfcfh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.mhx1999.top/gtrrkihnyf.html

[Q53] 按条件删除
来源：http://hz.wangdashe.top/gtlfimxbgs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuetiantiany.cn/gtwxotakhx.html

[Q54] 清空表
来源：http://hz.ydzc1.top/gtdxbmljvr.html

TRUNCATE TABLE logs;
来源：http://hz.mhx1999.top/gtwjhdfaez.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtavkoqyrv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.52xcode.cn/gttwachpwv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenlongwang.top/gtzlunfhrd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj202588.top/gtlxclxcyj.html

[Q57] 行号
来源：http://hz.iojbl.cn/gtcyytyygl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.316326.xyz/gtvjyjgjsp.html

[Q58] 累计求和
来源：http://hz.gzhubu.top/gtzdyfihnv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuanzx.com/gtvzyzeknu.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtzhcsedao.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hysaishi.cn/gtemsarijd.html

[Q60] 取上一行 / 下一行
来源：http://hz.havefunace.top/gtyfaszzdg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtoqdjabdr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigufen.top/gtrlcdedwp.html

[Q61] 移动平均
来源：http://hz.snrcjt.cn/gteoudeqwo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtdrdagbfd.html

[Q62] 分组占比
来源：http://hz.hnqzz.top/gtsbsqqpbq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtzeemkrnm.html

[Q63] 开启事务
来源：http://hz.yuanzhike.top/gtterljvfw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtmeurqtfr.html

[Q64] 提交事务
来源：http://hz.hywenlv.cn/gtkdvhujqq.html

COMMIT;
来源：http://hz.ppjwa.cn/gtuqifxnvs.html

[Q65] 回滚事务
来源：http://hz.xziqi.cn/gtzgdpbyfq.html

ROLLBACK;
来源：http://hz.jianghu66.top/gtejhifrso.html

[Q66] 行锁查询
来源：http://hz.nanxuanxn.top/gtsnceqzhp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sysykeji.top/gtpmfbjmqs.html

[Q67] 设置隔离级别
来源：http://hz.bjfxy.top/gthabgyzlm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gtwdfvbbcc.html

[Q68] 保存点
来源：http://hz.birdmap.top/gtbjvguyvo.html

SAVEPOINT sp1;
来源：http://hz.svipenyu.cn/gtebtdelvk.html

ROLLBACK TO sp1;
来源：http://hz.haohaochexian.top/gthgdriuhe.html

[Q69] 查看执行计划
来源：http://hz.9152youxi.cn/gtmhussrov.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fengsongda.top/gtiwzfwzph.html

[Q70] 更新统计信息
来源：http://hz.zdqjudy.top/gtaaoykzwy.html

ANALYZE TABLE users;
来源：http://hz.ydjk.org.cn/gteczeogvx.html

[Q71] 查看建表语句
来源：http://hz.jinyuanbaomall.cn/gtawscqbdw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shzxlz.cn/gtzecpjgsy.html

[Q72] 查看索引
来源：http://hz.yongpay.top/gtldyzjrat.html

SHOW INDEX FROM users;
来源：http://hz.gaohongyu789.top/gtyayypvgr.html

[Q73] 查看表状态
来源：http://hz.meibo888.top/gtunnbzxha.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sxryk.cn/gtxzcprdri.html

[Q74] 强制使用索引
来源：http://hz.chenjidiqi.icu/gttphxrlaj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gtrzuqonbf.html

[Q75] 日期格式化
来源：http://hz.zhengqikj.top/gtvcvvkvih.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.meibo888.top/gtvggnrchm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangkeji.top/gtmoguorsd.html

[Q76] 按天统计
来源：http://hz.jyoumei.cn/gtjdnsfmun.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sxryk.cn/gtjyshecng.html

[Q77] 时间加减
来源：http://hz.yangfankeji.com/gtymrceyoy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gotoacloud.top/gthywcujef.html

[Q78] 当前时间
来源：http://hz.hysaishi.cn/gtbknrujbl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gtphripmlm.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gtumsvqqpl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.smart0.xyz/gtnxbivfem.html

[Q80] 字符串截取
来源：http://hz.yongpay.top/gtnsahpism.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yvedp.cn/gtpdqdnthk.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gtaxagwtty.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.c1oappe.top/gtvkreirsi.html

[Q82] 字符长度与字节长度
来源：http://hz.jyoumei.cn/gtdfjrckvu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.snrcjt.cn/gtncukmrur.html

[Q83] 大小写转换
来源：http://hz.daxiang520.top/gtwszvkeev.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daxiang520.top/gtgbcwtusd.html

[Q84] 去除首尾空格
来源：http://hz.kuanghao11.cn/gtvrkpvovb.html

SELECT TRIM(name) FROM users;
来源：http://hz.daxiang520.top/gtcbfozkba.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtufbgcgqd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sysykeji.top/gtvwermcjt.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gtddlxgqkx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fzhhl.top/gtmrlnnegt.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gtpguzrbkn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gaohongyu789.top/gtvmyetkfq.html

[Q88] 行转列（条件聚合）
来源：http://hz.mhx1999.top/gtxlephuga.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yanxiufei.cn/gtikfynbqx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sweek.top/gtibcpuasl.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gtvtdxonpm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gtsdmrtfxe.html

[Q90] 生成序号列
来源：http://hz.yj20258.top/gtopshfwnh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydjk.org.cn/gthfpbhmsp.html

================================================================================
来源：http://hz.yj20258.top/gtyxgcurzc.html

R. Bash 专题
来源：http://hz.meibo888.top/gttsqzencq.html

================================================================================
来源：http://hz.sweek.top/gtxpuyaunv.html

[R01] shebang 与严格模式
来源：http://hz.yj20258.top/gtzduajvfb.html

#!/usr/bin/env bash
来源：http://hz.316326.xyz/gtvkznxpkl.html

set -euo pipefail
来源：http://hz.redwolf501.top/gtqokccgmy.html

[R02] 变量赋值与使用
来源：http://hz.hammf.cn/gtiahbvsha.html

name="Tom"; echo "$name"
来源：http://hz.0kj1m.cn/gtvbociavy.html

[R03] 只读变量
来源：http://hz.nanxinkj.top/gtafjhnoml.html

readonly PI=3.14
来源：http://hz.quarkkingdee.top/gtdejbqccp.html

[R04] 位置参数
来源：http://hz.jyoumei.cn/gtzqoxbobv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yanxiufei.cn/gtdaxutqmk.html

[R05] 参数默认值
来源：http://hz.zdqjudy.top/gtbbgnoclo.html

name="${1:-default}"
来源：http://hz.chenlongwang.top/gtpjkvtqce.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtecuovmgy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ivvv.top/gtbuqizkgz.html

[R07] if 判断文件
来源：http://hz.guowangkeji.top/gtiipufiht.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ppjwa.cn/gtqrmpwgjx.html

[R08] 数值比较
来源：http://hz.xuetiantiany.cn/gtvxdahzqv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.bjfxy.top/gtzxzjlssb.html

[R09] 字符串比较
来源：http://hz.yanxiufei.cn/gtqvppyxyq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zdqjudy.top/gtpjcqdmap.html

[R10] 正则匹配
来源：http://hz.dashuyun.cn/gtpdsjfgql.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxuanxn.top/gtvwvrcmma.html

[R11] case 多分支
来源：http://hz.guannengcc.top/gtlqdyqrlg.html

case "$1" in
来源：http://hz.zhijiandao.cn/gtviwgkuzk.html

start) echo "启动" ;;
来源：http://hz.yj20258888.top/gtrwnqrwbn.html

stop)  echo "停止" ;;
来源：http://hz.gogol.net.cn/gtndgkekqp.html

*)     echo "未知命令" ;;
来源：http://hz.52xcode.cn/gtfaunbfvg.html

esac
来源：http://hz.shangyingyoupin.top/gthpncxayp.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gtqbjbomuo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.feifeiyinyue.top/gtbyrpnrot.html

[R13] for 计数循环
来源：http://hz.dianchejie.cn/gttvttchcb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtrpjeunen.html

[R14] C 风格 for
来源：http://hz.jinyuanbaomall.cn/gtuccwmvee.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pycfn.com/gthcwkpkap.html

[R15] while 逐行读文件
来源：http://hz.hnqzz.top/gtroxcqrnc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangshuangyany.cn/gtluzygylg.html

[R16] until 等待条件
来源：http://hz.hfpthk.cn/gtgvvxcxik.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhoulong.xyz/gtxzssybvn.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtjhmszbmg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hfpthk.cn/gtrnorqexc.html

[R18] 遍历数组
来源：http://hz.gaohongyu789.top/gtsciiztcs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtmoizvodo.html

[R19] 数组长度
来源：http://hz.jinyuanbaomall.cn/gtjxrjofbg.html

echo "${#arr[@]}"
来源：http://hz.jqgfzy.top/gtwytetmuc.html

[R20] 关联数组（字典）
来源：http://hz.tian-w.cn/gtlflgengf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xinyue.icu/gtuadkjwdp.html

[R21] 字符串长度
来源：http://hz.ydjk.org.cn/gtkwxzimbt.html

echo "${#s}"
来源：http://hz.zhijiandao.cn/gtpdqaanhk.html

[R22] 截取子串
来源：http://hz.ybcxt.top/gtzejtadle.html

echo "${s:0:5}"
来源：http://hz.shanyushiyangtech.top/gtmopyxvvg.html

[R23] 字符串替换
来源：http://hz.zhijiandao.cn/gtwsgougou.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhiwuduotai.top/gtbrqfnwjt.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtwaxcnfbc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zdqjudy.top/gtibqnxvfv.html

[R25] 去后缀 / 去前缀
来源：http://hz.sweek.top/gtrukirexx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.bjfxy.top/gtdvedsgfy.html

[R26] 命令替换
来源：http://hz.yanxiufei.cn/gtvxoetvkn.html

now=$(date +%F); echo "$now"
来源：http://hz.52xcode.cn/gtangsrvwg.html

[R27] 算术展开
来源：http://hz.yanxiufei.cn/gtzmvopwht.html

echo $((1 + 2 * 3))
来源：http://hz.quarkkingdee.top/gtfcggnbmr.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gthurniteh.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtskjzeqzp.html

[R29] 定义函数
来源：http://hz.yuxming.cn/gtuoxgjvxv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangshuangyany.cn/gtozzsfrbh.html

[R30] 函数返回状态码
来源：http://hz.hongshengwenyu.top/gtmlrtxiwc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cdnleiting.top/gtandddimj.html

[R31] 局部变量
来源：http://hz.zycfv.cn/gtsqgmeqby.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhongyouzk.top/gtyycnevdh.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtvixemlbp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.redwolf501.top/gtgecfikef.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtsymngztm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinyuanbaomall.cn/gtlrdwhimo.html

[R34] 退出时清理
来源：http://hz.andypj.xyz/gtfyjilkas.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtccqquzxq.html

[R35] 后台执行并等待
来源：http://hz.hnxiangtu.top/gtivhobaiu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aibaodan.cn/gtufxeuqiz.html

[R36] 并发执行多个任务
来源：http://hz.redwolf501.top/gtlwiyegik.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ppjwa.cn/gtapqsqxzd.html

[R37] 把输出赋给变量
来源：http://hz.jqgufenzy.top/gtswncbrjw.html

files=$(ls -1)
来源：http://hz.xuanzx.com/gtjiratozi.html

[R38] 管道串联
来源：http://hz.xinyue.icu/gtaeqtxqdi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.9152youxi.cn/gtyvvwxtho.html

[R39] 重定向标准输出与错误
来源：http://hz.cheryme.top/gtrardldkq.html

cmd > out.log 2>&1
来源：http://hz.gotoacloud.top/gtqiyuzsoj.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gtvwotybrn.html

echo "log" >> out.log
来源：http://hz.chenzaomai.com/gtoepyollu.html

[R41] 丢弃输出
来源：http://hz.hysaishi.cn/gthdnwmdnd.html

cmd >/dev/null 2>&1
来源：http://hz.dashuyun.cn/gtpqzjolvb.html

[R42] 输入重定向
来源：http://hz.mhx1999.top/gtyjyduahl.html

wc -l < a.txt
来源：http://hz.chenlongwang.top/gtziilkava.html

[R43] 按名字查找文件
来源：http://hz.0kj1m.cn/gtlyzvfyjv.html

find . -name "*.log" -type f
来源：http://hz.tanke756.top/gtzkwfxhov.html

[R44] 按修改时间查找
来源：http://hz.daxiang520.top/gtbeprovii.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gtnyszkidk.html

[R45] 批量删除
来源：http://hz.sysykeji.top/gtyvlyhusg.html


<!-- 参考信息 -->