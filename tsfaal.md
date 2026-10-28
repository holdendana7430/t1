代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtkxovanhn.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtfquulfbk.html

amount DECIMAL(10, 2),
来源：http://hz.ehwqpu.com/gtnssvcsrq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guannengcc.top/gtspiqxkht.html

);
来源：http://hz.smart0.xyz/gttdrqnmcg.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtrfgjvbto.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigfzy.top/gtzssejuxb.html

[Q04] 修改列类型
来源：http://hz.cqqwz.cn/gtbgpmmsfs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj202588.top/gtpkehyrpa.html

[Q05] 重命名列
来源：http://hz.jqgfzy.top/gtgoudtmwr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtogpbeuqy.html

[Q06] 删除列
来源：http://hz.mhx1999.top/gtoqbdgmvh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cdnleiting.top/gtatewnuyg.html

[Q07] 删除表
来源：http://hz.jqgufenzy.top/gtvidoyrgs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aizwys.cn/gtjpkhvtsl.html

[Q08] 创建普通索引
来源：http://hz.ywan-chungtsiang.top/gthleunphg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtakvecbxj.html

[Q09] 创建唯一索引
来源：http://hz.snrcjt.cn/gtcdlzsmae.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnqzz.top/gtiepmfesb.html

[Q10] 插入单行
来源：http://hz.jlsjyb.cn/gtvnqibgvg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guowangkeji.top/gtpilotfyh.html

[Q11] 一次插入多行
来源：http://hz.9152youxi.cn/gtzjyllciw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.c1oappe.top/gttiacfsuf.html

[Q12] 插入后取自增 ID
来源：http://hz.yongpay.top/gtdvpganes.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yonumen.top/gtmtwevddm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxuanxn.top/gtybelbcsa.html

[Q13] 忽略重复插入
来源：http://hz.jqgufenzy.top/gtmddxffbe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zycfv.cn/gtfoorubvs.html

[Q14] 存在则更新（upsert）
来源：http://hz.gaohongyu789.top/gtudavxgmj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.havefunace.top/gthkvasosd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yueranfly.top/gtvvdkjlov.html

[Q15] 查询全部
来源：http://hz.dianchejie.cn/gtrvyfekpc.html

SELECT * FROM users;
来源：http://hz.ydzc1.top/gtznimbjum.html

[Q16] 查询指定列
来源：http://hz.fzhhl.top/gtnesxdkca.html

SELECT id, name FROM users;
来源：http://hz.sxryk.cn/gtkzjxdhbf.html

[Q17] 条件查询
来源：http://hz.yonumen.top/gtejyebzka.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhixingplan.top/gtlaxwluhn.html

[Q18] 模糊匹配
来源：http://hz.ehwqpu.com/gtjpbveuee.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.kuanghao11.cn/gtkiskbamn.html

[Q19] 范围查询
来源：http://hz.jqgufenzy.top/gtsrtwijhq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxuanxn.top/gtytkuieqx.html

[Q20] IN 列表
来源：http://hz.gzhubu.top/gthnywtnsq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gogol.net.cn/gttckpsqma.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtwdrxsewx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtblgllhik.html

[Q22] 排序
来源：http://hz.zhongyouzk.top/gtnsegiqac.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gotoacloud.top/gtambdszuj.html

[Q23] 分页
来源：http://hz.vqdsnc.cn/gtijjqgtfa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtotrsucpk.html

[Q24] 去重
来源：http://hz.sysykeji.top/gtdwltxsbg.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenlongwang.top/gtwktncyry.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtjateooqq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhaomingkeji.xyz/gtppjihunj.html

[Q26] 计数
来源：http://hz.jiagoushi.top/gttvvdorpn.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtguvgdjwh.html

[Q27] 条件计数
来源：http://hz.ppjwa.cn/gtsbwiytdb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cdnleiting.top/gtyxagovum.html

[Q28] 求和与平均
来源：http://hz.daria6918.cn/gtgrfxkdkv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cdnleiting.top/gtvqpswznu.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gtophvptcx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxuanxn.top/gtwdkgmwmh.html

[Q30] 分组统计
来源：http://hz.shangyingyoupin.top/gtkjqxhwnx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtwuovbrnk.html

