代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.feifeiyinyue.top/gtjnmjzceb.html

);
来源：http://hz.9152youxi.cn/gtcdpsixwm.html

[Q02] 创建带外键的表
来源：http://hz.tanke756.top/gtcqkypjqj.html

CREATE TABLE orders (
来源：http://hz.andypj.xyz/gtnymibsmj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sweek.top/gtyjrsekqw.html

user_id INT NOT NULL,
来源：http://hz.chenzaomai.com/gtcymxypuy.html

amount DECIMAL(10, 2),
来源：http://hz.316326.xyz/gtbexicybb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtddemlzxx.html

);
来源：http://hz.xziqi.cn/gtvttktlkm.html

[Q03] 增加列
来源：http://hz.tanke756.top/gtlfxyfwzr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhiwuduotai.top/gtdctqjmdl.html

[Q04] 修改列类型
来源：http://hz.sysykeji.top/gtfegigyyj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xuetiantiany.cn/gtehkckibj.html

[Q05] 重命名列
来源：http://hz.andypj.xyz/gtgdlzadkn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtcghtdadh.html

[Q06] 删除列
来源：http://hz.hammf.cn/gthmvovbkt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgufenzy.top/gttnmfhnzq.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gtlkdsljfe.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gogol.net.cn/gtwndtgain.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtsudjntya.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yvedp.cn/gtdybutscc.html

[Q09] 创建唯一索引
来源：http://hz.zhengqikj.top/gtgdxxrked.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yvedp.cn/gtolgebxkt.html

[Q10] 插入单行
来源：http://hz.hfpthk.cn/gtvwosovsv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cheryme.top/gtwrewkmpu.html

[Q11] 一次插入多行
来源：http://hz.zhongyouzk.top/gtnynvrypf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangshuangyany.cn/gtfqfjumxf.html

[Q12] 插入后取自增 ID
来源：http://hz.pengpengdd.cyou/gtcxmospsp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gtpzhzcocn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hfpthk.cn/gtyyfmmuus.html

[Q13] 忽略重复插入
来源：http://hz.shangyingyoupin.top/gteaezuyns.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.c1oappe.top/gtbpaywhvj.html

[Q14] 存在则更新（upsert）
来源：http://hz.yanxiufei.cn/gtlojylbhz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zycfv.cn/gtnyeanywh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinyuanbaomall.cn/gtckpersfm.html

[Q15] 查询全部
来源：http://hz.fengsongda.top/gtchzsflwj.html

SELECT * FROM users;
来源：http://hz.316326.xyz/gtmiunpdud.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gtynlgxreb.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gttvlkufjp.html

[Q17] 条件查询
来源：http://hz.shanyushiyangkeji.top/gtqoqjhsec.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenlongwang.top/gttibfsanw.html

[Q18] 模糊匹配
来源：http://hz.quarkkingdee.top/gtcaibnlzo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenjidiqi.icu/gtxpkkapea.html

[Q19] 范围查询
来源：http://hz.guowangkeji.top/gtutvmfbkz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sweek.top/gttawbukih.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gtjwcoblem.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xziqi.cn/gtftouigpz.html

[Q21] 空值判断
来源：http://hz.quarkkingdee.top/gtfjlpfdql.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zycfv.cn/gtxnhjriyt.html

[Q22] 排序
来源：http://hz.daria6918.cn/gtxlwpmyvc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.andypj.xyz/gtossxbjax.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gtfejxlkzj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.fzhhl.top/gtjutawiui.html

[Q24] 去重
来源：http://hz.zhiwuduotai.top/gtzxevbxic.html

SELECT DISTINCT city FROM users;
来源：http://hz.jlsjyb.cn/gtxbjcciud.html

[Q25] 只取前 N 条
来源：http://hz.sysykeji.top/gtieveeofm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gtcyzqimqa.html

[Q26] 计数
来源：http://hz.daria6918.cn/gtdncbkncm.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinqigfzy.top/gtpsfqeljx.html

[Q27] 条件计数
来源：http://hz.sysykeji.top/gtprlirxwu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ehwqpu.com/gtuqbltwzz.html

[Q28] 求和与平均
来源：http://hz.c1oappe.top/gthvxqlmgo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gtlndukbkf.html

