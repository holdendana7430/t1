代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigfzy.top/gtjeivcuxz.html

user_id INT NOT NULL,
来源：http://hz.kuanghao11.cn/gtvhdmjofs.html

amount DECIMAL(10, 2),
来源：http://hz.52xcode.cn/gtoajcgvoz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.52xcode.cn/gtjggqaymh.html

);
来源：http://hz.cdnleiting.top/gtuzgjdfbt.html

[Q03] 增加列
来源：http://hz.yj202588.top/gtjpynamvb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shuidangran.top/gtwdrodfdx.html

[Q04] 修改列类型
来源：http://hz.dianchejie.cn/gttqrhnzks.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yanxiufei.cn/gtpcmdtmdl.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtzlnbfcms.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xziqi.cn/gtvaqrojtm.html

[Q06] 删除列
来源：http://hz.redwolf501.top/gtiffrmozm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.tianlin.xyz/gtfeuwyrzx.html

[Q07] 删除表
来源：http://hz.xziqi.cn/gtwwthruvo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xziqi.cn/gtcbouliej.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtovuvtzuc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.smart0.xyz/gtuxzmivvf.html

[Q09] 创建唯一索引
来源：http://hz.guowangkeji.top/gtyqecozwl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ivvv.top/gtalrudgzp.html

[Q10] 插入单行
来源：http://hz.chenjidiqi.icu/gtlekgcxfw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.andypj.xyz/gthvcsiiud.html

[Q11] 一次插入多行
来源：http://hz.cashguo.top/gtiubcmgom.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhaomingkeji.xyz/gtzccigifu.html

[Q12] 插入后取自增 ID
来源：http://hz.ywan-chungtsiang.top/gtxgyiaqrt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gtmtbjeght.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jiagoushi.top/gtmqyurevz.html

[Q13] 忽略重复插入
来源：http://hz.iojbl.cn/gtpfnodgqb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shangyingyoupin.top/gtjrvyuqdb.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtyofvjyez.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xingfuxueyuan.xyz/gtuzuvjlwt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuetiantiany.cn/gtftrdieoj.html

[Q15] 查询全部
来源：http://hz.feifeiyinyue.top/gtfgnocnyq.html

SELECT * FROM users;
来源：http://hz.chenjidiqi.icu/gtqprtvetb.html

[Q16] 查询指定列
来源：http://hz.yvedp.cn/gtriamdokw.html

SELECT id, name FROM users;
来源：http://hz.sufxvd.cn/gtmqpiynlz.html

[Q17] 条件查询
来源：http://hz.aibaodan.cn/gtubckeqtg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxuanxn.top/gtoytnvboz.html

[Q18] 模糊匹配
来源：http://hz.jyoumei.cn/gtmhigdnzq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.feifeiyinyue.top/gtwpaewqyu.html

[Q19] 范围查询
来源：http://hz.yuanzhike.top/gtbofiiion.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhiwuduotai.top/gtacqcofsf.html

[Q20] IN 列表
来源：http://hz.zycfv.cn/gtjumgnstv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shuidangran.top/gtkzunomos.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtknvustxj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.iojbl.cn/gtikrgnjxy.html

[Q22] 排序
来源：http://hz.xinyue.icu/gtlpejakba.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtukzmkdgc.html

[Q23] 分页
来源：http://hz.cqqwz.cn/gtnrfxufyv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gzhubu.top/gtfttimnzl.html

[Q24] 去重
来源：http://hz.tian-w.cn/gthzvttutl.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gtmlcbvzwy.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtnmpqmuhv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hammf.cn/gtdvgxbprd.html

[Q26] 计数
来源：http://hz.yuxming.cn/gterpmuouz.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtzjgdieok.html

[Q27] 条件计数
来源：http://hz.pengpengdd.cyou/gtmgmxphfx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtshxsnhue.html

[Q28] 求和与平均
来源：http://hz.gogol.net.cn/gtzufhvubc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtqcbclmws.html

[Q29] 最大最小值
来源：http://hz.tian-w.cn/gtbzhljkmr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gaohongyu789.top/gtzaqbuamb.html

[Q30] 分组统计
来源：http://hz.ybcxt.top/gtrxvkmaxd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtwxtsbamc.html

