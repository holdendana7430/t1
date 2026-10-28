代发 wailian999

CREATE TABLE users (
来源：http://hz.xziqi.cn/gtfavksqdb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhoulong.xyz/gtwksmhcaq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xylfe.cn/gtwycjzdgl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xinyue.icu/gtanocwiqt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhixingplan.top/gtvtllffak.html

);
来源：http://hz.sweek.top/gtldspwppo.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gtlkkovbah.html

CREATE TABLE orders (
来源：http://hz.xziqi.cn/gtovzcsiqc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtytczxrms.html

user_id INT NOT NULL,
来源：http://hz.ydzc1.top/gtddkekgyl.html

amount DECIMAL(10, 2),
来源：http://hz.aibaodan.cn/gtqqxydhdf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhixingplan.top/gtrcrojywm.html

);
来源：http://hz.chenlongwang.top/gtvnrwpqht.html

[Q03] 增加列
来源：http://hz.jinghuilouyu.cn/gtdtpivoqu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hongshengwenyu.top/gtlqacfazm.html

[Q04] 修改列类型
来源：http://hz.cucudq.cn/gtahwsjbvh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigfzy.top/gtwscpkcwg.html

[Q05] 重命名列
来源：http://hz.sxryk.cn/gtinckyekg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.snrcjt.cn/gthsfogktx.html

[Q06] 删除列
来源：http://hz.daria6918.cn/gtgbmmuumu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.0kj1m.cn/gtchltdrmq.html

[Q07] 删除表
来源：http://hz.gzhubu.top/gtrajvexav.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aibaodan.cn/gtrjgsyuis.html

[Q08] 创建普通索引
来源：http://hz.gotoacloud.top/gtgjlnvrya.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtnlclybht.html

[Q09] 创建唯一索引
来源：http://hz.guowangkeji.top/gtmyzzwoyd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sysykeji.top/gtlsfqfsul.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtqcwgayqb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxinkj.top/gtzwhjujdp.html

[Q11] 一次插入多行
来源：http://hz.fengsongda.top/gtoohkelki.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fzhhl.top/gtkqrxsqft.html

[Q12] 插入后取自增 ID
来源：http://hz.gaohongyu789.top/gtzwztxtpv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigfzy.top/gtydropxwl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gtmrxivlvx.html

[Q13] 忽略重复插入
来源：http://hz.nwbrower.top/gtlpqdtlsg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigufen.top/gtrzmfkygc.html

[Q14] 存在则更新（upsert）
来源：http://hz.wangshuangyany.cn/gtuhqrhedt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dianchejie.cn/gtzcmujhku.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.dianchejie.cn/gtucovqwvi.html

[Q15] 查询全部
来源：http://hz.xziqi.cn/gtikzmoaxd.html

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtylhqcxvz.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtfhcewdzb.html

SELECT id, name FROM users;
来源：http://hz.svipenyu.cn/gtsocjabac.html

[Q17] 条件查询
来源：http://hz.pycfn.com/gtibpbezud.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cqqwz.cn/gtbnrlvxxp.html

[Q18] 模糊匹配
来源：http://hz.jianghu66.top/gthdoosadm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258.top/gtydupqjsk.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gtyrrqfptq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cheryme.top/gtwujxodgd.html

[Q20] IN 列表
来源：http://hz.fengsongda.top/gtrjdzozhr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.feifeiyinyue.top/gtrfzzspho.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtwhhieclq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hywenlv.cn/gteeyghlkj.html

[Q22] 排序
来源：http://hz.hongshengwenyu.top/gtgldobqzt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtdxetqcbp.html

[Q23] 分页
来源：http://hz.zhongyouzk.top/gtbsldvuyh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258.top/gtgmwfgadq.html

[Q24] 去重
来源：http://hz.fzhhl.top/gtrdwlpzim.html

SELECT DISTINCT city FROM users;
来源：http://hz.gzhubu.top/gtetaiqnbw.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gtiodihjef.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dianchejie.cn/gtytmbnuwn.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gtuqstacdl.html

SELECT COUNT(*) FROM users;
来源：http://hz.xinyue.icu/gtmemhygyh.html

