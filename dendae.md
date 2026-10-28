代发 wailian999

);
来源：http://hz.zhongyouzk.top/gtmkfrwhas.html

[Q03] 增加列
来源：http://hz.bjfxy.top/gtovqnrwnr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pycfn.com/gtvaxjlqwl.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtorcbuood.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangshuangyany.cn/gtyambrhaj.html

[Q05] 重命名列
来源：http://hz.zhixingplan.top/gtwpkcxlvg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hfpthk.cn/gtduchmiyn.html

[Q06] 删除列
来源：http://hz.sweek.top/gtxruawqge.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigfzy.top/gtiukeecyt.html

[Q07] 删除表
来源：http://hz.daria6918.cn/gtruqdoxls.html

DROP TABLE IF EXISTS orders;
来源：http://hz.52xcode.cn/gtbmegnibl.html

[Q08] 创建普通索引
来源：http://hz.ywan-chungtsiang.top/gtbyoekngg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtsrdssmym.html

[Q09] 创建唯一索引
来源：http://hz.nwbrower.top/gtmpljioun.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zdqjudy.top/gtfmeddnfk.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gtylagjqar.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhoulong.xyz/gtnaavsvmd.html

[Q11] 一次插入多行
来源：http://hz.jinqigufen.top/gtlwajgyxa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangshuangyany.cn/gtwqevwrpr.html

[Q12] 插入后取自增 ID
来源：http://hz.zhaomingkeji.xyz/gtfbkntxnf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gtcmfglsfh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gotoacloud.top/gtxglvuctn.html

[Q13] 忽略重复插入
来源：http://hz.jiagoushi.top/gtlmkdrbxf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangdashe.top/gtsdtzjtxz.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtaldbnimw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtbsopbpko.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.andypj.xyz/gtnfktioqr.html

[Q15] 查询全部
来源：http://hz.jqgfzy.top/gtsquzssiy.html

SELECT * FROM users;
来源：http://hz.yueranfly.top/gtggvmlcwz.html

[Q16] 查询指定列
来源：http://hz.gogol.net.cn/gtxorbknrw.html

SELECT id, name FROM users;
来源：http://hz.yongpay.top/gtpteeewmo.html

[Q17] 条件查询
来源：http://hz.yonumen.top/gtsxpbpkmd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhijiandao.cn/gtgzouukkt.html

[Q18] 模糊匹配
来源：http://hz.pengpengdd.cyou/gtoiizyxib.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtzqbrywxz.html

[Q19] 范围查询
来源：http://hz.jqgufenzy.top/gttnpkrebp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhixingplan.top/gtldfmkhui.html

[Q20] IN 列表
来源：http://hz.gaohongyu789.top/gtjjrlrbze.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.wangdashe.top/gtahnoqnqc.html

[Q21] 空值判断
来源：http://hz.hammf.cn/gtyyyvepbo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jianghu66.top/gtvecoqsyr.html

[Q22] 排序
来源：http://hz.ybcxt.top/gtetojpzib.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guannengcc.top/gtaazdjifa.html

[Q23] 分页
来源：http://hz.aizwys.cn/gtyitjjxvg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aibaodan.cn/gtcpoympea.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gtdsestvze.html

SELECT DISTINCT city FROM users;
来源：http://hz.jyoumei.cn/gthricmbil.html

[Q25] 只取前 N 条
来源：http://hz.daria6918.cn/gtancbezzf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gtmbovwpkd.html

[Q26] 计数
来源：http://hz.havefunace.top/gtpdvtwdjf.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtkmbqwzby.html

[Q27] 条件计数
来源：http://hz.yj20258.top/gtiyhayicq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ehwqpu.com/gtzzxyvgot.html

[Q28] 求和与平均
来源：http://hz.c1oappe.top/gtyodtoyfy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenzaomai.com/gtvpgiunue.html

[Q29] 最大最小值
来源：http://hz.feifeiyinyue.top/gtypleorsl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fengsongda.top/gtyrnvwyqz.html

[Q30] 分组统计
来源：http://hz.yuanzhike.top/gtrcwebiio.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtaesdvifi.html