[Q31] 分组后过滤
来源：http://hz.tanke756.top/gtbsmivodp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yonumen.top/gtznjvyhih.html

[Q32] 分组拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtktushfpf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtdgnyacjg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ppjwa.cn/gtfomqbanl.html

[Q33] 多列分组
来源：http://hz.chenzaomai.com/gthdbfskpl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ehwqpu.com/gtnmclidda.html

[Q34] 每组取第一条
来源：http://hz.zhaomingkeji.xyz/gtxrdhnhko.html

SELECT * FROM (
来源：http://hz.jqgufenzy.top/gtzmxkkrme.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daxiang520.top/gtgyfwvjpq.html

) t WHERE rn = 1;
来源：http://hz.cdnleiting.top/gtjjpmwuya.html

[Q35] 内连接
来源：http://hz.xylfe.cn/gtujlzpmex.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigufen.top/gtnefznuvu.html

[Q36] 左连接
来源：http://hz.chenlongwang.top/gtzpcinole.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtijdifuqb.html

[Q37] 右连接
来源：http://hz.c1oappe.top/gtxinbukoz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.andypj.xyz/gtvpnqdqmh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ppjwa.cn/gtoucsesla.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zdqjudy.top/gtiivnteif.html

[Q39] 自连接（查上下级）
来源：http://hz.pycfn.com/gtpnxfwqwv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tianlin.xyz/gtubsftenj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hongshengwenyu.top/gthcwfeusl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gtkqsrhrou.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guowangkeji.top/gtzyfhyvku.html

[Q41] 多表连接
来源：http://hz.aibaodan.cn/gtvtkswryg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hysaishi.cn/gtigskqzer.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgufenzy.top/gtsjfppanq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinghuilouyu.cn/gtunjoeomw.html

[Q42] 连接条件附加过滤
来源：http://hz.cdnleiting.top/gtkwzcaznm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.snrcjt.cn/gtrpcpglii.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jlsjyb.cn/gtfnlplbwa.html

[Q43] 标量子查询
来源：http://hz.bjfxy.top/gtzxsksbvm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ybcxt.top/gtawrhuxju.html

[Q44] IN 子查询
来源：http://hz.zhaomingkeji.xyz/gtgxqujqjb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtzcvareda.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gtvczdletx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtqxjiooot.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhoulong.xyz/gtrknjcijt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ppjwa.cn/gtpancugdn.html

[Q47] 与平均值比较
来源：http://hz.kuanghao11.cn/gttuukoqxd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gtkdjkeswa.html

[Q48] CTE 公用表表达式
来源：http://hz.shangyingyoupin.top/gtyjmqeeyj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuetiantiany.cn/gtqiuaxwcn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pycfn.com/gtpqrvhrec.html

[Q49] 更新单行
来源：http://hz.xuanzx.com/gtnhljzbqj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangdashe.top/gtpmsotbcw.html

[Q50] 批量更新
来源：http://hz.cucudq.cn/gtozhdlzkw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.bjfxy.top/gttafkijzx.html

[Q51] 用子查询更新
来源：http://hz.sxryk.cn/gtovqsthxa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtcwhngcrj.html

[Q52] 删除指定行
来源：http://hz.iojbl.cn/gtazjluppo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtujelndzl.html

[Q53] 按条件删除
来源：http://hz.hammf.cn/gtschotvva.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tanke756.top/gtndcuceod.html

[Q54] 清空表
来源：http://hz.cheryme.top/gtldhjttzf.html

TRUNCATE TABLE logs;
来源：http://hz.sxryk.cn/gtzgmcenjq.html

[Q55] 排名（并列占位）
来源：http://hz.zycfv.cn/gtxdqtnwgi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shuidangran.top/gttzcxwzdw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhijiandao.cn/gtleuizxou.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nwbrower.top/gtgygvcpgi.html

[Q57] 行号
来源：http://hz.cucudq.cn/gttsalpqlr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenjidiqi.icu/gtyqvzsyuc.html

[Q58] 累计求和
来源：http://hz.yvedp.cn/gtlkbnxjrg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtayqhfkxy.html