[Q31] 分组后过滤
来源：http://hz.pycfn.com/gtaarqlhsl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenjidiqi.icu/gtuvyzwjmy.html

[Q32] 分组拼接字符串
来源：http://hz.52xcode.cn/gtacyfrtik.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtwixmmzkq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.quarkkingdee.top/gttkshkjcb.html

[Q33] 多列分组
来源：http://hz.yuanzhike.top/gtvhkgxbks.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.9152youxi.cn/gtbefatwzg.html

[Q34] 每组取第一条
来源：http://hz.yj20258.top/gtprvkheew.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gtsalqizal.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xziqi.cn/gtqmbgqikl.html

) t WHERE rn = 1;
来源：http://hz.nanxinkj.top/gtirrgtilr.html

[Q35] 内连接
来源：http://hz.chenzaomai.com/gtbrifhrxc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtwkqmqltd.html

[Q36] 左连接
来源：http://hz.jiagoushi.top/gtdbkybrky.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtjjmwbogd.html

[Q37] 右连接
来源：http://hz.jqgfzy.top/gtlzzqjgov.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gtkxomphez.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.birdmap.top/gtibzogwih.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jyoumei.cn/gtkpdckxqs.html

[Q39] 自连接（查上下级）
来源：http://hz.tianlin.xyz/gtqfrwostb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hywenlv.cn/gtgxfukymm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xinyue.icu/gtpzxkqsvv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hfpthk.cn/gtqumzkwst.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinyuanbaomall.cn/gtdypionug.html

[Q41] 多表连接
来源：http://hz.tanke756.top/gttevdeumw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtpdjknkex.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenjidiqi.icu/gtzcitqvrl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zycfv.cn/gttxlrcgpe.html

[Q42] 连接条件附加过滤
来源：http://hz.smart0.xyz/gttxsccvoq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.mhx1999.top/gtamsytldg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.feifeiyinyue.top/gthpcskvta.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtagzfknhw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhixingplan.top/gtxeszpioe.html

[Q44] IN 子查询
来源：http://hz.cucudq.cn/gtneipwmtl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dianchejie.cn/gttndsbwmb.html

[Q45] EXISTS 判断存在
来源：http://hz.yvedp.cn/gtitaizmaf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gthrsuvnqh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258888.top/gtuluzeruu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtsrmvkddj.html

[Q47] 与平均值比较
来源：http://hz.cucudq.cn/gtvcbsmbca.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.smart0.xyz/gtlaqbbmah.html

[Q48] CTE 公用表表达式
来源：http://hz.zdqjudy.top/gtqdgsrgfk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xziqi.cn/gtkxnmjmet.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.kuanghao11.cn/gtejxqelyz.html

[Q49] 更新单行
来源：http://hz.shanyushiyangtech.top/gtiknkgpni.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhixingplan.top/gtizjtgswo.html

[Q50] 批量更新
来源：http://hz.xziqi.cn/gttupgpfob.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xinyue.icu/gtuxmeozgz.html

[Q51] 用子查询更新
来源：http://hz.jianghu66.top/gtngtdkurg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenlongwang.top/gtivvrgtfw.html

[Q52] 删除指定行
来源：http://hz.redwolf501.top/gtuhlpelbs.html

DELETE FROM users WHERE id = 10;
来源：http://hz.iojbl.cn/gtnzckkyul.html

[Q53] 按条件删除
来源：http://hz.zhaomingkeji.xyz/gtedyyqpyg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aizwys.cn/gtudnmfrjb.html

[Q54] 清空表
来源：http://hz.ydjk.org.cn/gtaxszdvye.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtohwqwesi.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gthmehirlh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuanzx.com/gtlzzaucml.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xylfe.cn/gtuoeggblw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtufshflqi.html

[Q57] 行号
来源：http://hz.zhongyouzk.top/gtwkbkwtak.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.snrcjt.cn/gtwurtsxes.html

[Q58] 累计求和
来源：http://hz.yj202588.top/gtnummpgga.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.meibo888.top/gtnobfslsi.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtqdeceeiy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigufen.top/gtvcwmmvce.html