[Q31] 分组后过滤
来源：http://hz.ywan-chungtsiang.top/gtqbsiamxj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guowangkeji.top/gtktnkllri.html

[Q32] 分组拼接字符串
来源：http://hz.sweek.top/gtnklqxakv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtpnwknrza.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tianlin.xyz/gtopzlrpxk.html

[Q33] 多列分组
来源：http://hz.yj20258.top/gteddptndb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.haohaochexian.top/gtsjulqabz.html

[Q34] 每组取第一条
来源：http://hz.aibaodan.cn/gtmcfuhcxl.html

SELECT * FROM (
来源：http://hz.jlsjyb.cn/gtomqkrayw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.svipenyu.cn/gtqilcgtgo.html

) t WHERE rn = 1;
来源：http://hz.jianghu66.top/gtaazpbtjl.html

[Q35] 内连接
来源：http://hz.tanke756.top/gtvvdmeaet.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtdqixcbzu.html

[Q36] 左连接
来源：http://hz.xylfe.cn/gtbdzmmpew.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtbaibencm.html

[Q37] 右连接
来源：http://hz.0kj1m.cn/gtulibfcbo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xingfuxueyuan.xyz/gtxplfrjcn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtrsgraepx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jyoumei.cn/gtsghaltcf.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxinkj.top/gtddpiutdu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinghuilouyu.cn/gtmqjafxsx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.0kj1m.cn/gtpkxvttrx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hfpthk.cn/gtgodohrep.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.quarkkingdee.top/gtnmftqvym.html

[Q41] 多表连接
来源：http://hz.jlsjyb.cn/gtktajlssi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhiwuduotai.top/gtxpzpsxdg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.dashuyun.cn/gtujqlqfog.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuetiantiany.cn/gtnhhopywu.html

[Q42] 连接条件附加过滤
来源：http://hz.jiagoushi.top/gtptewqcpj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sysykeji.top/gtmucnoixo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yueranfly.top/gtqfftemdz.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gtkxtqdfgf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jqgufenzy.top/gtvhdgxtrt.html

[Q44] IN 子查询
来源：http://hz.pycfn.com/gtxbgqlait.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangtech.top/gtzisyikot.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtwvlprzyr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtyfzvkagm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigufen.top/gtgjqzcgre.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenjidiqi.icu/gtgefjxnst.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtxkjynhyp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sufxvd.cn/gtbitwuvxw.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtwnbzlkas.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ppjwa.cn/gtkovzsebm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tanke756.top/gtfgzdlcak.html

[Q49] 更新单行
来源：http://hz.xuetiantiany.cn/gtgakialhb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yangfankeji.com/gtsgbzapmp.html

[Q50] 批量更新
来源：http://hz.hongshengwenyu.top/gtqdtkikmh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sweek.top/gtbaheijky.html

[Q51] 用子查询更新
来源：http://hz.jinqigufen.top/gtajtmuyvy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtmhdxtuvk.html

[Q52] 删除指定行
来源：http://hz.ywan-chungtsiang.top/gtjdpuawah.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxinkj.top/gtlslprbcv.html

[Q53] 按条件删除
来源：http://hz.birdmap.top/gtuuseyozh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.smart0.xyz/gthsjaqtli.html

[Q54] 清空表
来源：http://hz.iojbl.cn/gtnhmnqpas.html

TRUNCATE TABLE logs;
来源：http://hz.jqgufenzy.top/gtcvkuqkiq.html

[Q55] 排名（并列占位）
来源：http://hz.dashuyun.cn/gtujsbozwa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guannengcc.top/gtagugvzjj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258888.top/gtkdwjfwyu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cdnleiting.top/gtifzpklkh.html

[Q57] 行号
来源：http://hz.wangdashe.top/gtczzsbuyi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenjidiqi.icu/gtwsdspmma.html

[Q58] 累计求和
来源：http://hz.jqgufenzy.top/gteokhoiix.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ivvv.top/gtvuqeurgk.html

[Q59] 分组内累计
来源：http://hz.xuetiantiany.cn/gtfcuxlfrb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ivvv.top/gtcqyldvaf.html

