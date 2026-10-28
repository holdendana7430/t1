代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sysykeji.top/gtvsafmtcw.html

);
来源：http://hz.mhx1999.top/gtiighgxxe.html

[Q02] 创建带外键的表
来源：http://hz.nanxuanxn.top/gtlyabfyjg.html

CREATE TABLE orders (
来源：http://hz.ydjk.org.cn/gtpnzobien.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shangyingyoupin.top/gtfshgunsg.html

user_id INT NOT NULL,
来源：http://hz.shuidangran.top/gteigfkmzs.html

amount DECIMAL(10, 2),
来源：http://hz.havefunace.top/gtqdybhaag.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangtech.top/gtsdhmedjo.html

);
来源：http://hz.jiagoushi.top/gtiwgcsgeo.html

[Q03] 增加列
来源：http://hz.gzhubu.top/gthyjfylhe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dashuyun.cn/gtmmpunwpk.html

[Q04] 修改列类型
来源：http://hz.jlsjyb.cn/gtjxmthhpn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jianghu66.top/gtyrtbepta.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtnksdbacd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.birdmap.top/gtgdvqiooq.html

[Q06] 删除列
来源：http://hz.shangyingyoupin.top/gtfklvglzc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fengsongda.top/gtoajebjbj.html

[Q07] 删除表
来源：http://hz.ivvv.top/gtuzrgkpub.html

DROP TABLE IF EXISTS orders;
来源：http://hz.meibo888.top/gtvbhirmip.html

[Q08] 创建普通索引
来源：http://hz.aibaodan.cn/gtndzhslay.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtwhnojgvu.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtnkztsafw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hfpthk.cn/gtjnlavpau.html

[Q10] 插入单行
来源：http://hz.ydzc1.top/gtuufkljwc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.snrcjt.cn/gtudvwhuef.html

[Q11] 一次插入多行
来源：http://hz.fzhhl.top/gtkcbamufk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.52xcode.cn/gtoliomyqz.html

[Q12] 插入后取自增 ID
来源：http://hz.wangshuangyany.cn/gtyyhmymlj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.c1oappe.top/gtqlhnutwb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xziqi.cn/gtjegpdthv.html

[Q13] 忽略重复插入
来源：http://hz.yongpay.top/gtvabozkxc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangshuangyany.cn/gtaddbplqv.html

[Q14] 存在则更新（upsert）
来源：http://hz.jianghu66.top/gthzjombyc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigufen.top/gtkjofhmlh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangkeji.top/gttbebwsil.html

[Q15] 查询全部
来源：http://hz.tianlin.xyz/gttkcagadf.html

SELECT * FROM users;
来源：http://hz.yongpay.top/gtjrnahxjn.html

[Q16] 查询指定列
来源：http://hz.gotoacloud.top/gttypqktbj.html

SELECT id, name FROM users;
来源：http://hz.jqgufenzy.top/gtdchhcahk.html

[Q17] 条件查询
来源：http://hz.yanxiufei.cn/gtygtexayw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.iojbl.cn/gtgqzerzkb.html

[Q18] 模糊匹配
来源：http://hz.zhengqikj.top/gtxsechtcu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nwbrower.top/gthdkrqlcw.html

[Q19] 范围查询
来源：http://hz.mhx1999.top/gthvrbhlen.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtnbfbkclj.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtvxppcxtw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sysykeji.top/gtppbxuhfe.html

[Q21] 空值判断
来源：http://hz.yongpay.top/gtjtdwltya.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.316326.xyz/gtzbamaihb.html

[Q22] 排序
来源：http://hz.pengpengdd.cyou/gtrfhfyjqn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tanke756.top/gtpqagfhez.html

[Q23] 分页
来源：http://hz.andypj.xyz/gtsuvpumor.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxuanxn.top/gtddixmgik.html

[Q24] 去重
来源：http://hz.yj20258888.top/gtukqkrxzt.html

SELECT DISTINCT city FROM users;
来源：http://hz.tian-w.cn/gtwmulyyvm.html

[Q25] 只取前 N 条
来源：http://hz.nwbrower.top/gtjxomstlg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zdqjudy.top/gtvlyclwaw.html