[Q59] 分组内累计
来源：http://hz.jqgfzy.top/gtcbcdhbvz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jlsjyb.cn/gtvsjhoqse.html

[Q60] 取上一行 / 下一行
来源：http://hz.ehwqpu.com/gtrwqzznor.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xylfe.cn/gticdrbrfm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tanke756.top/gtzmlngzum.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtuyipfrkb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shuidangran.top/gterawpwch.html

[Q62] 分组占比
来源：http://hz.sufxvd.cn/gtlwgmwnvm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtqibhkbsp.html

[Q63] 开启事务
来源：http://hz.zhongyouzk.top/gtddleneie.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ybcxt.top/gtlenbqvpo.html

[Q64] 提交事务
来源：http://hz.zhiwuduotai.top/gtlxjljdbx.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtnxvcsdrx.html

[Q65] 回滚事务
来源：http://hz.wangshuangyany.cn/gtrjlqstcb.html

ROLLBACK;
来源：http://hz.chenjidiqi.icu/gtlztdtyhg.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gtjylaeyok.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fzhhl.top/gtucdrglcf.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtssninnsc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xinyue.icu/gtqfvxriyt.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gtimeuigyk.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtpijexwlq.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gtopqxjynq.html

[Q69] 查看执行计划
来源：http://hz.nwbrower.top/gtxdpplikv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ydjk.org.cn/gttxswgiea.html

[Q70] 更新统计信息
来源：http://hz.xziqi.cn/gtbgnsiccb.html

ANALYZE TABLE users;
来源：http://hz.xinyue.icu/gtoybxbeqv.html

[Q71] 查看建表语句
来源：http://hz.sysykeji.top/gteasuxhan.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pengpengdd.cyou/gthtzfppbc.html

[Q72] 查看索引
来源：http://hz.316326.xyz/gtrqkpgmpw.html

SHOW INDEX FROM users;
来源：http://hz.jinyuanbaomall.cn/gtuhkjltrk.html

[Q73] 查看表状态
来源：http://hz.hnqzz.top/gtbfokmmny.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gtkvpgrjjt.html

[Q74] 强制使用索引
来源：http://hz.hongshengwenyu.top/gtbhxhcwsl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhaomingkeji.xyz/gtvrwutnxz.html

[Q75] 日期格式化
来源：http://hz.sxryk.cn/gtdtvlzehr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gzhubu.top/gteaolveet.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guannengcc.top/gtpuftrfgl.html

[Q76] 按天统计
来源：http://hz.tanke756.top/gtuognuwdm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenzaomai.com/gtrpgilxfx.html

[Q77] 时间加减
来源：http://hz.daxiang520.top/gtzsplreqj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cdnleiting.top/gtakgxunpt.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gthcuyrgyk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shzxlz.cn/gtjbnsitqr.html

[Q79] 字符串拼接
来源：http://hz.zhiwuduotai.top/gtxtfvrpxe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangtech.top/gtuqjjjxfc.html

[Q80] 字符串截取
来源：http://hz.sxryk.cn/gtvywrfpzr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ybcxt.top/gtmjlfvibi.html

[Q81] 字符串替换
来源：http://hz.hfpthk.cn/gtoafmsrkx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ybcxt.top/gtowpdxmnc.html

[Q82] 字符长度与字节长度
来源：http://hz.mhx1999.top/gtxrxqjrae.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.andypj.xyz/gtczzslkdc.html

[Q83] 大小写转换
来源：http://hz.cdnleiting.top/gtdkbqfnnk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ivvv.top/gtzgjwckrl.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtkbdpkkxf.html

SELECT TRIM(name) FROM users;
来源：http://hz.52xcode.cn/gtuhgrzpom.html

[Q85] 数值取整
来源：http://hz.xingfuxueyuan.xyz/gtgbslkymo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gotoacloud.top/gttmiafuma.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtrtvcoiis.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.quarkkingdee.top/gtriiuimko.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtwhfgbwht.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pengpengdd.cyou/gtxdcphkif.html

[Q88] 行转列（条件聚合）
来源：http://hz.redwolf501.top/gtkbykibqv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zycfv.cn/gtkqstvmzm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zdqjudy.top/gticcafhqz.html

