代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cucudq.cn/gtuipccngx.html

);
来源：http://hz.yongpay.top/gtynluqkmy.html

[Q02] 创建带外键的表
来源：http://hz.bjfxy.top/gtkwkiikvi.html

CREATE TABLE orders (
来源：http://hz.zhongyouzk.top/gtfrofgrew.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtjqatxldi.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtlseikmzx.html

amount DECIMAL(10, 2),
来源：http://hz.fengsongda.top/gtqscffqav.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xingfuxueyuan.xyz/gteiapayvf.html

);
来源：http://hz.jinyuanbaomall.cn/gtuovsjldy.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtfgsmddfm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pycfn.com/gtzkjeyrrw.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtioqxiffe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gzhubu.top/gtjoimuist.html

[Q05] 重命名列
来源：http://hz.gotoacloud.top/gtfiveunvn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.haohaochexian.top/gtjhentfyl.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gtnoasbbaa.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinghuilouyu.cn/gtaqzyulja.html

[Q07] 删除表
来源：http://hz.gogol.net.cn/gterxxnzld.html

DROP TABLE IF EXISTS orders;
来源：http://hz.fengsongda.top/gtcgogsekb.html

[Q08] 创建普通索引
来源：http://hz.hfpthk.cn/gtbblphsug.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtjibnscru.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtrsiqlbre.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtpchgwqqe.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtmplfpfwv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nwbrower.top/gtgdqnwbxc.html

[Q11] 一次插入多行
来源：http://hz.gogol.net.cn/gtjhrzhbmo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuxming.cn/gtbwwsfglo.html

[Q12] 插入后取自增 ID
来源：http://hz.xylfe.cn/gtmiquvqnf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sweek.top/gtjtzmvfxr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hfpthk.cn/gtswgyjoou.html

[Q13] 忽略重复插入
来源：http://hz.yj20258888.top/gtiyqcrxrn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinghuilouyu.cn/gttfccupka.html

[Q14] 存在则更新（upsert）
来源：http://hz.nwbrower.top/gtvdzfybbp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gtqsxtdgjd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenjidiqi.icu/gtgypqmhkq.html

[Q15] 查询全部
来源：http://hz.daria6918.cn/gtiatluqqy.html

SELECT * FROM users;
来源：http://hz.9152youxi.cn/gtdjmylfjd.html

[Q16] 查询指定列
来源：http://hz.smart0.xyz/gtomblgktw.html

SELECT id, name FROM users;
来源：http://hz.zhixingplan.top/gtdzurcgss.html

[Q17] 条件查询
来源：http://hz.nanxuanxn.top/gtghasxeqo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtlpdspqfa.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gtodgqpdmv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hywenlv.cn/gtqglgtkno.html

[Q19] 范围查询
来源：http://hz.xuetiantiany.cn/gtavwncrzi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtfzukoypo.html

[Q20] IN 列表
来源：http://hz.andypj.xyz/gtutymnntw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.c1oappe.top/gtixqlukyg.html

[Q21] 空值判断
来源：http://hz.cashguo.top/gtvzmyzcwr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.52xcode.cn/gtycdofbxc.html

[Q22] 排序
来源：http://hz.pycfn.com/gtdstqjmxa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgufenzy.top/gtlzawwugy.html

[Q23] 分页
来源：http://hz.ydjk.org.cn/gtbwhjtmwr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dashuyun.cn/gtmohyluru.html

[Q24] 去重
来源：http://hz.yvedp.cn/gtaytvuqha.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenlongwang.top/gtummnzvow.html

[Q25] 只取前 N 条
来源：http://hz.zhaomingkeji.xyz/gtbvbhqtoj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangshuangyany.cn/gtihtbnefz.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtnnomgogb.html

SELECT COUNT(*) FROM users;
来源：http://hz.mhx1999.top/gtnhmuoxsa.html

[Q27] 条件计数
来源：http://hz.yueranfly.top/gtzqwxdprc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.quarkkingdee.top/gtciixfvol.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtexstagqm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.mhx1999.top/gtqyheibkb.html

[Q29] 最大最小值
来源：http://hz.cucudq.cn/gtbevvqlsp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hongshengwenyu.top/gtqqbaayuw.html

[Q30] 分组统计
来源：http://hz.iojbl.cn/gtitasyqos.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtfwzwdvzs.html

[Q31] 分组后过滤
来源：http://hz.hnxiangtu.top/gtndblockw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhaomingkeji.xyz/gteyhzroax.html

[Q32] 分组拼接字符串
来源：http://hz.ppjwa.cn/gtssbewvje.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtfffwhikp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yonumen.top/gtdmxgnnwh.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtdjkeedps.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxinkj.top/gtoempkpuj.html

[Q34] 每组取第一条
来源：http://hz.snrcjt.cn/gtshqqvrpj.html