[Q29] 最大最小值
来源：http://hz.316326.xyz/gtvvfndrqv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258888.top/gtuqsecipm.html

[Q30] 分组统计
来源：http://hz.birdmap.top/gtzqukezwn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtlnlswoku.html

[Q31] 分组后过滤
来源：http://hz.xuanzx.com/gteumqycvs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.dianchejie.cn/gtzykmiyal.html

[Q32] 分组拼接字符串
来源：http://hz.tianlin.xyz/gtepcunlyg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtowobvoos.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.52xcode.cn/gtzyyvdygg.html

[Q33] 多列分组
来源：http://hz.svipenyu.cn/gtzoxnbrdz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhoulong.xyz/gtsyzkedtj.html

[Q34] 每组取第一条
来源：http://hz.jinqigfzy.top/gtspxxupkk.html

SELECT * FROM (
来源：http://hz.yongpay.top/gtosjagrqq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.52xcode.cn/gtcruisxpr.html

) t WHERE rn = 1;
来源：http://hz.ydjk.org.cn/gtrxfrunlv.html

[Q35] 内连接
来源：http://hz.ppjwa.cn/gtazcjwwul.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.0kj1m.cn/gthgpyklnz.html

[Q36] 左连接
来源：http://hz.aizwys.cn/gtigkabech.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtnhwtyieo.html

[Q37] 右连接
来源：http://hz.dianchejie.cn/gtieifebtr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sxryk.cn/gtiftzjxhg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtnfokntkc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ehwqpu.com/gtymsmztlq.html

[Q39] 自连接（查上下级）
来源：http://hz.yvedp.cn/gtfuphrajp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtprhbfcdk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.316326.xyz/gtiwetwccg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yangfankeji.com/gtmlplyjda.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sweek.top/gttozyetzu.html

[Q41] 多表连接
来源：http://hz.iojbl.cn/gtjmsspjtg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangtech.top/gtusfhjpca.html

JOIN users u ON u.id = o.user_id
来源：http://hz.9152youxi.cn/gtdaxxdffx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xinyue.icu/gtqaikpkxo.html

[Q42] 连接条件附加过滤
来源：http://hz.daxiang520.top/gthqdehifs.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shangyingyoupin.top/gtigeuoara.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtpkrnkxgi.html

[Q43] 标量子查询
来源：http://hz.xinyue.icu/gtbuxzfdbn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenlongwang.top/gtpyxhhadz.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtxmbqjxyr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.iojbl.cn/gtovsqiebf.html

[Q45] EXISTS 判断存在
来源：http://hz.zhiwuduotai.top/gtefzvabju.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gtoawketct.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hywenlv.cn/gtyamnujqf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtqxnpjepx.html

[Q47] 与平均值比较
来源：http://hz.andypj.xyz/gtkydtcwlk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cashguo.top/gtgqxfcwct.html

[Q48] CTE 公用表表达式
来源：http://hz.cucudq.cn/gtkbngopgy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.havefunace.top/gtgfmlxyrs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.kuanghao11.cn/gtmvawkvnk.html

[Q49] 更新单行
来源：http://hz.yanxiufei.cn/gtpgkqdmgf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtbncpsbul.html

[Q50] 批量更新
来源：http://hz.zycfv.cn/gtzsugpric.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.iojbl.cn/gteoihjwzb.html

[Q51] 用子查询更新
来源：http://hz.yuanzhike.top/gtonjwrysz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnxiangtu.top/gtuycmviol.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtsgtroxfs.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtpbzmscsy.html

[Q53] 按条件删除
来源：http://hz.52xcode.cn/gtkpgsxunb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aizwys.cn/gtbdexsmxd.html

[Q54] 清空表
来源：http://hz.nanxuanxn.top/gtaafdlqgt.html

TRUNCATE TABLE logs;
来源：http://hz.guannengcc.top/gtztzowsow.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtctfvxgny.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnxiangtu.top/gtyjxjfdzl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sxryk.cn/gtznlxohcj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinyuanbaomall.cn/gthtgonjej.html

[Q57] 行号
来源：http://hz.zhongyouzk.top/gtkcjbcrpf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.smart0.xyz/gtwrfdcoce.html