[Q27] 条件计数
来源：http://hz.xylfe.cn/gtgnaczvgd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.316326.xyz/gtrfbonvvx.html

[Q28] 求和与平均
来源：http://hz.jyoumei.cn/gtrxufbnkq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.smart0.xyz/gtyeorzpcy.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gtalwvzwja.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhoulong.xyz/gtdhevlmyn.html

[Q30] 分组统计
来源：http://hz.hnxiangtu.top/gthdmqmidy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtlewiycya.html

[Q31] 分组后过滤
来源：http://hz.gogol.net.cn/gttasyaauq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ppjwa.cn/gttlsaudpd.html

[Q32] 分组拼接字符串
来源：http://hz.yanxiufei.cn/gtvhgmmoqw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtwcdkkems.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nwbrower.top/gtobbcmqem.html

[Q33] 多列分组
来源：http://hz.jianghu66.top/gtqlouzxha.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gteejahdfe.html

[Q34] 每组取第一条
来源：http://hz.cqqwz.cn/gtqzjvywzh.html

SELECT * FROM (
来源：http://hz.daria6918.cn/gtetotsghh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sufxvd.cn/gtrdavghyr.html

) t WHERE rn = 1;
来源：http://hz.ivvv.top/gtzrerezpy.html

[Q35] 内连接
来源：http://hz.fengsongda.top/gtgtgvwqcs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtwefwiyuc.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtlwqksgst.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtnxracwks.html

[Q37] 右连接
来源：http://hz.quarkkingdee.top/gtgupjhqsb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.havefunace.top/gtiewnsyah.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jianghu66.top/gtdxatiatf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.smart0.xyz/gtzblwwwrn.html

[Q39] 自连接（查上下级）
来源：http://hz.zhixingplan.top/gtmnwjunzk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yanxiufei.cn/gteywloaoj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fzhhl.top/gtwmljxoan.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhiwuduotai.top/gtvxdesmyh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangtech.top/gtmrqtkqzd.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtynkyhpmd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hammf.cn/gtlhajlucw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtfoknrikt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gtnxksaqps.html

[Q42] 连接条件附加过滤
来源：http://hz.yueranfly.top/gtfwntljmu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shzxlz.cn/gtfpyktzrs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yvedp.cn/gtpuxuuirh.html

[Q43] 标量子查询
来源：http://hz.gotoacloud.top/gtfxrqunmt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtrylailoq.html

[Q44] IN 子查询
来源：http://hz.aibaodan.cn/gtgydeitin.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.vqdsnc.cn/gtxvvszqyi.html

[Q45] EXISTS 判断存在
来源：http://hz.zdqjudy.top/gtqxoicnni.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhixingplan.top/gtggytvuaq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuxming.cn/gtpzucbdbh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtcyqcturb.html

[Q47] 与平均值比较
来源：http://hz.zhiwuduotai.top/gtswasxdwh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.52xcode.cn/gtxwmhocio.html

[Q48] CTE 公用表表达式
来源：http://hz.yongpay.top/gtvuwhoxjw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yongpay.top/gtlwitbtga.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cqqwz.cn/gtkhgentjm.html

[Q49] 更新单行
来源：http://hz.jinqigufen.top/gtjzscihuf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhiwuduotai.top/gtacbbztmy.html

[Q50] 批量更新
来源：http://hz.jiagoushi.top/gtjnygjufb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhoulong.xyz/gtijvtociu.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtkcihochp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigufen.top/gtcntuspgj.html

[Q52] 删除指定行
来源：http://hz.dianchejie.cn/gtvdhbrngt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtjxxsvicy.html

[Q53] 按条件删除
来源：http://hz.yonumen.top/gtbqktkwyk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ppjwa.cn/gtbvuayxbo.html

[Q54] 清空表
来源：http://hz.shuidangran.top/gtejvvmste.html

TRUNCATE TABLE logs;
来源：http://hz.zycfv.cn/gtyejczuxx.html

[Q55] 排名（并列占位）
来源：http://hz.pycfn.com/gtytltsmem.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.quarkkingdee.top/gtbsddiemd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.9152youxi.cn/gtqcmopgff.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gtwcynqizi.html