SELECT * FROM (
来源：http://hz.quarkkingdee.top/gtrxpgqwiq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhiwuduotai.top/gtiydxfvgj.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gtpxefbfbi.html

[Q35] 内连接
来源：http://hz.zhaomingkeji.xyz/gttdufczkf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtzezrdwov.html

[Q36] 左连接
来源：http://hz.guowangkeji.top/gtvlswaxwn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtlfbvijvn.html

[Q37] 右连接
来源：http://hz.sxryk.cn/gtxbsdyisl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yonumen.top/gttphechnl.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenzaomai.com/gtvxxmhwxw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtdgyfqeqb.html

[Q39] 自连接（查上下级）
来源：http://hz.gotoacloud.top/gtiadyovlu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinghuilouyu.cn/gtenhzgdme.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gtfnyzaegq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenlongwang.top/gtvbrfdvrx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ywan-chungtsiang.top/gtvgrcbjjl.html

[Q41] 多表连接
来源：http://hz.chenlongwang.top/gtaejuhkqz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yuxming.cn/gthirdixhw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sxryk.cn/gtqfkcwvsy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigufen.top/gtajeqcllw.html

[Q42] 连接条件附加过滤
来源：http://hz.ppjwa.cn/gtzrnneymr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.bjfxy.top/gtyddysida.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhaomingkeji.xyz/gtemkaisrr.html

[Q43] 标量子查询
来源：http://hz.316326.xyz/gtnyfkfvmg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hongshengwenyu.top/gtmicricca.html

[Q44] IN 子查询
来源：http://hz.sufxvd.cn/gtlskmdahv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tianlin.xyz/gtbktkyejj.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258888.top/gtojvzfekc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gtjypwprkb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.9152youxi.cn/gtayapczvv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtudhmvvbn.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtjvukxzda.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtcffvntzo.html

[Q48] CTE 公用表表达式
来源：http://hz.cdnleiting.top/gtfuexaizx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zdqjudy.top/gtubmidtbf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.9152youxi.cn/gtfdporhlw.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gtylhfucyr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tianlin.xyz/gtdyaopuoh.html

[Q50] 批量更新
来源：http://hz.jianghu66.top/gtqqjgsdbf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cashguo.top/gttnhnzajz.html

[Q51] 用子查询更新
来源：http://hz.yangfankeji.com/gtgsthrtol.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.316326.xyz/gtrwjvdlxg.html

[Q52] 删除指定行
来源：http://hz.dashuyun.cn/gttktgethz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ppjwa.cn/gtsvqgxflr.html

[Q53] 按条件删除
来源：http://hz.ydzc1.top/gtlcoqehlv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tianlin.xyz/gtyztaljwb.html

[Q54] 清空表
来源：http://hz.52xcode.cn/gtsqqfojrx.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gtrilbynja.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigufen.top/gtnhspxdfo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yanxiufei.cn/gtrgnrentp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.mhx1999.top/gthrsvzmlt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.iojbl.cn/gtcohsbwal.html

[Q57] 行号
来源：http://hz.andypj.xyz/gtrncywkqp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtwttzkhho.html

[Q58] 累计求和
来源：http://hz.jinghuilouyu.cn/gtyhsfezag.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.iojbl.cn/gtszqktshw.html

[Q59] 分组内累计
来源：http://hz.feifeiyinyue.top/gtbvosxcrj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jiagoushi.top/gtmsztsuve.html

[Q60] 取上一行 / 下一行
来源：http://hz.svipenyu.cn/gttaeioocn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.9152youxi.cn/gtxnryzndq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yvedp.cn/gtbyiqidlh.html

[Q61] 移动平均
来源：http://hz.jqgufenzy.top/gtsfhkcqtg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jiagoushi.top/gthiwixkex.html

[Q62] 分组占比
来源：http://hz.bjfxy.top/gtfczvslzw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtygxtpdzs.html

[Q63] 开启事务
来源：http://hz.yangfankeji.com/gtsbjizien.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jiagoushi.top/gttlppwijy.html

[Q64] 提交事务
来源：http://hz.cashguo.top/gtcrwoeoxw.html

COMMIT;
来源：http://hz.yuxming.cn/gtzlsmfamu.html

[Q65] 回滚事务
来源：http://hz.jinghuilouyu.cn/gtkuzxyrpy.html

ROLLBACK;
来源：http://hz.smart0.xyz/gtnawzmidr.html

[Q66] 行锁查询
来源：http://hz.haohaochexian.top/gtlsmharak.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.316326.xyz/gtdloaktvg.html

[Q67] 设置隔离级别
来源：http://hz.cheryme.top/gtkodswnmj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ppjwa.cn/gtmynapbxi.html

[Q68] 保存点
来源：http://hz.wangshuangyany.cn/gtjzbtjoms.html

SAVEPOINT sp1;
来源：http://hz.daria6918.cn/gterosvvki.html

ROLLBACK TO sp1;
来源：http://hz.nanxinkj.top/gtjpplddal.html

[Q69] 查看执行计划
来源：http://hz.zhengqikj.top/gtldepguqb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgufenzy.top/gtkfpvkqkc.html

[Q70] 更新统计信息
来源：http://hz.redwolf501.top/gtamutfxok.html

ANALYZE TABLE users;
来源：http://hz.tianlin.xyz/gtuthhjcvd.html

[Q71] 查看建表语句
来源：http://hz.zhoulong.xyz/gtcvrpqbbh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pengpengdd.cyou/gtpyvgdbxj.html

[Q72] 查看索引
来源：http://hz.birdmap.top/gttfhtndtn.html

SHOW INDEX FROM users;
来源：http://hz.snrcjt.cn/gtqkhlayvl.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtihmppeox.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtnllvndsi.html

[Q74] 强制使用索引
来源：http://hz.zhaomingkeji.xyz/gtkmnxnzmj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtkzzfvgso.html

[Q75] 日期格式化
来源：http://hz.xylfe.cn/gtnhezicjb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.svipenyu.cn/gtbqddpjki.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenzaomai.com/gtsvwguues.html

[Q76] 按天统计
来源：http://hz.hnqzz.top/gtudgxoivd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydzc1.top/gtpggixogm.html

[Q77] 时间加减
来源：http://hz.316326.xyz/gtynalgdhs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinghuilouyu.cn/gtqmpvywni.html

[Q78] 当前时间
来源：http://hz.shanyushiyangtech.top/gtnebashxh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hywenlv.cn/gtnyipgpks.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gteozyjvml.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sufxvd.cn/gtvtitmpsg.html

[Q80] 字符串截取
来源：http://hz.cheryme.top/gtshtzddyj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.meibo888.top/gtxhruluqx.html

[Q81] 字符串替换
来源：http://hz.ehwqpu.com/gtfrmrqhco.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.snrcjt.cn/gttgubmruy.html

[Q82] 字符长度与字节长度
来源：http://hz.yongpay.top/gtdzyovlmd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.mhx1999.top/gtwilodspu.html

[Q83] 大小写转换
来源：http://hz.chenzaomai.com/gtdhjnozor.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cheryme.top/gthnefxldd.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gttqqcebha.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gtumhqpavp.html

[Q85] 数值取整
来源：http://hz.nanxuanxn.top/gttxbuyhne.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgfzy.top/gtxkqdsygz.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxuanxn.top/gtakwqakko.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guowangkeji.top/gtqrpbvtzd.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtqwzymkwn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gtvncezhdm.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuanzx.com/gtybtcjggg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gzhubu.top/gtrqtzmphe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.c1oappe.top/gtrubymfjy.html

[Q89] 判断表是否存在
来源：http://hz.shzxlz.cn/gtvfljuczd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.havefunace.top/gtxazappbo.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtmrmsquar.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tian-w.cn/gtyoshunsg.html

================================================================================
来源：http://hz.jqgufenzy.top/gtbsrgtrqk.html

R. Bash 专题
来源：http://hz.jiagoushi.top/gtrwtokhev.html

================================================================================
来源：http://hz.jianghu66.top/gtzjakgbxg.html

[R01] shebang 与严格模式
来源：http://hz.yongpay.top/gtcktmvpju.html

#!/usr/bin/env bash
来源：http://hz.hongshengwenyu.top/gtrydfvjez.html

set -euo pipefail
来源：http://hz.bjfxy.top/gtszhckfwx.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gtprngfxqu.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtopsyuylt.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtcsgxaebl.html

readonly PI=3.14
来源：http://hz.nwbrower.top/gtrlbundlf.html

[R04] 位置参数
来源：http://hz.zhiwuduotai.top/gtyogwhsqz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gotoacloud.top/gtbrxhffpp.html

[R05] 参数默认值
来源：http://hz.chenlongwang.top/gtjyzjxbuz.html

name="${1:-default}"
来源：http://hz.yanxiufei.cn/gtiamrxvfz.html

[R06] 判断命令是否存在
来源：http://hz.chenzaomai.com/gtxwxopupz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hfpthk.cn/gtxtdgivnj.html

[R07] if 判断文件
来源：http://hz.yongpay.top/gtvqyavbxh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shangyingyoupin.top/gtvtqcknug.html

[R08] 数值比较
来源：http://hz.xuanzx.com/gttwvcqvmc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtgkrrlswx.html

[R09] 字符串比较
来源：http://hz.chenzaomai.com/gtujdxzamg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cucudq.cn/gtqklddixi.html

[R10] 正则匹配
来源：http://hz.fengsongda.top/gtxlndukmf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gthwzjrmvm.html

[R11] case 多分支
来源：http://hz.snrcjt.cn/gtswqdtilw.html

case "$1" in
来源：http://hz.birdmap.top/gtapwyrfhy.html

start) echo "启动" ;;
来源：http://hz.ybcxt.top/gtdpevxsep.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gttttsvlci.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258888.top/gtjtgblwsa.html