[Q58] 累计求和
来源：http://hz.xuetiantiany.cn/gtfbwlghvp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xziqi.cn/gtlgxfkixf.html

[Q59] 分组内累计
来源：http://hz.yuanzhike.top/gtsrimeflz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gogol.net.cn/gtowbkydtj.html

[Q60] 取上一行 / 下一行
来源：http://hz.redwolf501.top/gtmjfngskg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zycfv.cn/gttttvktad.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tanke756.top/gtbvykjuby.html

[Q61] 移动平均
来源：http://hz.cqqwz.cn/gtrspdoqpj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hongshengwenyu.top/gtkcbzctgs.html

[Q62] 分组占比
来源：http://hz.jyoumei.cn/gtbrmzrvbw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtsjkuhwun.html

[Q63] 开启事务
来源：http://hz.tian-w.cn/gtypojwtoe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.iojbl.cn/gtaokzzwlb.html

[Q64] 提交事务
来源：http://hz.shanyushiyangkeji.top/gtvqvgoyis.html

COMMIT;
来源：http://hz.jinqigufen.top/gtzxfmgajl.html

[Q65] 回滚事务
来源：http://hz.daria6918.cn/gteeegcdkq.html

ROLLBACK;
来源：http://hz.hnqzz.top/gttsgfzkiw.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtpgissent.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xingfuxueyuan.xyz/gtctwhowmk.html

[Q67] 设置隔离级别
来源：http://hz.ydzc1.top/gtmrawypun.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ehwqpu.com/gtjqwfgytz.html

[Q68] 保存点
来源：http://hz.yonumen.top/gtpcptiwvz.html

SAVEPOINT sp1;
来源：http://hz.cashguo.top/gtzrkehckp.html

ROLLBACK TO sp1;
来源：http://hz.chenjidiqi.icu/gthjjfjgms.html

[Q69] 查看执行计划
来源：http://hz.jianghu66.top/gtdmqgizhw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jlsjyb.cn/gtsgswyxls.html

[Q70] 更新统计信息
来源：http://hz.xuetiantiany.cn/gtmcxnxlcq.html

ANALYZE TABLE users;
来源：http://hz.pengpengdd.cyou/gtndxjlllg.html

[Q71] 查看建表语句
来源：http://hz.jianghu66.top/gtrifetugu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shanyushiyangtech.top/gtsqpdcmel.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtnseobddl.html

SHOW INDEX FROM users;
来源：http://hz.hongshengwenyu.top/gtkuztdvsy.html

[Q73] 查看表状态
来源：http://hz.jlsjyb.cn/gtnhbhnacy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ivvv.top/gtxzuigjtu.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtnpryimxd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtynmmvfzn.html

[Q75] 日期格式化
来源：http://hz.nwbrower.top/gtdqpxolpt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tanke756.top/gtgjguczig.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258888.top/gtnnzxodls.html

[Q76] 按天统计
来源：http://hz.sysykeji.top/gtavayofrn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daria6918.cn/gtakykhoiw.html

[Q77] 时间加减
来源：http://hz.pengpengdd.cyou/gtlgcgbjmn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangshuangyany.cn/gtgpoldueo.html

[Q78] 当前时间
来源：http://hz.jinqigufen.top/gtquvxovxp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenzaomai.com/gtblrkjabf.html

[Q79] 字符串拼接
来源：http://hz.jianghu66.top/gtifoopqbo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhixingplan.top/gtnsmljawy.html

[Q80] 字符串截取
来源：http://hz.316326.xyz/gttxfpapjl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daria6918.cn/gtscgyannr.html

[Q81] 字符串替换
来源：http://hz.aizwys.cn/gtyvwqloaz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.havefunace.top/gtkbaxjsgd.html

[Q82] 字符长度与字节长度
来源：http://hz.yj202588.top/gtzhncptwa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtyzdwzgve.html

[Q83] 大小写转换
来源：http://hz.jiagoushi.top/gtqdlndiqc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtzggaguhz.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtmsrljhsb.html

SELECT TRIM(name) FROM users;
来源：http://hz.kuanghao11.cn/gtiicegjdp.html

[Q85] 数值取整
来源：http://hz.snrcjt.cn/gtqqhpgyxi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigufen.top/gtkivzawsk.html

