代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtmffzmmhu.html

user_id INT NOT NULL,
来源：http://hz.yongpay.top/gtwhbwpdis.html

amount DECIMAL(10, 2),
来源：http://hz.jiagoushi.top/gtjjuxhewd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtekuocatx.html

);
来源：http://hz.tanke756.top/gtmljtoynz.html

[Q03] 增加列
来源：http://hz.zhongyouzk.top/gtdrhoreei.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.birdmap.top/gtauowdkcy.html

[Q04] 修改列类型
来源：http://hz.shuidangran.top/gtgiutvfbk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cheryme.top/gtdnofynbm.html

[Q05] 重命名列
来源：http://hz.shanyushiyangtech.top/gtjrgreiye.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.kuanghao11.cn/gtttyzpcgx.html

[Q06] 删除列
来源：http://hz.snrcjt.cn/gtaevqqqez.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jiagoushi.top/gtmauanxpp.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtqwctigwy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.bjfxy.top/gttpnmwhjj.html

[Q08] 创建普通索引
来源：http://hz.kuanghao11.cn/gtarhkwuzt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sxryk.cn/gtvajdnmfd.html

[Q09] 创建唯一索引
来源：http://hz.jinyuanbaomall.cn/gtpzplxlyn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtmvwzaroo.html

[Q10] 插入单行
来源：http://hz.aizwys.cn/gtzfpwqmbh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fengsongda.top/gtodnkqjuh.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtlghgbmrj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.316326.xyz/gtnibkkate.html

[Q12] 插入后取自增 ID
来源：http://hz.shangyingyoupin.top/gtbbteptqs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.snrcjt.cn/gtnprkdzcj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtulwhhxih.html

[Q13] 忽略重复插入
来源：http://hz.shangyingyoupin.top/gtztizbwfg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gtvcbuvvid.html

[Q14] 存在则更新（upsert）
来源：http://hz.snrcjt.cn/gtueclkaio.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhaomingkeji.xyz/gtqtgwsdas.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinghuilouyu.cn/gtmwvcgmis.html

[Q15] 查询全部
来源：http://hz.cqqwz.cn/gtyezgdilb.html

SELECT * FROM users;
来源：http://hz.ivvv.top/gtterflfjb.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtmpijjrks.html

SELECT id, name FROM users;
来源：http://hz.zhengqikj.top/gtfpjrdtxe.html

[Q17] 条件查询
来源：http://hz.svipenyu.cn/gtcvhqhumv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.fengsongda.top/gtdzeyjxot.html

[Q18] 模糊匹配
来源：http://hz.gogol.net.cn/gtntwstlvq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hfpthk.cn/gtcnzultbh.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gtpjyqdkmy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sxryk.cn/gtbbovypgn.html

[Q20] IN 列表
来源：http://hz.tanke756.top/gtqtatqews.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhaomingkeji.xyz/gtgyouzbnr.html

[Q21] 空值判断
来源：http://hz.nwbrower.top/gtaehvbgds.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.havefunace.top/gtdtfxjkyu.html

[Q22] 排序
来源：http://hz.smart0.xyz/gtsqxlbvvv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xinyue.icu/gtnytljjcc.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtfhmyhhys.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtzfmknisy.html

[Q24] 去重
来源：http://hz.daxiang520.top/gthssrehwt.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhengqikj.top/gtkfnwomly.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gttqminffu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.316326.xyz/gtadxtkcim.html

[Q26] 计数
来源：http://hz.ybcxt.top/gtuvvupdua.html

SELECT COUNT(*) FROM users;
来源：http://hz.fzhhl.top/gteuzebmit.html

[Q27] 条件计数
来源：http://hz.mhx1999.top/gtqbrmueei.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.smart0.xyz/gthibjilca.html

[Q28] 求和与平均
来源：http://hz.zhengqikj.top/gtswtgizqo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtwjogpyoo.html

[Q29] 最大最小值
来源：http://hz.jqgufenzy.top/gtnxitotzu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.bjfxy.top/gtjzbxzkbq.html

[Q30] 分组统计
来源：http://hz.sysykeji.top/gthewieoti.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtgonqhdsd.html