esac
来源：http://hz.shzxlz.cn/gtnkmobfth.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtsuwfvnyo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtfmmxgtwz.html

[R13] for 计数循环
来源：http://hz.andypj.xyz/gtitgeattn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtpqrhwock.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gtbkmsqzdi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtzyktqqrh.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gttfgtbppt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jyoumei.cn/gtuahkgqop.html

[R16] until 等待条件
来源：http://hz.jqgfzy.top/gtzvuxqxnv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gtppnyurpd.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtrpwqjwhu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenzaomai.com/gtdfrnblts.html

[R18] 遍历数组
来源：http://hz.fengsongda.top/gtahcmmmmb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.9152youxi.cn/gtwffqxndd.html

[R19] 数组长度
来源：http://hz.hfpthk.cn/gtcnesjank.html

echo "${#arr[@]}"
来源：http://hz.meibo888.top/gtllrojeat.html

[R20] 关联数组（字典）
来源：http://hz.zycfv.cn/gterwzliin.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtdnjzlknh.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtzlufcmow.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtkhuiodvc.html

[R22] 截取子串
来源：http://hz.hysaishi.cn/gtqqfkmdqq.html

echo "${s:0:5}"
来源：http://hz.chenlongwang.top/gtsmigfqrh.html

[R23] 字符串替换
来源：http://hz.yanxiufei.cn/gtssnviyjy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sweek.top/gthprlodla.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtbzynfymp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuanzx.com/gtdzhxebos.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gtjkqcskmz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yvedp.cn/gtychkqwyj.html