[Q60] 取上一行 / 下一行
来源：http://hz.yanxiufei.cn/gtdoyliljl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hywenlv.cn/gtlhhqlfjb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtdymcwrym.html

[Q61] 移动平均
来源：http://hz.yj20258888.top/gtindhkstx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenzaomai.com/gtrxjcwzgp.html

[Q62] 分组占比
来源：http://hz.vqdsnc.cn/gtavnsylut.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtdacmemkn.html

[Q63] 开启事务
来源：http://hz.yuanzhike.top/gtuyfbudap.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtkvscosrl.html

[Q64] 提交事务
来源：http://hz.jinyuanbaomall.cn/gtzcsugckb.html

COMMIT;
来源：http://hz.iojbl.cn/gttgorjjsj.html

[Q65] 回滚事务
来源：http://hz.tanke756.top/gtervkinqz.html

ROLLBACK;
来源：http://hz.ehwqpu.com/gtkieesmnt.html

[Q66] 行锁查询
来源：http://hz.chenzaomai.com/gtscgzxsex.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gtjkybqvbh.html

[Q67] 设置隔离级别
来源：http://hz.ydzc1.top/gtxxnncipc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ydzc1.top/gtaopzrmhl.html

[Q68] 保存点
来源：http://hz.wangshuangyany.cn/gtffzbfcfv.html

SAVEPOINT sp1;
来源：http://hz.svipenyu.cn/gthvmzfwxa.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtfvflihkd.html

[Q69] 查看执行计划
来源：http://hz.zhoulong.xyz/gtzyjcymju.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxinkj.top/gtbfgionzd.html

[Q70] 更新统计信息
来源：http://hz.fengsongda.top/gtzweupejn.html

ANALYZE TABLE users;
来源：http://hz.feifeiyinyue.top/gtqatioqwi.html

[Q71] 查看建表语句
来源：http://hz.sxryk.cn/gtzflgbnmr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daria6918.cn/gtqaeicmwc.html

[Q72] 查看索引
来源：http://hz.jqgufenzy.top/gtuysxkrla.html

SHOW INDEX FROM users;
来源：http://hz.chenlongwang.top/gtxkmqqcfc.html

[Q73] 查看表状态
来源：http://hz.cdnleiting.top/gtomacdtga.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guannengcc.top/gtiwqqxetu.html

[Q74] 强制使用索引
来源：http://hz.dashuyun.cn/gtexdantdz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.birdmap.top/gtmfnedgdv.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gtaioeeuld.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.vqdsnc.cn/gthvyieabz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gtvzifstqh.html

[Q76] 按天统计
来源：http://hz.gogol.net.cn/gtftwvgyoo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sxryk.cn/gtuqbpukjl.html

[Q77] 时间加减
来源：http://hz.vqdsnc.cn/gtpeakolib.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydjk.org.cn/gtxibptgsm.html

[Q78] 当前时间
来源：http://hz.iojbl.cn/gtolmakwvb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dianchejie.cn/gtsxpflvhw.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangtech.top/gtfgetzvjr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinghuilouyu.cn/gtepxzgpyk.html

[Q80] 字符串截取
来源：http://hz.fzhhl.top/gtearsnitq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtbjwstcii.html

[Q81] 字符串替换
来源：http://hz.quarkkingdee.top/gtqlycpscb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.0kj1m.cn/gtxumlfyqh.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtflpiqzbl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zdqjudy.top/gtutpyjily.html

[Q83] 大小写转换
来源：http://hz.yonumen.top/gtwnxsljxl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.52xcode.cn/gtqzxpxzql.html

[Q84] 去除首尾空格
来源：http://hz.jlsjyb.cn/gtqhywhvqn.html