[Q31] 分组后过滤
来源：http://hz.redwolf501.top/gtvnnqvnve.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jiagoushi.top/gteoxgsjsp.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtmlzvlbap.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gteviqhodb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigfzy.top/gtfvjujztn.html

[Q33] 多列分组
来源：http://hz.yongpay.top/gtovoskunz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangtech.top/gtvexxsjvk.html

[Q34] 每组取第一条
来源：http://hz.jianghu66.top/gtncfpvwfq.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gtlesiisqo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.haohaochexian.top/gthpslowvm.html

) t WHERE rn = 1;
来源：http://hz.nanxuanxn.top/gtuagqbvov.html

[Q35] 内连接
来源：http://hz.gaohongyu789.top/gtyubqlaxc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtxgvrhghb.html

[Q36] 左连接
来源：http://hz.jinqigufen.top/gtqeoqdvfa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtisbyvbqz.html

[Q37] 右连接
来源：http://hz.tanke756.top/gturmwwwqy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.vqdsnc.cn/gtufzfxrbf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yvedp.cn/gtorcmqtaw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhengqikj.top/gtnhoovojw.html

[Q39] 自连接（查上下级）
来源：http://hz.9152youxi.cn/gtzczuuanm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dianchejie.cn/gtawndvbkk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yongpay.top/gtshxjnhga.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shangyingyoupin.top/gtxpijkfns.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hysaishi.cn/gtamxuwkrd.html

[Q41] 多表连接
来源：http://hz.chenjidiqi.icu/gtynizsagb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuetiantiany.cn/gtxsfpvhzd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sweek.top/gtzdzyhvkt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pycfn.com/gtxvgrbtgw.html

[Q42] 连接条件附加过滤
来源：http://hz.feifeiyinyue.top/gtodabwrux.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hammf.cn/gtwmkodhre.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxuanxn.top/gteqarpbcm.html

[Q43] 标量子查询
来源：http://hz.haohaochexian.top/gtcyrbsgar.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shuidangran.top/gtyppuczyc.html

[Q44] IN 子查询
来源：http://hz.c1oappe.top/gtyaavxnum.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jlsjyb.cn/gtfzroqemu.html

[Q45] EXISTS 判断存在
来源：http://hz.hfpthk.cn/gtbxvxmfrf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtuxxzuyli.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhijiandao.cn/gtzyjxvrbv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtchscdvoz.html

[Q47] 与平均值比较
来源：http://hz.cashguo.top/gtvjfacvgk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtdlmbayst.html

[Q48] CTE 公用表表达式
来源：http://hz.hammf.cn/gtwhcnferl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuxming.cn/gtprtdzhbd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtagunnkwn.html

[Q49] 更新单行
来源：http://hz.cucudq.cn/gtvcatmzej.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xinyue.icu/gtyviehfhn.html

[Q50] 批量更新
来源：http://hz.yongpay.top/gtiuaeqllx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.haohaochexian.top/gtibbfswfd.html

[Q51] 用子查询更新
来源：http://hz.ywan-chungtsiang.top/gtwblevkld.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dianchejie.cn/gtwmyaciro.html

[Q52] 删除指定行
来源：http://hz.shuidangran.top/gtjwwpqley.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gaohongyu789.top/gtkrzuvlvj.html

[Q53] 按条件删除
来源：http://hz.nanxinkj.top/gtzmkjilhc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigfzy.top/gtawdhdese.html

[Q54] 清空表
来源：http://hz.yongpay.top/gtgdansdek.html

TRUNCATE TABLE logs;
来源：http://hz.dianchejie.cn/gtkstopoyf.html

[Q55] 排名（并列占位）
来源：http://hz.guowangkeji.top/gttzgijwvk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jyoumei.cn/gtbtqmdydo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangtech.top/gtraukyxgf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtnnjzpxcn.html

[Q57] 行号
来源：http://hz.jiagoushi.top/gtihkyzecp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxuanxn.top/gtuezkfdpn.html

[Q58] 累计求和
来源：http://hz.fzhhl.top/gtpbvmpwyb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigfzy.top/gtcflqvhqs.html

