代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtdbxaqyzg.html

user_id INT NOT NULL,
来源：http://hz.jqgufenzy.top/gtdaheliws.html

amount DECIMAL(10, 2),
来源：http://hz.cashguo.top/gtcibfzhzf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sweek.top/gtkreqhipl.html

);
来源：http://hz.cashguo.top/gtxacmzknh.html

[Q03] 增加列
来源：http://hz.sysykeji.top/gtdnaoxjtn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daxiang520.top/gtpdibrpsy.html

[Q04] 修改列类型
来源：http://hz.zhaomingkeji.xyz/gtzfxkkqqs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tanke756.top/gtnobqyuoy.html

[Q05] 重命名列
来源：http://hz.jinghuilouyu.cn/gtduzmlkmy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shuidangran.top/gtwdpxqkwk.html

[Q06] 删除列
来源：http://hz.cucudq.cn/gtzxiblaaf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.smart0.xyz/gtyydmxyzu.html

[Q07] 删除表
来源：http://hz.xingfuxueyuan.xyz/gtlkytkzsv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangtech.top/gtgijpwxdy.html

[Q08] 创建普通索引
来源：http://hz.shanyushiyangkeji.top/gtbennipcg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yonumen.top/gtodsosijq.html

[Q09] 创建唯一索引
来源：http://hz.ivvv.top/gtnnwpskpg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tanke756.top/gthabspeto.html

[Q10] 插入单行
来源：http://hz.9152youxi.cn/gtsobbnswy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sysykeji.top/gtltrpwokk.html

[Q11] 一次插入多行
来源：http://hz.sysykeji.top/gtigwyqgcq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258888.top/gtigejdnxu.html

[Q12] 插入后取自增 ID
来源：http://hz.ywan-chungtsiang.top/gtqgibqnhx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hongshengwenyu.top/gtanujmkkf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuanzx.com/gtxomawqck.html

[Q13] 忽略重复插入
来源：http://hz.guowangkeji.top/gthqsebzxc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhaomingkeji.xyz/gtwsebhsyt.html

[Q14] 存在则更新（upsert）
来源：http://hz.birdmap.top/gtvmsxmpki.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gteoccvogn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.0kj1m.cn/gtmjwsejbl.html

[Q15] 查询全部
来源：http://hz.zhijiandao.cn/gtameuiqgz.html

SELECT * FROM users;
来源：http://hz.cqqwz.cn/gtlszkosjp.html

[Q16] 查询指定列
来源：http://hz.aizwys.cn/gtaecybjhs.html

SELECT id, name FROM users;
来源：http://hz.hnqzz.top/gtpzsifrom.html

[Q17] 条件查询
来源：http://hz.hfpthk.cn/gtytuvzpnt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuxming.cn/gtcawpmeyu.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gtlrxlyiux.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fengsongda.top/gtrwjrsgjx.html

[Q19] 范围查询
来源：http://hz.yj202588.top/gtnapvwzzv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnxiangtu.top/gtuuqxkhbc.html

[Q20] IN 列表
来源：http://hz.cheryme.top/gtjcskxkrj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xylfe.cn/gtobjvotvd.html

[Q21] 空值判断
来源：http://hz.hammf.cn/gtbtltqiht.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tian-w.cn/gtnbsvgbkw.html

[Q22] 排序
来源：http://hz.zdqjudy.top/gtrdfltaor.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.daxiang520.top/gttwahsixb.html

[Q23] 分页
来源：http://hz.zhaomingkeji.xyz/gtitpgvelp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cheryme.top/gtajdelyqm.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gtoeiriqia.html

SELECT DISTINCT city FROM users;
来源：http://hz.havefunace.top/gtoalwvlkj.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtxzxbwnfc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.guannengcc.top/gtlxsabenn.html

[Q26] 计数
来源：http://hz.cheryme.top/gtwecxlusf.html

SELECT COUNT(*) FROM users;
来源：http://hz.zdqjudy.top/gtjahslfvf.html

[Q27] 条件计数
来源：http://hz.shanyushiyangkeji.top/gtsoglpezm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pycfn.com/gtjfsbeufx.html