[Q89] 判断表是否存在
来源：http://hz.xingfuxueyuan.xyz/gtlwnxitsc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtswlapavu.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gtcxuvyavx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258888.top/gtxegywosp.html

================================================================================
来源：http://hz.sufxvd.cn/gtcwggafba.html

R. Bash 专题
来源：http://hz.xylfe.cn/gtesichzqj.html

================================================================================
来源：http://hz.smart0.xyz/gtzaihpxzw.html

[R01] shebang 与严格模式
来源：http://hz.zycfv.cn/gtybpfjbin.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangkeji.top/gtfwnegjkq.html

set -euo pipefail
来源：http://hz.daxiang520.top/gtsdyzckzj.html

[R02] 变量赋值与使用
来源：http://hz.cqqwz.cn/gtmfthzxti.html

name="Tom"; echo "$name"
来源：http://hz.hongshengwenyu.top/gtsofhgwpn.html

[R03] 只读变量
来源：http://hz.ivvv.top/gtkxjvqhvr.html

readonly PI=3.14
来源：http://hz.yueranfly.top/gtrjvayeys.html

[R04] 位置参数
来源：http://hz.yj20258888.top/gtvbnwkrcv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhongyouzk.top/gtauutmmhy.html

[R05] 参数默认值
来源：http://hz.kuanghao11.cn/gtmwvybuyh.html

name="${1:-default}"
来源：http://hz.zycfv.cn/gtbybortdi.html

[R06] 判断命令是否存在
来源：http://hz.wangshuangyany.cn/gtqgolllgm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtthgcbwjd.html

[R07] if 判断文件
来源：http://hz.jyoumei.cn/gtlgmlfkzp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nwbrower.top/gtplaydizn.html

[R08] 数值比较
来源：http://hz.yuanzhike.top/gtzccxqopj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gogol.net.cn/gtpsdhjfqa.html

[R09] 字符串比较
来源：http://hz.zhixingplan.top/gtexyjxlrz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gzhubu.top/gtcfxtjurg.html

[R10] 正则匹配
来源：http://hz.hongshengwenyu.top/gtshudqpqc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.9152youxi.cn/gtosqqwcmu.html

[R11] case 多分支
来源：http://hz.nwbrower.top/gttjbzkmmd.html

case "$1" in
来源：http://hz.zhijiandao.cn/gtlfognknf.html

start) echo "启动" ;;
来源：http://hz.cashguo.top/gtsfskskwe.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtueicuqdh.html

*)     echo "未知命令" ;;
来源：http://hz.sufxvd.cn/gtlzmalkqr.html

esac
来源：http://hz.cqqwz.cn/gtzdfbihhx.html

[R12] for 遍历文件
来源：http://hz.iojbl.cn/gthewfcxmo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnqzz.top/gtisnnnwrq.html

[R13] for 计数循环
来源：http://hz.smart0.xyz/gtcljrxfvj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.feifeiyinyue.top/gtoavdwywr.html

[R14] C 风格 for
来源：http://hz.zhixingplan.top/gtcjmgdzvq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtjpqkfyxj.html

[R15] while 逐行读文件
来源：http://hz.jinghuilouyu.cn/gtefflgoly.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yueranfly.top/gtixogverr.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtnoirmzrk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.andypj.xyz/gtdgtwmjcr.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangkeji.top/gtrrmluaqz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinyuanbaomall.cn/gtolawbbvn.html

[R18] 遍历数组
来源：http://hz.yonumen.top/gtjbqltfnx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.bjfxy.top/gtraojazxm.html

[R19] 数组长度
来源：http://hz.dashuyun.cn/gtcvjigbwe.html

echo "${#arr[@]}"
来源：http://hz.yueranfly.top/gtkvglcupr.html

[R20] 关联数组（字典）
来源：http://hz.feifeiyinyue.top/gtyeyvaall.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dashuyun.cn/gtcaanoiff.html

[R21] 字符串长度
来源：http://hz.hfpthk.cn/gtfqzgnqec.html

echo "${#s}"
来源：http://hz.sysykeji.top/gtxbonodoy.html

[R22] 截取子串
来源：http://hz.ydjk.org.cn/gtqqlvrmen.html