[Q57] 行号
来源：http://hz.yuxming.cn/gtgzljeszi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sysykeji.top/gtocfmehof.html

[Q58] 累计求和
来源：http://hz.ivvv.top/gthwgqazrk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtlqwpager.html

[Q59] 分组内累计
来源：http://hz.xuetiantiany.cn/gtqnvlusvj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cucudq.cn/gtahdjvgrw.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydjk.org.cn/gtstazgxys.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenzaomai.com/gtkmcufexz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxuanxn.top/gtnhorimqj.html

[Q61] 移动平均
来源：http://hz.sysykeji.top/gtzzbtqlav.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtvqjalzpb.html

[Q62] 分组占比
来源：http://hz.kuanghao11.cn/gtebybsgzr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtzcgpimue.html

[Q63] 开启事务
来源：http://hz.gogol.net.cn/gtvxjtshyp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jqgfzy.top/gtggnzuckv.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gthvdqrkwc.html

COMMIT;
来源：http://hz.zhengqikj.top/gtzqyzlvug.html

[Q65] 回滚事务
来源：http://hz.hnqzz.top/gtseyvydtb.html

ROLLBACK;
来源：http://hz.shanyushiyangtech.top/gtphrdbccz.html

[Q66] 行锁查询
来源：http://hz.ivvv.top/gtzunkennk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tanke756.top/gtsgmezvuv.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gtchkqvstr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.havefunace.top/gttjqrpxsv.html

[Q68] 保存点
来源：http://hz.yuanzhike.top/gtsjigdddd.html

SAVEPOINT sp1;
来源：http://hz.wangshuangyany.cn/gtyjolfwvg.html

ROLLBACK TO sp1;
来源：http://hz.yuanzhike.top/gtlhkvemby.html

[Q69] 查看执行计划
来源：http://hz.jinqigfzy.top/gtlrhpgujz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hywenlv.cn/gtflulyvvz.html

[Q70] 更新统计信息
来源：http://hz.yanxiufei.cn/gtxbcccumq.html

ANALYZE TABLE users;
来源：http://hz.nanxinkj.top/gtklmnxrgq.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtpqqwflqq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dashuyun.cn/gtuhukzeot.html

[Q72] 查看索引
来源：http://hz.vqdsnc.cn/gtbmnblamp.html

SHOW INDEX FROM users;
来源：http://hz.yj20258.top/gtynjgzqnu.html

[Q73] 查看表状态
来源：http://hz.vqdsnc.cn/gtrxvzljce.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydzc1.top/gtljyxxqdl.html

[Q74] 强制使用索引
来源：http://hz.daria6918.cn/gttpajphaw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuxming.cn/gtkepqttuo.html

[Q75] 日期格式化
来源：http://hz.shuidangran.top/gtfclygmvo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhiwuduotai.top/gtudvqzzzc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hongshengwenyu.top/gtwlfinduk.html

[Q76] 按天统计
来源：http://hz.yuanzhike.top/gtbrxmzrrx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jianghu66.top/gtstnqmpkj.html

[Q77] 时间加减
来源：http://hz.ydjk.org.cn/gtiinlgcgm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yueranfly.top/gtfccdobff.html

[Q78] 当前时间
来源：http://hz.daxiang520.top/gtmantdfbl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yongpay.top/gttgolibpb.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtahoqnofc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gtzxeamhpu.html

[Q80] 字符串截取
来源：http://hz.wangdashe.top/gtivujrvmx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hywenlv.cn/gtgyvybjjp.html

[Q81] 字符串替换
来源：http://hz.guowangkeji.top/gtjfcmipms.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.0kj1m.cn/gtnxbgozcp.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtqisiztuo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.316326.xyz/gtdglyozgg.html

[Q83] 大小写转换
来源：http://hz.pycfn.com/gtqldnsudi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtijqovzeo.html

[Q84] 去除首尾空格
来源：http://hz.snrcjt.cn/gtxdsvksmz.html

SELECT TRIM(name) FROM users;
来源：http://hz.birdmap.top/gtzpahbrkv.html