[Q28] 求和与平均
来源：http://hz.xziqi.cn/gtrfbcrocf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jqgufenzy.top/gtamkodxgz.html

[Q29] 最大最小值
来源：http://hz.iojbl.cn/gtvnhiawqw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.kuanghao11.cn/gtegmhfnxk.html

[Q30] 分组统计
来源：http://hz.yvedp.cn/gtewbhgeuz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtlihnjqvp.html

[Q31] 分组后过滤
来源：http://hz.haohaochexian.top/gtdbptwffu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.aizwys.cn/gtodtioabg.html

[Q32] 分组拼接字符串
来源：http://hz.dianchejie.cn/gtxtbsmvyg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtrfccykgp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cucudq.cn/gtrlqpxisz.html

[Q33] 多列分组
来源：http://hz.316326.xyz/gthrlbzuye.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daxiang520.top/gtxihuzfsx.html

[Q34] 每组取第一条
来源：http://hz.gzhubu.top/gtsyszwcnk.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gteovdwywc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zycfv.cn/gtftrqkzga.html

) t WHERE rn = 1;
来源：http://hz.pycfn.com/gtyzurcdin.html

[Q35] 内连接
来源：http://hz.xinyue.icu/gtkyvdhpff.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gttcjxvisf.html

[Q36] 左连接
来源：http://hz.sxryk.cn/gtsndtlola.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtdhwovbps.html

[Q37] 右连接
来源：http://hz.jinqigfzy.top/gttybxayto.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yangfankeji.com/gtaoijasvh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yongpay.top/gtbbxbtfjt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zycfv.cn/gtbianeihv.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtkowdybqr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.haohaochexian.top/gtdqqhbtea.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gtuvidtipw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gogol.net.cn/gttkofkkqn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zycfv.cn/gtdmtvcnzl.html

[Q41] 多表连接
来源：http://hz.tianlin.xyz/gtzqwshhfl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.feifeiyinyue.top/gtzeziqiri.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtdtwwmein.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenlongwang.top/gtodyplrmr.html

[Q42] 连接条件附加过滤
来源：http://hz.pengpengdd.cyou/gthdtapdfq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sxryk.cn/gtqumvaeyh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhijiandao.cn/gtpkkizzip.html

[Q43] 标量子查询
来源：http://hz.bjfxy.top/gtfzruvlte.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuetiantiany.cn/gtevqxrkxq.html

[Q44] IN 子查询
来源：http://hz.0kj1m.cn/gtjpusfsgg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cucudq.cn/gtwfigwcnd.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258888.top/gteukaimuo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtlyulxvon.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jiagoushi.top/gtrqpvitmg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daxiang520.top/gtbmclwhoc.html

[Q47] 与平均值比较
来源：http://hz.zhiwuduotai.top/gtpfqzdwxb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.fzhhl.top/gtjgeyysiv.html

[Q48] CTE 公用表表达式
来源：http://hz.52xcode.cn/gtjmqxtjto.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sxryk.cn/gtzqyvrihn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangtech.top/gtyflpblcm.html

[Q49] 更新单行
来源：http://hz.hysaishi.cn/gttrwqbeew.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.0kj1m.cn/gttikeaiaf.html

[Q50] 批量更新
来源：http://hz.hammf.cn/gtbhujhdog.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yvedp.cn/gthajmcsfk.html

[Q51] 用子查询更新
来源：http://hz.guannengcc.top/gthxhnodpu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj202588.top/gtozheptwo.html

[Q52] 删除指定行
来源：http://hz.yanxiufei.cn/gtvydokdyv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cashguo.top/gtvzjknvym.html

[Q53] 按条件删除
来源：http://hz.yj20258.top/gtfjkkglxt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigufen.top/gtzhyjzonr.html

[Q54] 清空表
来源：http://hz.cucudq.cn/gtrwmgznis.html

TRUNCATE TABLE logs;
来源：http://hz.gzhubu.top/gtjxbngmjk.html

[Q55] 排名（并列占位）
来源：http://hz.aizwys.cn/gtebfxyall.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.daria6918.cn/gtpretwhqy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cheryme.top/gtznefanzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinyuanbaomall.cn/gtsdbtcfyp.html