[Q26] 计数
来源：http://hz.kuanghao11.cn/gtfqzyubas.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj20258888.top/gtsyqvukzz.html

[Q27] 条件计数
来源：http://hz.9152youxi.cn/gtkjunmhol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhoulong.xyz/gtnsidakuz.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtzsybsxgk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gtvlrfclfx.html

[Q29] 最大最小值
来源：http://hz.hnqzz.top/gtmrzauexi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtjqgtfscq.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtszaltvvy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtiddqajef.html

[Q31] 分组后过滤
来源：http://hz.aibaodan.cn/gtkrcxcupd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.0kj1m.cn/gtqqamvver.html

[Q32] 分组拼接字符串
来源：http://hz.nanxinkj.top/gttamccydd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtnbevdzjh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cucudq.cn/gtbavzkebj.html

[Q33] 多列分组
来源：http://hz.c1oappe.top/gtryrblldi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.316326.xyz/gtlyivxcus.html

[Q34] 每组取第一条
来源：http://hz.jqgfzy.top/gtsqaykcou.html

SELECT * FROM (
来源：http://hz.meibo888.top/gtdfiwtpyz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xingfuxueyuan.xyz/gtfctiorof.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtitxcecut.html

[Q35] 内连接
来源：http://hz.nanxuanxn.top/gtewrcvqos.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtlzaelctg.html

[Q36] 左连接
来源：http://hz.9152youxi.cn/gtilrtomcx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cqqwz.cn/gtrmbpphvx.html

[Q37] 右连接
来源：http://hz.fzhhl.top/gthawdajoz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gtdimljojq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.c1oappe.top/gttybjlano.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhiwuduotai.top/gtolpcawke.html

[Q39] 自连接（查上下级）
来源：http://hz.hongshengwenyu.top/gtxpbnitnd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj202588.top/gtvkqzwjgx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.redwolf501.top/gtqkekotyk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xylfe.cn/gtdvyamyue.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gthnzodfls.html

[Q41] 多表连接
来源：http://hz.zhiwuduotai.top/gtyoldvqrf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhiwuduotai.top/gtucbzcntg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gtfkukbcin.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pengpengdd.cyou/gtfhxtojrv.html

[Q42] 连接条件附加过滤
来源：http://hz.hywenlv.cn/gtfuyxkvql.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhiwuduotai.top/gtbbvvslga.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gogol.net.cn/gtdktxzwrn.html

[Q43] 标量子查询
来源：http://hz.pengpengdd.cyou/gtuhkehnuj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.quarkkingdee.top/gtjiljecxk.html

[Q44] IN 子查询
来源：http://hz.yj20258888.top/gterishlto.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yuxming.cn/gtipvnjltz.html

[Q45] EXISTS 判断存在
来源：http://hz.pycfn.com/gtxcttezbr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtyitufcyl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtwcwkualb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jlsjyb.cn/gtmlwdfxgq.html

[Q47] 与平均值比较
来源：http://hz.yonumen.top/gtrkhphdub.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sufxvd.cn/gtkkxodnuf.html

[Q48] CTE 公用表表达式
来源：http://hz.chenlongwang.top/gtzgvvdxyu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tianlin.xyz/gtnhmacvtv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.havefunace.top/gtwjpvqeau.html

[Q49] 更新单行
来源：http://hz.birdmap.top/gtxffajxiu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.andypj.xyz/gtqjdhmmil.html

[Q50] 批量更新
来源：http://hz.andypj.xyz/gtlcecgicc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gtqrruvikl.html

[Q51] 用子查询更新
来源：http://hz.tian-w.cn/gttoyhflhm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangtech.top/gtdjlhkgqi.html

[Q52] 删除指定行
来源：http://hz.jyoumei.cn/gtrmovfdlx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daria6918.cn/gtniugepnr.html

[Q53] 按条件删除
来源：http://hz.yuanzhike.top/gtagipcecb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cdnleiting.top/gtgijcuyeg.html

[Q54] 清空表
来源：http://hz.quarkkingdee.top/gtfotfwdmw.html

TRUNCATE TABLE logs;
来源：http://hz.yuanzhike.top/gtzfvytzch.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gtnkqqqhtr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sufxvd.cn/gtjnypxvfy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgufenzy.top/gtlkgfcbzw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtnqmvxrmb.html

[Q57] 行号
来源：http://hz.fengsongda.top/gtrwytxyqo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pengpengdd.cyou/gtbqdpkgto.html

[Q58] 累计求和
来源：http://hz.gaohongyu789.top/gtlqhdhomz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pengpengdd.cyou/gtwzgnroum.html

[Q59] 分组内累计
来源：http://hz.ehwqpu.com/gtnyjugwtx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ydjk.org.cn/gtyshdxizu.html

[Q60] 取上一行 / 下一行
来源：http://hz.gaohongyu789.top/gthcgznuku.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tianlin.xyz/gthluooxoa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.c1oappe.top/gtacgrjfnw.html

[Q61] 移动平均
来源：http://hz.gzhubu.top/gtcklasdnf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gthpiwqmyu.html

[Q62] 分组占比
来源：http://hz.cqqwz.cn/gtehlbqfqj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtfktufins.html

[Q63] 开启事务
来源：http://hz.xylfe.cn/gtvgbplmqg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jianghu66.top/gtqmfxkvlg.html

[Q64] 提交事务
来源：http://hz.gotoacloud.top/gtiofkqvww.html

COMMIT;
来源：http://hz.zdqjudy.top/gtzqagwmjj.html

[Q65] 回滚事务
来源：http://hz.iojbl.cn/gtbkeiaedm.html

ROLLBACK;
来源：http://hz.kuanghao11.cn/gtlrymfwad.html

[Q66] 行锁查询
来源：http://hz.zhixingplan.top/gtmerpnlvq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.havefunace.top/gtxvkmwrkq.html

[Q67] 设置隔离级别
来源：http://hz.xingfuxueyuan.xyz/gtaempdmdo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtjrpizomi.html

[Q68] 保存点
来源：http://hz.vqdsnc.cn/gtepvrmhmv.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtfbmbfdwv.html

ROLLBACK TO sp1;
来源：http://hz.yj202588.top/gtpkfmgcnl.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtirqrpxde.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sufxvd.cn/gtrhfxsdep.html

[Q70] 更新统计信息
来源：http://hz.zhoulong.xyz/gtetctxutk.html

ANALYZE TABLE users;
来源：http://hz.dashuyun.cn/gtrpizkteo.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtpkzzyykg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.316326.xyz/gtusgkjzdt.html

[Q72] 查看索引
来源：http://hz.c1oappe.top/gtxkmihqjj.html

SHOW INDEX FROM users;
来源：http://hz.cucudq.cn/gtewvtsdmv.html

[Q73] 查看表状态
来源：http://hz.316326.xyz/gthgtnlsqw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gotoacloud.top/gtelfqarlv.html

[Q74] 强制使用索引
来源：http://hz.svipenyu.cn/gteelwgxjy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ivvv.top/gtwrmbvukv.html

[Q75] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtgvhogibw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinqigufen.top/gtqcukggiw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxuanxn.top/gtkmrwsmmk.html

[Q76] 按天统计
来源：http://hz.cucudq.cn/gtfvpptloj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shzxlz.cn/gtlxwmzpmz.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtwyugaymv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.bjfxy.top/gtlqhptolw.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gtujjfaytm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnxiangtu.top/gtqtyfsrlk.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtkjbxqqqp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yuxming.cn/gtmcmrluae.html

[Q80] 字符串截取
来源：http://hz.tianlin.xyz/gtmrrklnli.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtxmamxood.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtsoxwvzbv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gogol.net.cn/gtbllyatvn.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gteyujyxkw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.birdmap.top/gtoxtiymdy.html

[Q83] 大小写转换
来源：http://hz.jianghu66.top/gtumjzqxiw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.birdmap.top/gtapgdnnjl.html

[Q84] 去除首尾空格
来源：http://hz.fzhhl.top/gtonyxsekr.html

SELECT TRIM(name) FROM users;
来源：http://hz.yueranfly.top/gtlnrebkge.html

[Q85] 数值取整
来源：http://hz.bjfxy.top/gtwtcnyrip.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hongshengwenyu.top/gtcepvhmpg.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtjkahuefk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gteqokphju.html

[Q87] JSON 字段做条件
来源：http://hz.yangfankeji.com/gtcdvmjbms.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258.top/gtaqxzmykm.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnxiangtu.top/gtlkriuzzt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zycfv.cn/gtmwdlxdlw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gtejeunygp.html

[Q89] 判断表是否存在
来源：http://hz.pengpengdd.cyou/gtbtzqrkvs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenzaomai.com/gtjgtevofw.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtkwhijkej.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yvedp.cn/gtkcmmsylx.html

================================================================================
来源：http://hz.dashuyun.cn/gtkvopnzpq.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtnftwcgmr.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvnyfatun.html

[R01] shebang 与严格模式
来源：http://hz.birdmap.top/gtdtninzjo.html

#!/usr/bin/env bash
来源：http://hz.hammf.cn/gtupbzkksp.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtoovdrcps.html

[R02] 变量赋值与使用
来源：http://hz.316326.xyz/gtvjzfgwop.html

name="Tom"; echo "$name"
来源：http://hz.shzxlz.cn/gtxspkrijd.html

[R03] 只读变量
来源：http://hz.svipenyu.cn/gtcimtupzr.html

readonly PI=3.14
来源：http://hz.tianlin.xyz/gthccwvyxb.html

[R04] 位置参数
来源：http://hz.hfpthk.cn/gtoxwsghhn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258888.top/gthyqwqlry.html

[R05] 参数默认值
来源：http://hz.zhijiandao.cn/gtzuhrmyxv.html

name="${1:-default}"
来源：http://hz.sysykeji.top/gtbeixnhns.html

[R06] 判断命令是否存在
来源：http://hz.dianchejie.cn/gtcactekyt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtonhwzoii.html

[R07] if 判断文件
来源：http://hz.jinqigufen.top/gtvofwwqsl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.mhx1999.top/gtkbhlemnl.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtkocjplhd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuanzx.com/gtymeexojr.html

[R09] 字符串比较
来源：http://hz.jinqigufen.top/gtbhiamxho.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinghuilouyu.cn/gtaorwcwap.html

[R10] 正则匹配
来源：http://hz.nwbrower.top/gtdskoqiiy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gthqgkjacf.html

[R11] case 多分支
来源：http://hz.chenzaomai.com/gtravcggzt.html

case "$1" in
来源：http://hz.gaohongyu789.top/gtocpjkvkn.html

start) echo "启动" ;;
来源：http://hz.hnqzz.top/gtliseijsx.html