echo "${s:0:5}"
来源：http://hz.haohaochexian.top/gtkdlhbpcm.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtkneckawi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtgcpggfsi.html

[R24] 大小写转换
来源：http://hz.jyoumei.cn/gtjepinjgl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jiagoushi.top/gtertcajjk.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtogtyrsry.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yvedp.cn/gtveptywez.html

[R26] 命令替换
来源：http://hz.quarkkingdee.top/gttdzraevw.html

now=$(date +%F); echo "$now"
来源：http://hz.cucudq.cn/gtgyowypmi.html

[R27] 算术展开
来源：http://hz.c1oappe.top/gtrgppnaql.html

echo $((1 + 2 * 3))
来源：http://hz.yj202588.top/gtbpkyawhs.html

[R28] 浮点运算
来源：http://hz.chenzaomai.com/gtiddbrisb.html

echo "scale=2; 10/3" | bc
来源：http://hz.daxiang520.top/gtgmykvjqr.html

[R29] 定义函数
来源：http://hz.snrcjt.cn/gtnaektbwy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.bjfxy.top/gtypbhxzpp.html

[R30] 函数返回状态码
来源：http://hz.vqdsnc.cn/gtvnfzcoxc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtztllgepr.html

[R31] 局部变量
来源：http://hz.gotoacloud.top/gtbkznbdhh.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtpfblolpu.html

[R32] 参数个数校验
来源：http://hz.fzhhl.top/gtybwpkwhq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shzxlz.cn/gtakeduhsm.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtdzsckirx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shangyingyoupin.top/gtdihuvwgb.html

[R34] 退出时清理
来源：http://hz.cheryme.top/gtcfprpfei.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gtokdnhdxp.html

[R35] 后台执行并等待
来源：http://hz.zhaomingkeji.xyz/gtgnjtuuyq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnxiangtu.top/gtcbtqcttt.html

[R36] 并发执行多个任务
来源：http://hz.wangshuangyany.cn/gtvgxcolwv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.52xcode.cn/gtfmpehzyy.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gteysoebce.html

files=$(ls -1)
来源：http://hz.haohaochexian.top/gtuomawsnk.html

[R38] 管道串联
来源：http://hz.zhoulong.xyz/gtdnfgloaa.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtrofzsagt.html

[R39] 重定向标准输出与错误
来源：http://hz.shangyingyoupin.top/gtwurpmlca.html

cmd > out.log 2>&1
来源：http://hz.gotoacloud.top/gtwsemkucr.html

[R40] 追加写日志
来源：http://hz.jinqigufen.top/gtetvylxsb.html

echo "log" >> out.log
来源：http://hz.52xcode.cn/gtwwtjjuqe.html

[R41] 丢弃输出
来源：http://hz.aibaodan.cn/gtnjasqlfo.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtooarorjy.html

[R42] 输入重定向
来源：http://hz.cqqwz.cn/gtetqjwseo.html

wc -l < a.txt
来源：http://hz.jinqigfzy.top/gtnyycseyd.html

[R43] 按名字查找文件
来源：http://hz.shzxlz.cn/gtxrpdrung.html

find . -name "*.log" -type f
来源：http://hz.guowangkeji.top/gtupuwssci.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gtwrbrkwgc.html

find . -mtime -7 -type f
来源：http://hz.xuanzx.com/gtqpzegnoz.html

[R45] 批量删除
来源：http://hz.hongshengwenyu.top/gtyodhcbei.html

find . -name "*.tmp" -delete
来源：http://hz.nwbrower.top/gtgutnaluu.html

[R46] 递归替换文件内容
来源：http://hz.yueranfly.top/gtpguxiizq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtnuvfkjub.html

[R47] sed 单行替换
来源：http://hz.sufxvd.cn/gtrulrbwsm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ywan-chungtsiang.top/gtkiiwtetx.html

[R48] awk 取指定列
来源：http://hz.birdmap.top/gtzppxrcpl.html

awk '{print $1, $3}' a.txt
来源：http://hz.52xcode.cn/gtosleuwlt.html

[R49] awk 带条件
来源：http://hz.pycfn.com/gtgqpxmpye.html


<!-- 参考信息 -->