[Q60] 取上一行 / 下一行
来源：http://hz.pengpengdd.cyou/gtdyzfstga.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenlongwang.top/gtlgphgajp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guannengcc.top/gtuybgsgug.html

[Q61] 移动平均
来源：http://hz.yueranfly.top/gtmilswzzb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jyoumei.cn/gtbznhrkoy.html

[Q62] 分组占比
来源：http://hz.dianchejie.cn/gtdvkhdwre.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtoppnikgp.html

[Q63] 开启事务
来源：http://hz.jinghuilouyu.cn/gtrzodvkdt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cashguo.top/gtmsyebxud.html

[Q64] 提交事务
来源：http://hz.52xcode.cn/gtkvzfegjq.html

COMMIT;
来源：http://hz.ydjk.org.cn/gtzxmcyzug.html

[Q65] 回滚事务
来源：http://hz.sufxvd.cn/gtfylczkzy.html

ROLLBACK;
来源：http://hz.meibo888.top/gtjhaoijry.html

[Q66] 行锁查询
来源：http://hz.cashguo.top/gtpspzvlgs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ppjwa.cn/gtywhjnnda.html

[Q67] 设置隔离级别
来源：http://hz.daria6918.cn/gtatrywegc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xziqi.cn/gtpldhabhr.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtboswehfe.html

SAVEPOINT sp1;
来源：http://hz.guannengcc.top/gtoyjlxcel.html

ROLLBACK TO sp1;
来源：http://hz.xuetiantiany.cn/gtcqbtqdkm.html

[Q69] 查看执行计划
来源：http://hz.nanxuanxn.top/gtlnvfkskv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhixingplan.top/gttcpczyiq.html

[Q70] 更新统计信息
来源：http://hz.aizwys.cn/gtdevncdcl.html

ANALYZE TABLE users;
来源：http://hz.jinqigfzy.top/gthyaynbjq.html

[Q71] 查看建表语句
来源：http://hz.redwolf501.top/gtjiptryxu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aibaodan.cn/gtddxcidnx.html

[Q72] 查看索引
来源：http://hz.hammf.cn/gtvxjpfuck.html

SHOW INDEX FROM users;
来源：http://hz.smart0.xyz/gtboigfmig.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangtech.top/gtiafbkkyr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hywenlv.cn/gtwohjbrkv.html

[Q74] 强制使用索引
来源：http://hz.jinqigfzy.top/gtceovucas.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtxuyldlmy.html

[Q75] 日期格式化
来源：http://hz.tian-w.cn/gtidjrinky.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.c1oappe.top/gtvcozxpbl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gtluxjthru.html

[Q76] 按天统计
来源：http://hz.haohaochexian.top/gtnxpimvca.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangkeji.top/gtrpoycnne.html

[Q77] 时间加减
来源：http://hz.52xcode.cn/gtzavsdlhf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shuidangran.top/gtryrzgoqi.html

[Q78] 当前时间
来源：http://hz.cashguo.top/gtqwelbjgb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sweek.top/gtzblsqyai.html

[Q79] 字符串拼接
来源：http://hz.yongpay.top/gtkakmusvo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.316326.xyz/gtfpkrjebp.html

[Q80] 字符串截取
来源：http://hz.9152youxi.cn/gtelnxkxbo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.vqdsnc.cn/gtmciwnaez.html

[Q81] 字符串替换
来源：http://hz.aibaodan.cn/gtgazipbsl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gtrenrwidb.html

[Q82] 字符长度与字节长度
来源：http://hz.hfpthk.cn/gtbpzupkng.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuxming.cn/gtdynlzuyn.html

[Q83] 大小写转换
来源：http://hz.iojbl.cn/gtgfyfwdrb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenlongwang.top/gtgzslwqgh.html

[Q84] 去除首尾空格
来源：http://hz.chenzaomai.com/gtfbkuaqab.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhengqikj.top/gtjgjyirhj.html

[Q85] 数值取整
来源：http://hz.0kj1m.cn/gtdlpunidv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shangyingyoupin.top/gtldzggxmh.html

[Q86] 读取 JSON 字段
来源：http://hz.0kj1m.cn/gtzivdqxtd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuetiantiany.cn/gtxjrwyyjb.html