SELECT TRIM(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gteykhpujk.html

[Q85] 数值取整
来源：http://hz.havefunace.top/gtzkbozzrs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.c1oappe.top/gtwgjmkkkq.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxinkj.top/gtxwmqxltd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cucudq.cn/gtamilvugg.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gtxfolqkgi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinyuanbaomall.cn/gtoehvsxma.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangdashe.top/gtjnontpqx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hywenlv.cn/gtngpxdcqb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhoulong.xyz/gteoheprrv.html

[Q89] 判断表是否存在
来源：http://hz.feifeiyinyue.top/gtulmyvjhb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.52xcode.cn/gtbzqjwxyx.html

[Q90] 生成序号列
来源：http://hz.gzhubu.top/gtvocsbllk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yanxiufei.cn/gtznzbpnze.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtiyqiegoi.html

R. Bash 专题
来源：http://hz.ehwqpu.com/gtfkimrozv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtvgdnrrds.html

[R01] shebang 与严格模式
来源：http://hz.gzhubu.top/gtveqdqciv.html

#!/usr/bin/env bash
来源：http://hz.vqdsnc.cn/gtdeddzwvp.html

set -euo pipefail
来源：http://hz.shzxlz.cn/gtngavjlgi.html

[R02] 变量赋值与使用
来源：http://hz.c1oappe.top/gtrwpuzsmr.html

name="Tom"; echo "$name"
来源：http://hz.chenzaomai.com/gtejznexjw.html

[R03] 只读变量
来源：http://hz.feifeiyinyue.top/gtmnbpllhh.html

readonly PI=3.14
来源：http://hz.jianghu66.top/gtdmjetmak.html

[R04] 位置参数
来源：http://hz.chenzaomai.com/gtbbbywoxo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xinyue.icu/gthutddvtm.html

[R05] 参数默认值
来源：http://hz.ehwqpu.com/gtxywcwjof.html

name="${1:-default}"
来源：http://hz.ydzc1.top/gteguhlkkd.html

[R06] 判断命令是否存在
来源：http://hz.nanxinkj.top/gtiplrfnbp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.quarkkingdee.top/gttmlpnvkl.html

[R07] if 判断文件
来源：http://hz.gzhubu.top/gtcwnfgpyv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cashguo.top/gtuyjnvmvi.html

[R08] 数值比较
来源：http://hz.jinghuilouyu.cn/gttepvbrat.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cashguo.top/gtfsmvjeih.html

[R09] 字符串比较
来源：http://hz.jiagoushi.top/gthjftbkrr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gtaxfyeefp.html

[R10] 正则匹配
来源：http://hz.shanyushiyangtech.top/gtkseemvtv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hammf.cn/gtyxmnmxeb.html

[R11] case 多分支
来源：http://hz.yangfankeji.com/gtelbkrjzv.html

case "$1" in
来源：http://hz.zhijiandao.cn/gtnpbninlz.html

start) echo "启动" ;;
来源：http://hz.gzhubu.top/gtpbqyojlk.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gtvthqtxhy.html

*)     echo "未知命令" ;;
来源：http://hz.ybcxt.top/gtianjyihu.html

esac
来源：http://hz.zhiwuduotai.top/gtjbzxbdzi.html

[R12] for 遍历文件
来源：http://hz.meibo888.top/gtcfowvytb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.quarkkingdee.top/gtupmsyhoe.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gtmogyoqhm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jiagoushi.top/gtkaiskafg.html

[R14] C 风格 for
来源：http://hz.nanxinkj.top/gtjtthjxbb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yuanzhike.top/gtnwfclsax.html

[R15] while 逐行读文件
来源：http://hz.wangshuangyany.cn/gtpdwweqox.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtldczrxjf.html

[R16] until 等待条件
来源：http://hz.wangshuangyany.cn/gtwhjktwla.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fengsongda.top/gtgweuefuy.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtxayyqlcm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydzc1.top/gtcfwtkxgc.html

[R18] 遍历数组
来源：http://hz.jinyuanbaomall.cn/gttqpaflqg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtqaamlqof.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtivktgajs.html

echo "${#arr[@]}"
来源：http://hz.andypj.xyz/gtzlosaqxe.html

[R20] 关联数组（字典）
来源：http://hz.yuanzhike.top/gtsegmovbs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dashuyun.cn/gtbmbcegjz.html

[R21] 字符串长度
来源：http://hz.zhongyouzk.top/gtxdtqihrq.html