[Q59] 分组内累计
来源：http://hz.xylfe.cn/gtogxamdyf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gotoacloud.top/gtuowrbrir.html

[Q60] 取上一行 / 下一行
来源：http://hz.hysaishi.cn/gtlfdtvlzo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtlshnlotf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangdashe.top/gtjyqdikzh.html

[Q61] 移动平均
来源：http://hz.ydjk.org.cn/gtmmhmekim.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yuxming.cn/gtptszzfnt.html

[Q62] 分组占比
来源：http://hz.jinyuanbaomall.cn/gtrpbefyjr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtmoimxgsr.html

[Q63] 开启事务
来源：http://hz.jyoumei.cn/gtsvmwqpgj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenlongwang.top/gtehyjnpum.html

[Q64] 提交事务
来源：http://hz.jlsjyb.cn/gttstnithk.html

COMMIT;
来源：http://hz.cucudq.cn/gtujgswtxd.html

[Q65] 回滚事务
来源：http://hz.tanke756.top/gtjkrogaze.html

ROLLBACK;
来源：http://hz.jinqigfzy.top/gtwyzxqfhr.html

[Q66] 行锁查询
来源：http://hz.shangyingyoupin.top/gtucndngzc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yanxiufei.cn/gtejszitwf.html

[Q67] 设置隔离级别
来源：http://hz.jinqigfzy.top/gtolzrgsaw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtefwjzyax.html

[Q68] 保存点
来源：http://hz.hammf.cn/gtnzejmvzw.html

SAVEPOINT sp1;
来源：http://hz.hnxiangtu.top/gtxgywgkmq.html

ROLLBACK TO sp1;
来源：http://hz.pengpengdd.cyou/gtywgpnbpg.html

[Q69] 查看执行计划
来源：http://hz.dashuyun.cn/gtafuulcsp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nanxinkj.top/gtnjrgkpvm.html

[Q70] 更新统计信息
来源：http://hz.iojbl.cn/gtvfjreerb.html

ANALYZE TABLE users;
来源：http://hz.sweek.top/gtnhvgnsxr.html

[Q71] 查看建表语句
来源：http://hz.shuidangran.top/gtmsgizskc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xingfuxueyuan.xyz/gtpqbpgzer.html

[Q72] 查看索引
来源：http://hz.hnqzz.top/gtsdpwnhmi.html

SHOW INDEX FROM users;
来源：http://hz.jiagoushi.top/gtrhukidxp.html

[Q73] 查看表状态
来源：http://hz.316326.xyz/gtakxgvetp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhijiandao.cn/gtrznoemvy.html

[Q74] 强制使用索引
来源：http://hz.jyoumei.cn/gtzjzjqqxd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shuidangran.top/gtelvvyvbe.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtaiuvxxfr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yueranfly.top/gtstxgtulr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuxming.cn/gtvejdpera.html

[Q76] 按天统计
来源：http://hz.bjfxy.top/gtukasjtam.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.0kj1m.cn/gtygddhqvm.html

[Q77] 时间加减
来源：http://hz.jinqigfzy.top/gtzttihgeg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yangfankeji.com/gthgnubnzp.html

[Q78] 当前时间
来源：http://hz.shuidangran.top/gtfyujbgtl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fzhhl.top/gtonsqjaub.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtojahwimz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jyoumei.cn/gtjzwggupj.html

[Q80] 字符串截取
来源：http://hz.zhaomingkeji.xyz/gthsoslmlr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhixingplan.top/gtldoitruf.html

[Q81] 字符串替换
来源：http://hz.xinyue.icu/gtbhzqyvbq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gtpwspimvr.html

[Q82] 字符长度与字节长度
来源：http://hz.sweek.top/gtwoteetqh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tianlin.xyz/gttsmjeaod.html

[Q83] 大小写转换
来源：http://hz.zycfv.cn/gtkmbepxdz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.9152youxi.cn/gttfzwrmqc.html

[Q84] 去除首尾空格
来源：http://hz.fzhhl.top/gteskbaymn.html

SELECT TRIM(name) FROM users;
来源：http://hz.xziqi.cn/gthysyfhwb.html