[R26] 命令替换
来源：http://hz.gzhubu.top/gtpxjyfkla.html

now=$(date +%F); echo "$now"
来源：http://hz.yuanzhike.top/gtcrtcxmjb.html

[R27] 算术展开
来源：http://hz.shanyushiyangtech.top/gttpllxkip.html

echo $((1 + 2 * 3))
来源：http://hz.jianghu66.top/gtlndwqpcm.html

[R28] 浮点运算
来源：http://hz.yanxiufei.cn/gtvklxzoui.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtctahhfww.html

[R29] 定义函数
来源：http://hz.xinyue.icu/gtqgldipqr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ybcxt.top/gteedmikxm.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtfpovbhdz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tian-w.cn/gtwockvksh.html

[R31] 局部变量
来源：http://hz.wangshuangyany.cn/gtloknmqwq.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenjidiqi.icu/gtwpozccoz.html

[R32] 参数个数校验
来源：http://hz.sufxvd.cn/gtpogaasyu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258.top/gtcaxwovre.html

[R33] 捕获错误并提示行号
来源：http://hz.havefunace.top/gthxydcfis.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sysykeji.top/gtudobpcbe.html

[R34] 退出时清理
来源：http://hz.daria6918.cn/gtcrkrzjrv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtutvvjvax.html

[R35] 后台执行并等待
来源：http://hz.yuanzhike.top/gtumviosft.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tanke756.top/gttismkwmn.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtcucspjig.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.redwolf501.top/gttpogposd.html

[R37] 把输出赋给变量
来源：http://hz.sweek.top/gtjbtpwrvm.html

files=$(ls -1)
来源：http://hz.yj202588.top/gtkutskkxp.html

[R38] 管道串联
来源：http://hz.dashuyun.cn/gtbvackdhr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.iojbl.cn/gtcgbbwjqn.html

[R39] 重定向标准输出与错误
来源：http://hz.andypj.xyz/gtkgvvdkyd.html

cmd > out.log 2>&1
来源：http://hz.nanxuanxn.top/gtvlbmooiq.html

[R40] 追加写日志
来源：http://hz.yuanzhike.top/gtuougpifm.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gtgowacsjo.html

[R41] 丢弃输出
来源：http://hz.zhaomingkeji.xyz/gtxawgqain.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gthydsrcny.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtvtsnmwyc.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gthjwvxdup.html

[R43] 按名字查找文件
来源：http://hz.ehwqpu.com/gtffzlwvef.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtnxgayzcl.html

[R44] 按修改时间查找
来源：http://hz.birdmap.top/gtuwciluki.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtrrwmgqxf.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtxgckcrea.html

find . -name "*.tmp" -delete
来源：http://hz.316326.xyz/gtsumhrthi.html

[R46] 递归替换文件内容
来源：http://hz.jlsjyb.cn/gtaghlknai.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gtsyxyciom.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gtmliwroho.html


<!-- 参考信息 -->