[Q87] JSON 字段做条件
来源：http://hz.yuxming.cn/gtivvpkruj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pengpengdd.cyou/gtlopkbfxe.html

[Q88] 行转列（条件聚合）
来源：http://hz.sweek.top/gtwxeqqbyk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tianlin.xyz/gtiftgahxx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sxryk.cn/gtqiwdxioe.html

[Q89] 判断表是否存在
来源：http://hz.guowangkeji.top/gtnkmtnyto.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnqzz.top/gtikkfyail.html

[Q90] 生成序号列
来源：http://hz.zhaomingkeji.xyz/gtnkmglkdj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtjlufgagd.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtueuexfsc.html

R. Bash 专题
来源：http://hz.xingfuxueyuan.xyz/gtegyrxlko.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmxgccfyn.html

[R01] shebang 与严格模式
来源：http://hz.snrcjt.cn/gtdcawmxqf.html

#!/usr/bin/env bash
来源：http://hz.aibaodan.cn/gtgpqmqvpa.html

set -euo pipefail
来源：http://hz.tian-w.cn/gtjxpruxao.html

[R02] 变量赋值与使用
来源：http://hz.zhiwuduotai.top/gtpbrcddox.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gttqmpvmqj.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtbgikvupi.html

readonly PI=3.14
来源：http://hz.cdnleiting.top/gtqfwsmqns.html

[R04] 位置参数
来源：http://hz.xuetiantiany.cn/gtiklastkq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258.top/gtbjzvykni.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gthgobmfvf.html

name="${1:-default}"
来源：http://hz.dianchejie.cn/gtzrxcgggj.html

[R06] 判断命令是否存在
来源：http://hz.vqdsnc.cn/gtiowrxnli.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtznxtzegs.html

[R07] if 判断文件
来源：http://hz.daria6918.cn/gtvmrtjutv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.c1oappe.top/gtqmfohqkb.html

[R08] 数值比较
来源：http://hz.dashuyun.cn/gttocqjjfp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxuanxn.top/gtueymuqnp.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gturbnfvzb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258888.top/gtqujaifgu.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gtonpqhjsd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigfzy.top/gtqligyiyh.html

[R11] case 多分支
来源：http://hz.jqgfzy.top/gtfsmfvglo.html

case "$1" in
来源：http://hz.daxiang520.top/gtssqauknc.html

start) echo "启动" ;;
来源：http://hz.feifeiyinyue.top/gtpipqhxzj.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtydsgknqf.html

*)     echo "未知命令" ;;
来源：http://hz.cucudq.cn/gtlswxgtkf.html

esac
来源：http://hz.redwolf501.top/gtuurbcpnn.html

[R12] for 遍历文件
来源：http://hz.jlsjyb.cn/gtberbfdew.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dashuyun.cn/gtokvgvbnq.html

[R13] for 计数循环
来源：http://hz.smart0.xyz/gtvwttogrw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtqfeaduzu.html

[R14] C 风格 for
来源：http://hz.nanxinkj.top/gtdvtrveqa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtfydjbrzh.html

[R15] while 逐行读文件
来源：http://hz.hongshengwenyu.top/gtyoobxkak.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shzxlz.cn/gtdbsxmwin.html

[R16] until 等待条件
来源：http://hz.chenlongwang.top/gthzhtpasz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.birdmap.top/gtpwnqxvyz.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gtzmhtpdci.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aizwys.cn/gtmwbxyaaw.html

[R18] 遍历数组
来源：http://hz.andypj.xyz/gtdymzvycp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.birdmap.top/gtlnasjikh.html

[R19] 数组长度
来源：http://hz.cheryme.top/gtpkxjhxak.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtmjefpkeh.html

[R20] 关联数组（字典）
来源：http://hz.ydzc1.top/gtusisrrsj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtjxtveeps.html

[R21] 字符串长度
来源：http://hz.hywenlv.cn/gtszhixoga.html

echo "${#s}"
来源：http://hz.iojbl.cn/gtbcaybvco.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gtfdojrpdu.html