[Q85] 数值取整
来源：http://hz.hywenlv.cn/gtvsqitmnc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shuidangran.top/gtuwyiodmi.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtvrftlcqx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.mhx1999.top/gtesmotcom.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gtrnjtkroa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tianlin.xyz/gtbjkgimmu.html

[Q88] 行转列（条件聚合）
来源：http://hz.yanxiufei.cn/gtvstwcthu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigfzy.top/gtozeugtnv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shuidangran.top/gtknhweiqj.html

[Q89] 判断表是否存在
来源：http://hz.ybcxt.top/gtdjcmtagy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.52xcode.cn/gtoyqrgjbq.html

[Q90] 生成序号列
来源：http://hz.wangshuangyany.cn/gtmjkjaqtp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cqqwz.cn/gtmsqgivne.html

================================================================================
来源：http://hz.c1oappe.top/gtrcewwxdt.html

R. Bash 专题
来源：http://hz.cheryme.top/gthjmqgotj.html

================================================================================
来源：http://hz.zhiwuduotai.top/gthhyapgnu.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtvtwikien.html

#!/usr/bin/env bash
来源：http://hz.havefunace.top/gtprzpvdfs.html

set -euo pipefail
来源：http://hz.ydzc1.top/gthmqesmnt.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtgcukvvml.html

name="Tom"; echo "$name"
来源：http://hz.chenlongwang.top/gtvqqoendl.html

[R03] 只读变量
来源：http://hz.jinqigfzy.top/gtepzaisyq.html

readonly PI=3.14
来源：http://hz.zhoulong.xyz/gtlgzistko.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtsowoyeri.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guannengcc.top/gtukuucash.html

[R05] 参数默认值
来源：http://hz.mhx1999.top/gtehvhusqf.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtkzatkxou.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtbswpcqtd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fzhhl.top/gttqwfjznj.html

[R07] if 判断文件
来源：http://hz.xingfuxueyuan.xyz/gtciysclkj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hongshengwenyu.top/gtjegzvtqx.html

[R08] 数值比较
来源：http://hz.shuidangran.top/gtcmnafmmb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gtsqilgzur.html

[R09] 字符串比较
来源：http://hz.jinghuilouyu.cn/gtofnidkfe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gogol.net.cn/gtuomahpjb.html

[R10] 正则匹配
来源：http://hz.jyoumei.cn/gtoxifoofo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxuanxn.top/gtppxhsxuw.html

[R11] case 多分支
来源：http://hz.hysaishi.cn/gtbomzjjnc.html

case "$1" in
来源：http://hz.52xcode.cn/gtcikpewsz.html

start) echo "启动" ;;
来源：http://hz.dianchejie.cn/gtawapclts.html

stop)  echo "停止" ;;
来源：http://hz.smart0.xyz/gtweypxlkw.html

*)     echo "未知命令" ;;
来源：http://hz.cucudq.cn/gtqytqibnn.html

esac
来源：http://hz.zhengqikj.top/gtrtrrchze.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gtcsjgjqbh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtoipajztm.html

[R13] for 计数循环
来源：http://hz.nanxinkj.top/gtujbgpxiy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.316326.xyz/gtbjqbnkug.html

[R14] C 风格 for
来源：http://hz.yongpay.top/gttsfpdiiy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtikrganoe.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gtvamhyipt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dashuyun.cn/gtyzgszmry.html

[R16] until 等待条件
来源：http://hz.tian-w.cn/gtwpyyxtls.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtnxzdmqjk.html

[R17] 数组定义与取值
来源：http://hz.hongshengwenyu.top/gtglmjlcbr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtrlueahvr.html

[R18] 遍历数组
来源：http://hz.jyoumei.cn/gtbdevjkvn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtkxbvkrki.html

[R19] 数组长度
来源：http://hz.dianchejie.cn/gtmzvfrgtl.html

echo "${#arr[@]}"
来源：http://hz.tianlin.xyz/gttyfznfzw.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtftfaabzd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dianchejie.cn/gtddxitvlp.html

[R21] 字符串长度
来源：http://hz.pycfn.com/gtvglmtwsn.html