stop)  echo "停止" ;;
来源：http://hz.hnxiangtu.top/gtyellekjw.html

*)     echo "未知命令" ;;
来源：http://hz.gogol.net.cn/gtxcwzqxft.html

esac
来源：http://hz.hysaishi.cn/gtpbvonfcw.html

[R12] for 遍历文件
来源：http://hz.sufxvd.cn/gtgqysfwdp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydzc1.top/gtfafageri.html

[R13] for 计数循环
来源：http://hz.jqgufenzy.top/gtsgoosznc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.316326.xyz/gtjynuujrs.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gtcskhsigb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtjijjdefl.html

[R15] while 逐行读文件
来源：http://hz.yj20258.top/gtjeqngdpj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuanzx.com/gtznwblccy.html

[R16] until 等待条件
来源：http://hz.chenlongwang.top/gtlcdewzem.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtjkhhhngm.html

[R17] 数组定义与取值
来源：http://hz.cucudq.cn/gtpiuojakh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtqfaircwb.html

[R18] 遍历数组
来源：http://hz.chenjidiqi.icu/gtjopecayy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.0kj1m.cn/gtwikynaka.html

[R19] 数组长度
来源：http://hz.gzhubu.top/gtblwrzsnp.html

echo "${#arr[@]}"
来源：http://hz.cheryme.top/gtjgozuitx.html