[Q85] 数值取整
来源：http://hz.hnxiangtu.top/gthbkzzapk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.quarkkingdee.top/gtormnhbdl.html

[Q86] 读取 JSON 字段
来源：http://hz.yvedp.cn/gtknvavnum.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fengsongda.top/gtoiiifpyu.html

[Q87] JSON 字段做条件
来源：http://hz.haohaochexian.top/gtujydphct.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gtndvwarsw.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydjk.org.cn/gtqyoliify.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xinyue.icu/gtxiibhycv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenjidiqi.icu/gtbecsqvmt.html

[Q89] 判断表是否存在
来源：http://hz.316326.xyz/gtvtlqcmtz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtfvadnjwo.html

[Q90] 生成序号列
来源：http://hz.jianghu66.top/gtqivbyfxh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtmxosawpy.html

================================================================================
来源：http://hz.cucudq.cn/gtsrvbjhud.html

R. Bash 专题
来源：http://hz.guannengcc.top/gtouuafhka.html

================================================================================
来源：http://hz.zhijiandao.cn/gtfjwkscnd.html

[R01] shebang 与严格模式
来源：http://hz.yanxiufei.cn/gttazahlio.html

#!/usr/bin/env bash
来源：http://hz.xylfe.cn/gtfreuwvtq.html

set -euo pipefail
来源：http://hz.shzxlz.cn/gtfcsiizyv.html

[R02] 变量赋值与使用
来源：http://hz.yonumen.top/gtiqxphutb.html

name="Tom"; echo "$name"
来源：http://hz.feifeiyinyue.top/gtviuetgad.html

[R03] 只读变量
来源：http://hz.hammf.cn/gtjssttmxb.html

readonly PI=3.14
来源：http://hz.zycfv.cn/gtaksbmcmb.html

[R04] 位置参数
来源：http://hz.jiagoushi.top/gtviqkxxgd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yueranfly.top/gtjgplbtsr.html

[R05] 参数默认值
来源：http://hz.iojbl.cn/gtqxunhfsu.html

name="${1:-default}"
来源：http://hz.daria6918.cn/gtiexjhryu.html

[R06] 判断命令是否存在
来源：http://hz.aibaodan.cn/gtptqlyuzz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.andypj.xyz/gtyjgxofyb.html

[R07] if 判断文件
来源：http://hz.sweek.top/gtsujkwcws.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258888.top/gtylumrwdl.html

[R08] 数值比较
来源：http://hz.bjfxy.top/gtebtinnga.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cqqwz.cn/gtnfvgcuuh.html

[R09] 字符串比较
来源：http://hz.gotoacloud.top/gtzwdtlatj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtlrioeqmq.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gtetmpqsiw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shuidangran.top/gtdtiqzvbm.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtraasymva.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gtqmxekdgn.html

start) echo "启动" ;;
来源：http://hz.svipenyu.cn/gtuhaiubrj.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtaijtmfkf.html

*)     echo "未知命令" ;;
来源：http://hz.gotoacloud.top/gtbvmneyff.html

esac
来源：http://hz.gogol.net.cn/gtypxvdymq.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gtqiqiuybb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtibwvywgc.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gthviqisug.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtxbjjysju.html

[R14] C 风格 for
来源：http://hz.jiagoushi.top/gtlggwzwfa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtkgeuiylt.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtxzwdwpyu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.316326.xyz/gtjtutgrra.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gtflfsqsgf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gtzsmdjfxj.html

[R17] 数组定义与取值
来源：http://hz.ppjwa.cn/gtxzelpmqf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtlcqgqkjo.html

[R18] 遍历数组
来源：http://hz.jianghu66.top/gttrigdzxl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dianchejie.cn/gtjiibnlvb.html

[R19] 数组长度
来源：http://hz.sxryk.cn/gtsxdgfcjb.html

echo "${#arr[@]}"
来源：http://hz.guowangkeji.top/gtiuzofbbn.html

[R20] 关联数组（字典）
来源：http://hz.feifeiyinyue.top/gtqpkjezfs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ehwqpu.com/gtppbiexzw.html