[Q57] 行号
来源：http://hz.shuidangran.top/gtamkcimfm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gotoacloud.top/gtgxuptfog.html

[Q58] 累计求和
来源：http://hz.zycfv.cn/gtpvczjzhp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fengsongda.top/gtndrxyndm.html

[Q59] 分组内累计
来源：http://hz.316326.xyz/gtzwvfuziu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gtduycgphd.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gtlknwnjku.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yanxiufei.cn/gtwhohozax.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tian-w.cn/gtbuuzhqwt.html

[Q61] 移动平均
来源：http://hz.andypj.xyz/gtcpwxutqt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinqigfzy.top/gtwtztxskf.html

[Q62] 分组占比
来源：http://hz.yonumen.top/gtlztqhloi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtayhqnmjm.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gttjhexjxy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gtbkjteovt.html

[Q64] 提交事务
来源：http://hz.wangshuangyany.cn/gtmvdvukjx.html

COMMIT;
来源：http://hz.zhiwuduotai.top/gtsgziloda.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtfmxwduop.html

ROLLBACK;
来源：http://hz.jinqigufen.top/gtijjxudbw.html

[Q66] 行锁查询
来源：http://hz.zdqjudy.top/gtfjoqordl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgfzy.top/gtfwrqdndc.html

[Q67] 设置隔离级别
来源：http://hz.yvedp.cn/gtgnztggdf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtpvclsyst.html

[Q68] 保存点
来源：http://hz.xingfuxueyuan.xyz/gthvmtygwa.html

SAVEPOINT sp1;
来源：http://hz.zhijiandao.cn/gtoiqgyhan.html

ROLLBACK TO sp1;
来源：http://hz.aibaodan.cn/gtjxctxoor.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtsvqzcbga.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ydzc1.top/gtqrqgsbjv.html

[Q70] 更新统计信息
来源：http://hz.jinqigufen.top/gtpfjmclcg.html

ANALYZE TABLE users;
来源：http://hz.jinghuilouyu.cn/gtmvthojqp.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtunonzlbr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cdnleiting.top/gtsqjvsgjm.html

[Q72] 查看索引
来源：http://hz.yuanzhike.top/gtwothsqvj.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gthypehkdh.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gthiincqqh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtkeyhtwdb.html

[Q74] 强制使用索引
来源：http://hz.zdqjudy.top/gtwbnflufd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258888.top/gtucxhrmpg.html

[Q75] 日期格式化
来源：http://hz.yueranfly.top/gtnzqpklcu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gaohongyu789.top/gtmbfffofu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhaomingkeji.xyz/gtopvsohpd.html

[Q76] 按天统计
来源：http://hz.tianlin.xyz/gtkpxmkrrj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cdnleiting.top/gtijtgbwla.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gthsmkhdqs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shanyushiyangtech.top/gthelompop.html

[Q78] 当前时间
来源：http://hz.gzhubu.top/gtxxvhnzop.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gtztugtshv.html

[Q79] 字符串拼接
来源：http://hz.yj20258888.top/gtqrkojpuu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cqqwz.cn/gtqbumhcur.html

[Q80] 字符串截取
来源：http://hz.birdmap.top/gtwpbjbuhw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.9152youxi.cn/gtddovhxxk.html

[Q81] 字符串替换
来源：http://hz.pengpengdd.cyou/gtwjdrqekz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aizwys.cn/gtbyuoabsc.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gtiszvfweu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtaxmaovfq.html

[Q83] 大小写转换
来源：http://hz.hnqzz.top/gtmawnhrmd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.0kj1m.cn/gtlgjfzvri.html

[Q84] 去除首尾空格
来源：http://hz.yuxming.cn/gtkbresukz.html

SELECT TRIM(name) FROM users;
来源：http://hz.jiagoushi.top/gtkpbhieqc.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtwnuttsjx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cheryme.top/gtvrilromn.html

[Q86] 读取 JSON 字段
来源：http://hz.sysykeji.top/gtsldczman.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ydzc1.top/gtzqfnwgbw.html