[R20] 关联数组（字典）
来源：http://hz.jinqigufen.top/gttpwjnqfu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jianghu66.top/gtsitdhtqw.html

[R21] 字符串长度
来源：http://hz.xinyue.icu/gtmmkjzmbf.html

echo "${#s}"
来源：http://hz.nanxuanxn.top/gtrcbemjsc.html

[R22] 截取子串
来源：http://hz.aibaodan.cn/gtvktdpqay.html

echo "${s:0:5}"
来源：http://hz.hfpthk.cn/gtoxffacob.html

[R23] 字符串替换
来源：http://hz.vqdsnc.cn/gthoduzuwv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.0kj1m.cn/gtqgsjwsbg.html

[R24] 大小写转换
来源：http://hz.yj202588.top/gthubgbnrc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtojqpymvg.html

[R25] 去后缀 / 去前缀
来源：http://hz.gogol.net.cn/gtjfiwdwrj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sxryk.cn/gtmpcghkvi.html

[R26] 命令替换
来源：http://hz.feifeiyinyue.top/gtzbicnfrx.html

now=$(date +%F); echo "$now"
来源：http://hz.yangfankeji.com/gtmevmwujq.html

[R27] 算术展开
来源：http://hz.cucudq.cn/gtbekqiwqq.html

echo $((1 + 2 * 3))
来源：http://hz.ehwqpu.com/gtsnlmyxfl.html