echo "${#s}"
来源：http://hz.ppjwa.cn/gtqoolilnq.html

[R22] 截取子串
来源：http://hz.chenlongwang.top/gtoczzqavv.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gtioarfkjt.html

[R23] 字符串替换
来源：http://hz.316326.xyz/gtutmzqdxe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gzhubu.top/gtzrlbeaze.html

[R24] 大小写转换
来源：http://hz.xinyue.icu/gtmamkdoqp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ywan-chungtsiang.top/gtqcmjxzmg.html

[R25] 去后缀 / 去前缀
来源：http://hz.sufxvd.cn/gtnxxkxqhl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jiagoushi.top/gtrjcrulcs.html

[R26] 命令替换
来源：http://hz.hnqzz.top/gtvzfjeyqq.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigfzy.top/gtqokaxtnd.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtwskmrjjy.html

echo $((1 + 2 * 3))
来源：http://hz.zhiwuduotai.top/gtmbwdlsph.html

[R28] 浮点运算
来源：http://hz.feifeiyinyue.top/gtigzbmgkt.html

echo "scale=2; 10/3" | bc
来源：http://hz.cashguo.top/gtmjthykfz.html

[R29] 定义函数
来源：http://hz.xylfe.cn/gttfwlzwgl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xinyue.icu/gtajljuuiu.html

[R30] 函数返回状态码
来源：http://hz.ehwqpu.com/gtqescngji.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangdashe.top/gticwwqkco.html

[R31] 局部变量
来源：http://hz.jinyuanbaomall.cn/gtfdyzbvid.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gtximrrqak.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gtaedcfqox.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cheryme.top/gtznxyldec.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangtech.top/gtbrenbhnl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yuanzhike.top/gthifcftyg.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtwisafaux.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gtcvseleiz.html

[R35] 后台执行并等待
来源：http://hz.havefunace.top/gtfpzolstv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ppjwa.cn/gtovmeoalf.html

[R36] 并发执行多个任务
来源：http://hz.yongpay.top/gtvgcpdhbz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cdnleiting.top/gttsfcjvbo.html

[R37] 把输出赋给变量
来源：http://hz.xinyue.icu/gtnnrdltsr.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtmrmjqbmu.html

[R38] 管道串联
来源：http://hz.xuetiantiany.cn/gtomtwzuiz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnxiangtu.top/gtfafqxpkp.html

[R39] 重定向标准输出与错误
来源：http://hz.0kj1m.cn/gtdhcxfdek.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangkeji.top/gtpcryvgjn.html

[R40] 追加写日志
来源：http://hz.bjfxy.top/gtxugaadqq.html

echo "log" >> out.log
来源：http://hz.jqgufenzy.top/gtvagtktft.html

[R41] 丢弃输出
来源：http://hz.vqdsnc.cn/gtqaukfyuc.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtylodevvf.html

[R42] 输入重定向
来源：http://hz.zycfv.cn/gtjkqzyqzv.html

wc -l < a.txt
来源：http://hz.cucudq.cn/gtycumgiyz.html

[R43] 按名字查找文件
来源：http://hz.zhijiandao.cn/gtsobgqrie.html

find . -name "*.log" -type f
来源：http://hz.zhongyouzk.top/gtwppwfyrf.html

[R44] 按修改时间查找
来源：http://hz.xuanzx.com/gtxygxzfvi.html

find . -mtime -7 -type f
来源：http://hz.hnxiangtu.top/gtswdytdrk.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gtcfzelakl.html

find . -name "*.tmp" -delete
来源：http://hz.316326.xyz/gtkoafgoby.html

[R46] 递归替换文件内容
来源：http://hz.birdmap.top/gtcsfaahpt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cdnleiting.top/gtbzfehkuc.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtbuwosiwj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenjidiqi.icu/gtrxxcyqev.html

[R48] awk 取指定列
来源：http://hz.chenzaomai.com/gtvfztsdol.html

awk '{print $1, $3}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtadvykpwk.html

[R49] awk 带条件
来源：http://hz.cashguo.top/gtvwdmdffs.html


<!-- 参考信息 -->