[Q87] JSON 字段做条件
来源：http://hz.ydzc1.top/gtxzwoigyd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hongshengwenyu.top/gtytdkwfbk.html

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gteswhjvty.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtmqxazsxk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hfpthk.cn/gtqtfcbewi.html

[Q89] 判断表是否存在
来源：http://hz.hfpthk.cn/gtnaaowivs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinghuilouyu.cn/gtbmpkdafo.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtcgadhywn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuanzhike.top/gtypskfewt.html

================================================================================
来源：http://hz.jqgfzy.top/gtqkaicxwx.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtrcyfkjds.html

================================================================================
来源：http://hz.316326.xyz/gtrufvpeqm.html

[R01] shebang 与严格模式
来源：http://hz.yangfankeji.com/gtrprkszex.html

#!/usr/bin/env bash
来源：http://hz.ivvv.top/gtenvzbzvm.html

set -euo pipefail
来源：http://hz.hnqzz.top/gtzbrhfpzd.html

[R02] 变量赋值与使用
来源：http://hz.iojbl.cn/gtxzunmmqx.html

name="Tom"; echo "$name"
来源：http://hz.yj20258.top/gtnrzikhso.html

[R03] 只读变量
来源：http://hz.yanxiufei.cn/gtjkixnthp.html

readonly PI=3.14
来源：http://hz.sufxvd.cn/gtghaaqwys.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtbcddqjzn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.feifeiyinyue.top/gtuykafcap.html

[R05] 参数默认值
来源：http://hz.yj20258.top/gtoradumwa.html

name="${1:-default}"
来源：http://hz.xuanzx.com/gtnbzaqlxk.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtyhiecccp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.redwolf501.top/gtbulczamv.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtfkmwzpfw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cdnleiting.top/gtzledipsn.html

[R08] 数值比较
来源：http://hz.zycfv.cn/gturgygvsl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhengqikj.top/gtgovfxgeu.html

[R09] 字符串比较
来源：http://hz.pycfn.com/gtlbndzdbb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pycfn.com/gtmegtbhfv.html

[R10] 正则匹配
来源：http://hz.wangshuangyany.cn/gtroluyjlo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gtwfajqxyf.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gteybvuhiy.html

case "$1" in
来源：http://hz.jqgufenzy.top/gtidilxmki.html

start) echo "启动" ;;
来源：http://hz.sweek.top/gtpvalcshq.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gtyvmndoqa.html

*)     echo "未知命令" ;;
来源：http://hz.zhiwuduotai.top/gtskfshgae.html

esac
来源：http://hz.gogol.net.cn/gternbfsyc.html

[R12] for 遍历文件
来源：http://hz.wangdashe.top/gtzwpbzrbp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj202588.top/gtkenyoqqf.html

[R13] for 计数循环
来源：http://hz.ybcxt.top/gtiqhkgzge.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hammf.cn/gtpbrntkvb.html

[R14] C 风格 for
来源：http://hz.shzxlz.cn/gtehbrazek.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.52xcode.cn/gthltkdyjm.html

[R15] while 逐行读文件
来源：http://hz.dashuyun.cn/gtzqawpvdn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.kuanghao11.cn/gthqziaubp.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gterlizlwy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.0kj1m.cn/gtlpbzlarr.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangtech.top/gtvhtqqfmi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shangyingyoupin.top/gtcwemimvl.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gtjsxjaumt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aibaodan.cn/gtrsxeauwv.html

[R19] 数组长度
来源：http://hz.zdqjudy.top/gthvajtark.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtthdnsvny.html

[R20] 关联数组（字典）
来源：http://hz.hongshengwenyu.top/gtfywfkivc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cucudq.cn/gtknisruor.html

[R21] 字符串长度
来源：http://hz.yj20258.top/gtxnwqammb.html

echo "${#s}"
来源：http://hz.yongpay.top/gttpkrnsun.html

[R22] 截取子串
来源：http://hz.fengsongda.top/gtiizzbdtx.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtdmchcqbu.html

[R23] 字符串替换
来源：http://hz.yangfankeji.com/gtbmnyyewh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ehwqpu.com/gtgdgvxmda.html