[Q86] 读取 JSON 字段
来源：http://hz.cashguo.top/gtjcvnyrha.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtbmplfznh.html

[Q87] JSON 字段做条件
来源：http://hz.iojbl.cn/gtkwhngkyb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gteahwjofx.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhongyouzk.top/gtzpcoecnp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hammf.cn/gtqeysyvun.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgufenzy.top/gtvomjyerm.html

[Q89] 判断表是否存在
来源：http://hz.nanxuanxn.top/gtcgtnehte.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinqigfzy.top/gtsuhtykee.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtobqiczru.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hywenlv.cn/gtrdqevkjj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtxynufprd.html

R. Bash 专题
来源：http://hz.yvedp.cn/gtjaoyyxie.html

================================================================================
来源：http://hz.zhoulong.xyz/gtbsigrkna.html

[R01] shebang 与严格模式
来源：http://hz.jlsjyb.cn/gtwawerhpz.html

#!/usr/bin/env bash
来源：http://hz.jlsjyb.cn/gttlmabbnu.html

set -euo pipefail
来源：http://hz.nanxuanxn.top/gtczcnwzqk.html

[R02] 变量赋值与使用
来源：http://hz.kuanghao11.cn/gtuzxhrouy.html

name="Tom"; echo "$name"
来源：http://hz.mhx1999.top/gtwkkcmehr.html

[R03] 只读变量
来源：http://hz.snrcjt.cn/gtttnrjvpm.html

readonly PI=3.14
来源：http://hz.ehwqpu.com/gtgzurbkyv.html

[R04] 位置参数
来源：http://hz.daxiang520.top/gtexbvcxcd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fengsongda.top/gtutvravyc.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtkoxxybbb.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gtwzkexzcm.html

[R06] 判断命令是否存在
来源：http://hz.nanxinkj.top/gtvdcddflq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nwbrower.top/gtulowczkh.html

[R07] if 判断文件
来源：http://hz.cucudq.cn/gtbplweosf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.haohaochexian.top/gtredpyduh.html

[R08] 数值比较
来源：http://hz.zhoulong.xyz/gtdptrzted.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aizwys.cn/gtyqyodnnp.html

[R09] 字符串比较
来源：http://hz.haohaochexian.top/gtopwfikfo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daxiang520.top/gtjdlmueph.html

[R10] 正则匹配
来源：http://hz.zhoulong.xyz/gtsyiuppby.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sysykeji.top/gtwuqzadyc.html

[R11] case 多分支
来源：http://hz.cqqwz.cn/gtmvbytjum.html

case "$1" in
来源：http://hz.chenlongwang.top/gtneijikjc.html

start) echo "启动" ;;
来源：http://hz.chenjidiqi.icu/gtdkbaycqr.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtsmpcgacb.html

*)     echo "未知命令" ;;
来源：http://hz.havefunace.top/gtzxmbbsqx.html

esac
来源：http://hz.yj20258.top/gtomzrulzm.html

[R12] for 遍历文件
来源：http://hz.xuanzx.com/gtnfqexhgw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigufen.top/gthkkkglaz.html

[R13] for 计数循环
来源：http://hz.316326.xyz/gtxhrvcdhr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tianlin.xyz/gtxvbxzbpe.html

[R14] C 风格 for
来源：http://hz.xziqi.cn/gtxuscqgrs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtjldzvcbo.html

[R15] while 逐行读文件
来源：http://hz.zhoulong.xyz/gtyaukyavg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtjhoerkmb.html

[R16] until 等待条件
来源：http://hz.aizwys.cn/gthuggbqei.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dianchejie.cn/gtagcvdoqy.html

[R17] 数组定义与取值
来源：http://hz.cdnleiting.top/gtstcfjefw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cashguo.top/gtdotnajpk.html

[R18] 遍历数组
来源：http://hz.shzxlz.cn/gterdhnkqw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dashuyun.cn/gtcxusjdca.html

[R19] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtmnxqxwnp.html

echo "${#arr[@]}"
来源：http://hz.quarkkingdee.top/gtwwyhsbta.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtkllcraph.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jyoumei.cn/gtimcmosxp.html