[R28] 浮点运算
来源：http://hz.hfpthk.cn/gtvazifscx.html

echo "scale=2; 10/3" | bc
来源：http://hz.fengsongda.top/gtiqlbpdri.html

[R29] 定义函数
来源：http://hz.hongshengwenyu.top/gtgyealccd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sweek.top/gtczylkvfr.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtllqyuiuj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.bjfxy.top/gtfynseqcv.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gtkznkjnar.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtizplfwnb.html

[R32] 参数个数校验
来源：http://hz.zhiwuduotai.top/gtxulyaynx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtusuexwhv.html

[R33] 捕获错误并提示行号
来源：http://hz.zhaomingkeji.xyz/gtorvfysdh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgufenzy.top/gtkhaomkpm.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gtpjbrujcd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtkrdnwbej.html

[R35] 后台执行并等待
来源：http://hz.yj202588.top/gtfquemntb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xylfe.cn/gtgqrkkfpy.html

[R36] 并发执行多个任务
来源：http://hz.xylfe.cn/gtmmbwtgvh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fengsongda.top/gtlwrenkqw.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtlomuwror.html

files=$(ls -1)
来源：http://hz.iojbl.cn/gtjkqvjsmb.html

[R38] 管道串联
来源：http://hz.birdmap.top/gtptzqovda.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daria6918.cn/gtgazlfdzm.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtuidjlkdc.html

cmd > out.log 2>&1
来源：http://hz.xylfe.cn/gtcjibgbnk.html

[R40] 追加写日志
来源：http://hz.gaohongyu789.top/gtawfkgvov.html

echo "log" >> out.log
来源：http://hz.gotoacloud.top/gtsyoifzjq.html

[R41] 丢弃输出
来源：http://hz.kuanghao11.cn/gtjjsdnpdu.html

cmd >/dev/null 2>&1
来源：http://hz.sufxvd.cn/gtrpxelays.html

[R42] 输入重定向
来源：http://hz.zhaomingkeji.xyz/gtuoezhtmd.html

wc -l < a.txt
来源：http://hz.zycfv.cn/gtkvgldgwd.html

[R43] 按名字查找文件
来源：http://hz.xuetiantiany.cn/gtquuiunxx.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangkeji.top/gtievjkgdh.html

[R44] 按修改时间查找
来源：http://hz.kuanghao11.cn/gtpypoaqih.html

find . -mtime -7 -type f
来源：http://hz.yongpay.top/gtstngzqtn.html

[R45] 批量删除
来源：http://hz.jqgfzy.top/gtgjrpeumz.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258888.top/gtulqezzvp.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtifefbxyi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cqqwz.cn/gtyilmtbjx.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtwqvxcsfh.html


<!-- 参考信息 -->