[R24] 大小写转换
来源：http://hz.yuanzhike.top/gtiucyyerm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pycfn.com/gtntuydeff.html

[R25] 去后缀 / 去前缀
来源：http://hz.iojbl.cn/gtaqimgjwh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.daria6918.cn/gtbtxsyxyc.html

[R26] 命令替换
来源：http://hz.ybcxt.top/gtidzoxlum.html

now=$(date +%F); echo "$now"
来源：http://hz.chenjidiqi.icu/gtxcgbhxtl.html

[R27] 算术展开
来源：http://hz.chenzaomai.com/gtquzqzguv.html

echo $((1 + 2 * 3))
来源：http://hz.ivvv.top/gtlftzekom.html

[R28] 浮点运算
来源：http://hz.guannengcc.top/gtomqscakf.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenzaomai.com/gtdfsttbbe.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtptgvters.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gtghdivzft.html

[R30] 函数返回状态码
来源：http://hz.ydjk.org.cn/gtvayapwma.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgufenzy.top/gtwhnjsxnv.html

[R31] 局部变量
来源：http://hz.mhx1999.top/gtdrwppnpd.html

f() { local x=1; echo "$x"; }
来源：http://hz.tianlin.xyz/gtqwmwnasz.html

[R32] 参数个数校验
来源：http://hz.cheryme.top/gtpccltpli.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jianghu66.top/gtfhmzunhb.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gtmishgcmw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cucudq.cn/gtlloqskgw.html

[R34] 退出时清理
来源：http://hz.birdmap.top/gtmezzuuhu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtmnwbpbrk.html

[R35] 后台执行并等待
来源：http://hz.hnxiangtu.top/gthfqsyqhx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangshuangyany.cn/gtdbtliege.html

[R36] 并发执行多个任务
来源：http://hz.0kj1m.cn/gtqbcmsxvb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.svipenyu.cn/gtkfevazte.html

[R37] 把输出赋给变量
来源：http://hz.yonumen.top/gtrmonqadv.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtxpxinqwn.html

[R38] 管道串联
来源：http://hz.bjfxy.top/gtzakoglsl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.smart0.xyz/gtgoiwjusz.html

[R39] 重定向标准输出与错误
来源：http://hz.gogol.net.cn/gtrmaqtpsx.html

cmd > out.log 2>&1
来源：http://hz.chenzaomai.com/gtreixctfu.html

[R40] 追加写日志
来源：http://hz.jinqigfzy.top/gtobmxjlxq.html

echo "log" >> out.log
来源：http://hz.guannengcc.top/gtwphyayll.html

[R41] 丢弃输出
来源：http://hz.wangshuangyany.cn/gtkxusoxwt.html

cmd >/dev/null 2>&1
来源：http://hz.zhaomingkeji.xyz/gtrxyszfvc.html

[R42] 输入重定向
来源：http://hz.pengpengdd.cyou/gtoznoilmx.html

wc -l < a.txt
来源：http://hz.ydzc1.top/gtlkpwggsi.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtqbjhhrnh.html

find . -name "*.log" -type f
来源：http://hz.xylfe.cn/gtousrjflp.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gtkwuvmyuy.html

find . -mtime -7 -type f
来源：http://hz.jinqigufen.top/gttaaxggth.html

[R45] 批量删除
来源：http://hz.chenzaomai.com/gtqgmpjlge.html

find . -name "*.tmp" -delete
来源：http://hz.haohaochexian.top/gtecuxqwlr.html

[R46] 递归替换文件内容
来源：http://hz.vqdsnc.cn/gtckttviao.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhoulong.xyz/gtgdsplpmq.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gtxuqhoglm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jlsjyb.cn/gtxzccpagu.html

[R48] awk 取指定列
来源：http://hz.vqdsnc.cn/gtlgphjjed.html

awk '{print $1, $3}' a.txt
来源：http://hz.snrcjt.cn/gtoaszkflg.html

[R49] awk 带条件
来源：http://hz.gogol.net.cn/gtsezwlydd.html


<!-- 参考信息 -->