[R21] 字符串长度
来源：http://hz.zhiwuduotai.top/gtbukqoybu.html

echo "${#s}"
来源：http://hz.quarkkingdee.top/gtsuwrwfbq.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtbveyzvcp.html

echo "${s:0:5}"
来源：http://hz.zhiwuduotai.top/gtgsaaxnjt.html

[R23] 字符串替换
来源：http://hz.shangyingyoupin.top/gtwoxjeiaa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhijiandao.cn/gtzxedzrri.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gtznkorwpk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hongshengwenyu.top/gtztzlxdlj.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gtourdkyvf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aibaodan.cn/gtosenzxrw.html

[R26] 命令替换
来源：http://hz.pycfn.com/gtgfdhltgc.html

now=$(date +%F); echo "$now"
来源：http://hz.daria6918.cn/gtzjahvdcg.html

[R27] 算术展开
来源：http://hz.redwolf501.top/gtoyfadpyy.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangtech.top/gtweqxnuxs.html

[R28] 浮点运算
来源：http://hz.snrcjt.cn/gtfnybjwsw.html

echo "scale=2; 10/3" | bc
来源：http://hz.yonumen.top/gtwewecoqm.html

[R29] 定义函数
来源：http://hz.cqqwz.cn/gtlmiedkxf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.snrcjt.cn/gtwkcgawut.html

[R30] 函数返回状态码
来源：http://hz.xylfe.cn/gttapndiml.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.feifeiyinyue.top/gtjxiuftbd.html

[R31] 局部变量
来源：http://hz.316326.xyz/gtxdwxosqx.html

f() { local x=1; echo "$x"; }
来源：http://hz.mhx1999.top/gterpfiaaw.html

[R32] 参数个数校验
来源：http://hz.ywan-chungtsiang.top/gtfwzlrdbw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cucudq.cn/gtrpaabpmk.html

[R33] 捕获错误并提示行号
来源：http://hz.yanxiufei.cn/gtmoovpkmn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgufenzy.top/gtvbtcejhn.html

[R34] 退出时清理
来源：http://hz.xingfuxueyuan.xyz/gthoahwode.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuetiantiany.cn/gtngdfncvj.html

[R35] 后台执行并等待
来源：http://hz.zycfv.cn/gthlfgwhsh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shangyingyoupin.top/gtoojeatud.html

[R36] 并发执行多个任务
来源：http://hz.xuetiantiany.cn/gtkjnzwtlk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxuanxn.top/gtudeonnsl.html

[R37] 把输出赋给变量
来源：http://hz.mhx1999.top/gtankfexsm.html

files=$(ls -1)
来源：http://hz.0kj1m.cn/gtwciyrkkh.html

[R38] 管道串联
来源：http://hz.yuxming.cn/gtgcbsrhly.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuxming.cn/gtcxnfmrcc.html

[R39] 重定向标准输出与错误
来源：http://hz.yuanzhike.top/gtvdketbvj.html

cmd > out.log 2>&1
来源：http://hz.ppjwa.cn/gtcfhffzrk.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtdctulwbp.html

echo "log" >> out.log
来源：http://hz.yonumen.top/gthybjqjcw.html

[R41] 丢弃输出
来源：http://hz.guannengcc.top/gtyaympffc.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gthnvrarjz.html

[R42] 输入重定向
来源：http://hz.yonumen.top/gtlejpaspl.html

wc -l < a.txt
来源：http://hz.yonumen.top/gtfqdzfqja.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gthcmxnehy.html

find . -name "*.log" -type f
来源：http://hz.quarkkingdee.top/gtxgncuzfl.html

[R44] 按修改时间查找
来源：http://hz.jinqigufen.top/gtylccbbec.html

find . -mtime -7 -type f
来源：http://hz.jlsjyb.cn/gtjtltpxwu.html

[R45] 批量删除
来源：http://hz.hysaishi.cn/gtrzahvbpu.html

find . -name "*.tmp" -delete
来源：http://hz.cucudq.cn/gtoxfwovfk.html

[R46] 递归替换文件内容
来源：http://hz.xylfe.cn/gtxngwrdai.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yanxiufei.cn/gtbkwdvbcw.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gtvxinzhpd.html


<!-- 参考信息 -->