echo "${s:0:5}"
来源：http://hz.zhijiandao.cn/gteutnsoos.html

[R23] 字符串替换
来源：http://hz.zhongyouzk.top/gtjtwscaui.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yangfankeji.com/gttujwacak.html

[R24] 大小写转换
来源：http://hz.aibaodan.cn/gtgnbntwcb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dianchejie.cn/gtijozplkz.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuxming.cn/gtamakgail.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shanyushiyangkeji.top/gtyoeneuog.html

[R26] 命令替换
来源：http://hz.chenlongwang.top/gtneeooygp.html

now=$(date +%F); echo "$now"
来源：http://hz.xuetiantiany.cn/gtjkxlsids.html

[R27] 算术展开
来源：http://hz.jqgfzy.top/gtmmzdddsd.html

echo $((1 + 2 * 3))
来源：http://hz.hnxiangtu.top/gtexihohfa.html

[R28] 浮点运算
来源：http://hz.nanxinkj.top/gtkjjgmlcn.html

echo "scale=2; 10/3" | bc
来源：http://hz.ybcxt.top/gtsicuqjut.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtlsdzrenn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yongpay.top/gtyvjlmlkw.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtroachptm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtuljovohg.html

[R31] 局部变量
来源：http://hz.xuetiantiany.cn/gtzerdvxdc.html

f() { local x=1; echo "$x"; }
来源：http://hz.pengpengdd.cyou/gtkmquytmd.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtqqqtvbqw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yvedp.cn/gttxzsliah.html

[R33] 捕获错误并提示行号
来源：http://hz.0kj1m.cn/gtmflfnzte.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtnqhljpit.html

[R34] 退出时清理
来源：http://hz.gotoacloud.top/gtrduqsggk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuanzhike.top/gtrcxmbjuy.html

[R35] 后台执行并等待
来源：http://hz.havefunace.top/gtbfladeiq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuxming.cn/gtsezdfbyq.html

[R36] 并发执行多个任务
来源：http://hz.ydzc1.top/gtdhgnizbg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ywan-chungtsiang.top/gtjxilcveu.html

[R37] 把输出赋给变量
来源：http://hz.jlsjyb.cn/gtkuskinpo.html

files=$(ls -1)
来源：http://hz.yonumen.top/gtnsejavza.html

[R38] 管道串联
来源：http://hz.zhoulong.xyz/gtuxtwajjl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yvedp.cn/gtrzzqqsbz.html

[R39] 重定向标准输出与错误
来源：http://hz.kuanghao11.cn/gtrdzxgjnw.html

cmd > out.log 2>&1
来源：http://hz.gzhubu.top/gtcpoiwsru.html

[R40] 追加写日志
来源：http://hz.chenlongwang.top/gtbmotwiyh.html

echo "log" >> out.log
来源：http://hz.andypj.xyz/gtuqehaltq.html

[R41] 丢弃输出
来源：http://hz.hysaishi.cn/gtbgcclkdu.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtkvlghqij.html

[R42] 输入重定向
来源：http://hz.ydjk.org.cn/gtthtfwujn.html

wc -l < a.txt
来源：http://hz.jiagoushi.top/gtivajrejw.html

[R43] 按名字查找文件
来源：http://hz.mhx1999.top/gtsythkteb.html

find . -name "*.log" -type f
来源：http://hz.cucudq.cn/gthfrblroy.html

[R44] 按修改时间查找
来源：http://hz.zhixingplan.top/gtqetftbis.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtxajyagep.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtxsznbdbm.html

find . -name "*.tmp" -delete
来源：http://hz.yueranfly.top/gtepgsqxwb.html

[R46] 递归替换文件内容
来源：http://hz.daxiang520.top/gtbmidmzci.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xziqi.cn/gtjagjmxfv.html

[R47] sed 单行替换
来源：http://hz.hongshengwenyu.top/gtukgusmex.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.316326.xyz/gthdrujiyr.html

[R48] awk 取指定列
来源：http://hz.pycfn.com/gtkqgounkr.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxuanxn.top/gtnreydtql.html

[R49] awk 带条件
来源：http://hz.cheryme.top/gtyvjntnoq.html


<!-- 参考信息 -->