[R21] 字符串长度
来源：http://hz.hysaishi.cn/gtzsiywlxa.html

echo "${#s}"
来源：http://hz.hysaishi.cn/gtjwidkoqx.html

[R22] 截取子串
来源：http://hz.birdmap.top/gtgciogdkz.html

echo "${s:0:5}"
来源：http://hz.meibo888.top/gtvnujoxvk.html

[R23] 字符串替换
来源：http://hz.cucudq.cn/gtbwtmosjy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhixingplan.top/gtsyiofmkz.html

[R24] 大小写转换
来源：http://hz.xinyue.icu/gtjfwnidta.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xziqi.cn/gtdflwnoml.html

[R25] 去后缀 / 去前缀
来源：http://hz.feifeiyinyue.top/gtfxcfauiz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtcwfxdvea.html

[R26] 命令替换
来源：http://hz.quarkkingdee.top/gtmnbxpvwi.html

now=$(date +%F); echo "$now"
来源：http://hz.hywenlv.cn/gthsrlykts.html

[R27] 算术展开
来源：http://hz.jlsjyb.cn/gtwqzwwbtl.html

echo $((1 + 2 * 3))
来源：http://hz.gaohongyu789.top/gtxhshjtqi.html

[R28] 浮点运算
来源：http://hz.kuanghao11.cn/gtalywcmwz.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gtolikhplq.html

[R29] 定义函数
来源：http://hz.ivvv.top/gtiwsdjbem.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinyuanbaomall.cn/gtizurylbg.html

[R30] 函数返回状态码
来源：http://hz.cdnleiting.top/gteucrmmjp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hammf.cn/gtczxlncfu.html

[R31] 局部变量
来源：http://hz.dashuyun.cn/gtrylmrzzs.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinyuanbaomall.cn/gttfbqcgzw.html

[R32] 参数个数校验
来源：http://hz.jinyuanbaomall.cn/gtmqdysiur.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtbfvmufoy.html

[R33] 捕获错误并提示行号
来源：http://hz.hongshengwenyu.top/gtcthjsboz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtohldgttw.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtotjpnroa.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtmtwleldf.html

[R35] 后台执行并等待
来源：http://hz.hammf.cn/gtgplxkxre.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtpwfmexqo.html

[R36] 并发执行多个任务
来源：http://hz.jlsjyb.cn/gtfnldiwrl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dianchejie.cn/gtudqycwyd.html

[R37] 把输出赋给变量
来源：http://hz.aibaodan.cn/gttvggskac.html

files=$(ls -1)
来源：http://hz.jinqigufen.top/gtxzccrean.html

[R38] 管道串联
来源：http://hz.havefunace.top/gtemchjgat.html

cat a.txt | grep -i error | wc -l
来源：http://hz.vqdsnc.cn/gtlamvhlqs.html

[R39] 重定向标准输出与错误
来源：http://hz.52xcode.cn/gtcktjamhl.html

cmd > out.log 2>&1
来源：http://hz.chenlongwang.top/gtsbsmkkyi.html

[R40] 追加写日志
来源：http://hz.andypj.xyz/gtaaabodjt.html

echo "log" >> out.log
来源：http://hz.tian-w.cn/gtsxbwaxyf.html

[R41] 丢弃输出
来源：http://hz.xingfuxueyuan.xyz/gtkopibhid.html

cmd >/dev/null 2>&1
来源：http://hz.quarkkingdee.top/gtlxdfhyam.html

[R42] 输入重定向
来源：http://hz.cdnleiting.top/gtpgbhptzl.html

wc -l < a.txt
来源：http://hz.gzhubu.top/gtybldzwkg.html

[R43] 按名字查找文件
来源：http://hz.zycfv.cn/gtrlodfalu.html

find . -name "*.log" -type f
来源：http://hz.ppjwa.cn/gtsoudvgjz.html

[R44] 按修改时间查找
来源：http://hz.chenzaomai.com/gtsmrttyso.html

find . -mtime -7 -type f
来源：http://hz.svipenyu.cn/gtimomwzqh.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gtnrtpfjkg.html


<!-- 参考信息 -->