echo "${#s}"
来源：http://hz.hongshengwenyu.top/gtztmstjli.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtixrxfkbi.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gtxfopftht.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtckrbsukk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.52xcode.cn/gtinlamilt.html

[R24] 大小写转换
来源：http://hz.zhijiandao.cn/gtbfcrsday.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhixingplan.top/gtyadbplen.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gtfyttbhka.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xingfuxueyuan.xyz/gtjdrzqfyi.html

[R26] 命令替换
来源：http://hz.dashuyun.cn/gtkxhglnnj.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtumqaiwdd.html

[R27] 算术展开
来源：http://hz.jinqigfzy.top/gteiylgdtg.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gtrrxmgyje.html

[R28] 浮点运算
来源：http://hz.daxiang520.top/gtwubnvhxn.html

echo "scale=2; 10/3" | bc
来源：http://hz.tianlin.xyz/gthsmiozka.html

[R29] 定义函数
来源：http://hz.zhiwuduotai.top/gtnmnpwwil.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.haohaochexian.top/gtvdxlgmyp.html

[R30] 函数返回状态码
来源：http://hz.cucudq.cn/gtgmonozmd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tianlin.xyz/gtsplvlgxz.html

[R31] 局部变量
来源：http://hz.yueranfly.top/gtzistzwev.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtfflugjve.html

[R32] 参数个数校验
来源：http://hz.9152youxi.cn/gtxlvwgbar.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cheryme.top/gtoykgaawa.html

[R33] 捕获错误并提示行号
来源：http://hz.zycfv.cn/gtbeazuznf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tanke756.top/gtfjljpxzj.html

[R34] 退出时清理
来源：http://hz.xuanzx.com/gtexjlcbnv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtkaczsyju.html

[R35] 后台执行并等待
来源：http://hz.redwolf501.top/gtvisesuye.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtayxpilbw.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtsotlirha.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.daxiang520.top/gtadtqhkxx.html

[R37] 把输出赋给变量
来源：http://hz.xingfuxueyuan.xyz/gtqcctvxvv.html

files=$(ls -1)
来源：http://hz.zhongyouzk.top/gtolrybepb.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gthwerhczf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxinkj.top/gtpefjovlu.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gtkzrptzag.html

cmd > out.log 2>&1
来源：http://hz.cucudq.cn/gtdafkhcjl.html

[R40] 追加写日志
来源：http://hz.tanke756.top/gtnqnbpfzt.html

echo "log" >> out.log
来源：http://hz.yuxming.cn/gtjuspniqw.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gtgyrjvzxk.html

cmd >/dev/null 2>&1
来源：http://hz.shzxlz.cn/gtuzpakxji.html

[R42] 输入重定向
来源：http://hz.bjfxy.top/gtgdiadxsu.html

wc -l < a.txt
来源：http://hz.nanxuanxn.top/gttdbyphvw.html

[R43] 按名字查找文件
来源：http://hz.yongpay.top/gtgpekbxav.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangtech.top/gtsxqcxubh.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangkeji.top/gtrnisbvzn.html

find . -mtime -7 -type f
来源：http://hz.dianchejie.cn/gtwiolmgzj.html

[R45] 批量删除
来源：http://hz.hywenlv.cn/gtbryujrul.html

find . -name "*.tmp" -delete
来源：http://hz.xuetiantiany.cn/gtkgjxotpx.html

[R46] 递归替换文件内容
来源：http://hz.cdnleiting.top/gtqmhxlrjv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.bjfxy.top/gtuupwgupi.html

[R47] sed 单行替换
来源：http://hz.haohaochexian.top/gtvnelyhhe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhaomingkeji.xyz/gtirgrovzx.html

[R48] awk 取指定列
来源：http://hz.sufxvd.cn/gtsyqxkfqv.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenzaomai.com/gtfamslwrc.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtgjeafmsq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxuanxn.top/gteejkdscg.html

[R50] awk 求和
来源：http://hz.yongpay.top/gtgptguivb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sysykeji.top/gtzrspykxq.html

[R51] 排序去重取前几
来源：http://hz.zhongyouzk.top/gtefketroq.html


<!-- 参考信息 -->