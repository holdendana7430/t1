代发 wailian999

PHP:  // 手写时间戳比较
来源：http://hz.chenzaomai.com/gtsazmvcrl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtnirlvitr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cucudq.cn/gtxelcmnle.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hfpthk.cn/gtydcwlibn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangtech.top/gtrfxqvtpb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gtdzemjnjb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtdcppyqke.html

[P08] 处理浮点精度问题
来源：http://hz.yj202588.top/gtbjiqrlgm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yongpay.top/gtgqplzskd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.feifeiyinyue.top/gtmnhhwtlz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yvedp.cn/gtahrgjcun.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.birdmap.top/gtdkswwsir.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ywan-chungtsiang.top/gtaonkzmks.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhiwuduotai.top/gtaevbympu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhoulong.xyz/gtojasbslu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangshuangyany.cn/gtgbqebhlu.html

================================================================================
来源：http://hz.jinqigfzy.top/gtnubyhoer.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sysykeji.top/gtaciwgeur.html

================================================================================
来源：http://hz.mhx1999.top/gtizsyoezu.html

[Q01] 创建表
来源：http://hz.xinyue.icu/gtdkdhvrds.html

CREATE TABLE users (
来源：http://hz.xuanzx.com/gtvovroedj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtqqrsiqts.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhongyouzk.top/gtjlwtycks.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dianchejie.cn/gtcsihmawz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxuanxn.top/gttljnqxdu.html

);
来源：http://hz.dashuyun.cn/gtnlsoukgu.html

[Q02] 创建带外键的表
来源：http://hz.ehwqpu.com/gtpdvfwusn.html

CREATE TABLE orders (
来源：http://hz.zhaomingkeji.xyz/gtfqhdxtfl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtbhicrizc.html

user_id INT NOT NULL,
来源：http://hz.jqgfzy.top/gtybcadzkg.html

amount DECIMAL(10, 2),
来源：http://hz.hnqzz.top/gtzlyabirh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhongyouzk.top/gtqcdqofxj.html

);
来源：http://hz.zhaomingkeji.xyz/gtpbufbaiu.html

[Q03] 增加列
来源：http://hz.ehwqpu.com/gtspuodhcz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ehwqpu.com/gtkeeyawkj.html

[Q04] 修改列类型
来源：http://hz.dianchejie.cn/gttbkchokq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gttyvefyiw.html

[Q05] 重命名列
来源：http://hz.zycfv.cn/gtcmbvkyrh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hongshengwenyu.top/gtwtrbtzfv.html

[Q06] 删除列
来源：http://hz.shanyushiyangkeji.top/gtwdqdvfxt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nwbrower.top/gtmjajoheh.html

[Q07] 删除表
来源：http://hz.zhiwuduotai.top/gtlhtecpvf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.daria6918.cn/gtptiqarsr.html

[Q08] 创建普通索引
来源：http://hz.0kj1m.cn/gtlytchpbh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtfotftdcb.html

[Q09] 创建唯一索引
来源：http://hz.vqdsnc.cn/gtphinfoqg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yongpay.top/gtbejevmip.html

[Q10] 插入单行
来源：http://hz.zdqjudy.top/gtxqihrmcv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.redwolf501.top/gtzvgrxhai.html

[Q11] 一次插入多行
来源：http://hz.jinyuanbaomall.cn/gtlmefxxsn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.aizwys.cn/gtaommxghh.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gtcbbseucd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gaohongyu789.top/gteyxyzhim.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gotoacloud.top/gtkxmeupyh.html

[Q13] 忽略重复插入
来源：http://hz.bjfxy.top/gtugyhciwn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.quarkkingdee.top/gtsmvfmanz.html

[Q14] 存在则更新（upsert）
来源：http://hz.fengsongda.top/gtarjomkpz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenjidiqi.icu/gtznutwgpc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhaomingkeji.xyz/gtbkkxipaf.html

[Q15] 查询全部
来源：http://hz.smart0.xyz/gtfjkgbsjh.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtpdpgejma.html

[Q16] 查询指定列
来源：http://hz.nwbrower.top/gtzshpfyux.html

SELECT id, name FROM users;
来源：http://hz.aizwys.cn/gtuxkudqjv.html

[Q17] 条件查询
来源：http://hz.iojbl.cn/gtwcsvuhpa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.9152youxi.cn/gtljrcccjo.html

[Q18] 模糊匹配
来源：http://hz.yj20258.top/gtsqshwogw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cheryme.top/gtkzenqptj.html

[Q19] 范围查询
来源：http://hz.zhijiandao.cn/gtwjzeikyy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sysykeji.top/gtjoxvfzlt.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gtlxxkpmrs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sxryk.cn/gthiwnzkzw.html

[Q21] 空值判断
来源：http://hz.yuxming.cn/gtdfxcnuhl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.havefunace.top/gthorbfckk.html

[Q22] 排序
来源：http://hz.pycfn.com/gtgdnurnsc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangdashe.top/gtbgoklyen.html

[Q23] 分页
来源：http://hz.yuanzhike.top/gtasntnnur.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dianchejie.cn/gtwidzzryi.html

[Q24] 去重
来源：http://hz.tanke756.top/gtsokfcgnq.html

SELECT DISTINCT city FROM users;
来源：http://hz.bjfxy.top/gturwzrxqb.html

[Q25] 只取前 N 条
来源：http://hz.yj20258888.top/gtufaqaums.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ybcxt.top/gttdhkpszr.html

[Q26] 计数
来源：http://hz.cdnleiting.top/gtyhkuozkl.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangdashe.top/gtrwzjocgc.html

[Q27] 条件计数
来源：http://hz.xinyue.icu/gtcbnvaolu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.svipenyu.cn/gtkrdrepsn.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtlywvdowb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jqgfzy.top/gtjykmyzua.html

[Q29] 最大最小值
来源：http://hz.bjfxy.top/gtbtwnlivd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fengsongda.top/gtyoxrxkei.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtvexbdeqs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtggoipsum.html

[Q31] 分组后过滤
来源：http://hz.meibo888.top/gtfynaddwu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jlsjyb.cn/gtmrvmncty.html

[Q32] 分组拼接字符串
来源：http://hz.ppjwa.cn/gtkltpjbfy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtysmiuhrh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sysykeji.top/gtnhrflmie.html

[Q33] 多列分组
来源：http://hz.zhiwuduotai.top/gtzpvwgdhf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.haohaochexian.top/gtyusvwfpq.html

[Q34] 每组取第一条
来源：http://hz.yanxiufei.cn/gtkjaxknxw.html

SELECT * FROM (
来源：http://hz.gaohongyu789.top/gtnkezlcbq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtoyclsuhc.html

) t WHERE rn = 1;
来源：http://hz.yj20258888.top/gtivnuxkpt.html

[Q35] 内连接
来源：http://hz.feifeiyinyue.top/gtysqevtfo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuanzx.com/gtwsdgqkgj.html

[Q36] 左连接
来源：http://hz.jiagoushi.top/gtjftqridj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gthdxxqgdk.html

[Q37] 右连接
来源：http://hz.316326.xyz/gtaqszpwpd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangtech.top/gtjoudcjeo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yonumen.top/gtmlipndxp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgufenzy.top/gtppnhfzcr.html

[Q39] 自连接（查上下级）
来源：http://hz.jinghuilouyu.cn/gtpysbjtju.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ybcxt.top/gtbpqykbkh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gtcppvjhuj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hongshengwenyu.top/gtcnrrzajg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangdashe.top/gtkhompkde.html

[Q41] 多表连接
来源：http://hz.zhengqikj.top/gtrruvfcka.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhijiandao.cn/gtrcgtcljd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gotoacloud.top/gtvgrjqrsi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigfzy.top/gtwnegzplq.html

[Q42] 连接条件附加过滤
来源：http://hz.cheryme.top/gtrznofcrj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydzc1.top/gtiexeqjtr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.316326.xyz/gtqrfnftej.html

[Q43] 标量子查询
来源：http://hz.xylfe.cn/gtyjdjwuhu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.andypj.xyz/gtkegmnzjj.html

[Q44] IN 子查询
来源：http://hz.quarkkingdee.top/gtwykumxzo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hongshengwenyu.top/gtmhibsahn.html

[Q45] EXISTS 判断存在
来源：http://hz.gzhubu.top/gtsjouzdrm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtfacbopif.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yvedp.cn/gttvxabqqm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtmekihtzn.html

[Q47] 与平均值比较
来源：http://hz.jqgfzy.top/gtypiteouk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtfzubewaz.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gthdnpwvnj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cucudq.cn/gtzfhwqbkb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yangfankeji.com/gtdwztzdft.html

[Q49] 更新单行
来源：http://hz.fzhhl.top/gtvglqymlr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhijiandao.cn/gtzviygibx.html

[Q50] 批量更新
来源：http://hz.tianlin.xyz/gtcyluhwnj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.iojbl.cn/gtufufugbr.html

[Q51] 用子查询更新
来源：http://hz.cashguo.top/gtgnqkpigw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cheryme.top/gtgsbrmxvz.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gtkfxvfhad.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinqigfzy.top/gtwopufibj.html

[Q53] 按条件删除
来源：http://hz.zhaomingkeji.xyz/gtqtejdgdw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhiwuduotai.top/gtjwwumrio.html

[Q54] 清空表
来源：http://hz.jiagoushi.top/gtvaldmowg.html

TRUNCATE TABLE logs;
来源：http://hz.wangdashe.top/gtwlhhnvsz.html

[Q55] 排名（并列占位）
来源：http://hz.hfpthk.cn/gtjflbmnns.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.haohaochexian.top/gtocfxkisi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shzxlz.cn/gtqfibodte.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shangyingyoupin.top/gtmcdjurlv.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gtsfgrpkml.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guowangkeji.top/gtllbinhfg.html

[Q58] 累计求和
来源：http://hz.wangdashe.top/gtrxdfegjh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.smart0.xyz/gtbrhhuhza.html

[Q59] 分组内累计
来源：http://hz.redwolf501.top/gtxthrmmfp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxuanxn.top/gtvgzuusqu.html

[Q60] 取上一行 / 下一行
来源：http://hz.guannengcc.top/gtfgldslqf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fzhhl.top/gtajexhpky.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gtkfcrwief.html

[Q61] 移动平均
来源：http://hz.andypj.xyz/gteijlbdyl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtaerqylgn.html

[Q62] 分组占比
来源：http://hz.nanxinkj.top/gtekemmtyz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtqqnypofr.html

[Q63] 开启事务
来源：http://hz.xinyue.icu/gtinmrekig.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.havefunace.top/gtpxbgqmde.html

[Q64] 提交事务
来源：http://hz.ydzc1.top/gtbtvqhlfr.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gtvtaanniu.html

[Q65] 回滚事务
来源：http://hz.316326.xyz/gttvvqylcn.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtcfdwrepf.html

[Q66] 行锁查询
来源：http://hz.0kj1m.cn/gtvuyksdfy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.kuanghao11.cn/gtxclhiknb.html

[Q67] 设置隔离级别
来源：http://hz.ppjwa.cn/gtgtzzurgk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jyoumei.cn/gteqbbujhk.html

[Q68] 保存点
来源：http://hz.pycfn.com/gtfvlekdsm.html

SAVEPOINT sp1;
来源：http://hz.fengsongda.top/gtqatbxzah.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtigromecn.html

[Q69] 查看执行计划
来源：http://hz.316326.xyz/gtqzxxfoqt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hnqzz.top/gtzkbkkfmm.html

[Q70] 更新统计信息
来源：http://hz.jlsjyb.cn/gtntddhcmh.html

ANALYZE TABLE users;
来源：http://hz.fengsongda.top/gtmcmjrecm.html

[Q71] 查看建表语句
来源：http://hz.zhaomingkeji.xyz/gtxmdkppkx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gtrlrlzxci.html

[Q72] 查看索引
来源：http://hz.dashuyun.cn/gttqhtictc.html

SHOW INDEX FROM users;
来源：http://hz.shzxlz.cn/gtikbjexpo.html

[Q73] 查看表状态
来源：http://hz.jqgufenzy.top/gtxdolibci.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cashguo.top/gtdoaidwgd.html

[Q74] 强制使用索引
来源：http://hz.gaohongyu789.top/gtdwdpudan.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xziqi.cn/gtxvzphnav.html

[Q75] 日期格式化
来源：http://hz.andypj.xyz/gtkekswpfb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtajizvmrp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.316326.xyz/gtqzknyzwk.html

[Q76] 按天统计
来源：http://hz.quarkkingdee.top/gtscnfcwvl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuetiantiany.cn/gtviuaccxv.html

[Q77] 时间加减
来源：http://hz.guannengcc.top/gtxyhmcuvq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dashuyun.cn/gtkqpgstix.html

[Q78] 当前时间
来源：http://hz.guannengcc.top/gtwtpvsjjl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhiwuduotai.top/gtkcbjafah.html

[Q79] 字符串拼接
来源：http://hz.zhongyouzk.top/gtnffuroiz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.vqdsnc.cn/gtungcxdtx.html

[Q80] 字符串截取
来源：http://hz.sufxvd.cn/gtavjofvrd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuxming.cn/gtlxorauqj.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gtdphmstkj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cqqwz.cn/gtxnvytmgc.html

[Q82] 字符长度与字节长度
来源：http://hz.fzhhl.top/gtwiszewqj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.vqdsnc.cn/gtwialnwjq.html

[Q83] 大小写转换
来源：http://hz.dianchejie.cn/gtdavjvkze.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tian-w.cn/gtrjgfqmcf.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtulupwskl.html

SELECT TRIM(name) FROM users;
来源：http://hz.nanxuanxn.top/gtbohrawah.html

[Q85] 数值取整
来源：http://hz.jinqigfzy.top/gtiusrylru.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gtuyzaekha.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtcfzaulkv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhongyouzk.top/gtwrvyaccy.html

[Q87] JSON 字段做条件
来源：http://hz.jinghuilouyu.cn/gtyajgroqp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.meibo888.top/gtlvrhltgf.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gtkcvpiahr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtslyqjfpm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cheryme.top/gtkfnbuafi.html

[Q89] 判断表是否存在
来源：http://hz.chenjidiqi.icu/gtcjgtnwek.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gtcmkodslw.html

[Q90] 生成序号列
来源：http://hz.wangshuangyany.cn/gtvobkieso.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtqlphejla.html

================================================================================
来源：http://hz.gogol.net.cn/gtwmqflnik.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtusovuxdo.html

================================================================================
来源：http://hz.nwbrower.top/gtjyeyhfri.html

[R01] shebang 与严格模式
来源：http://hz.haohaochexian.top/gtxxebjhso.html

#!/usr/bin/env bash
来源：http://hz.yvedp.cn/gthugdekxy.html

set -euo pipefail
来源：http://hz.pycfn.com/gtxpwmodko.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gtvryzpmnj.html

name="Tom"; echo "$name"
来源：http://hz.zhengqikj.top/gtcjdjmcff.html

[R03] 只读变量
来源：http://hz.iojbl.cn/gtwgehmqdx.html

readonly PI=3.14
来源：http://hz.cucudq.cn/gtblybsunf.html

[R04] 位置参数
来源：http://hz.cheryme.top/gtbgxvdnya.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtiyvzwhzw.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtsulrhjsn.html

name="${1:-default}"
来源：http://hz.jlsjyb.cn/gtxbvrjxkb.html

[R06] 判断命令是否存在
来源：http://hz.birdmap.top/gthazczuny.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.quarkkingdee.top/gttvlaawgm.html

[R07] if 判断文件
来源：http://hz.nanxuanxn.top/gtruiitwwo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.haohaochexian.top/gtoclpwadi.html

[R08] 数值比较
来源：http://hz.quarkkingdee.top/gtmzbeyhff.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sysykeji.top/gtxnoyftvh.html

[R09] 字符串比较
来源：http://hz.jlsjyb.cn/gtjvfwgjbb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gtrtyezcei.html

[R10] 正则匹配
来源：http://hz.cqqwz.cn/gtkglawybw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nwbrower.top/gthzcynpba.html

[R11] case 多分支
来源：http://hz.sweek.top/gtimgxzbnh.html

case "$1" in
来源：http://hz.ybcxt.top/gthmqefvrr.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gtqseqaosp.html

stop)  echo "停止" ;;
来源：http://hz.tanke756.top/gtbnqsihtf.html

*)     echo "未知命令" ;;
来源：http://hz.ppjwa.cn/gttlasnppl.html

esac
来源：http://hz.hongshengwenyu.top/gtedvghwyz.html

[R12] for 遍历文件
来源：http://hz.cheryme.top/gtlinotzze.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tanke756.top/gtwbkqrvum.html

[R13] for 计数循环
来源：http://hz.sxryk.cn/gttvjcyyfg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj202588.top/gttpalofhe.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtmlkoiqnb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gttuesaxni.html

[R15] while 逐行读文件
来源：http://hz.mhx1999.top/gthaodbdil.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fengsongda.top/gtaircrets.html

[R16] until 等待条件
来源：http://hz.zhiwuduotai.top/gthorljlqd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhoulong.xyz/gtormbkjtg.html

[R17] 数组定义与取值
来源：http://hz.yj20258888.top/gtbabkepbm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cheryme.top/gtqpisizzr.html

[R18] 遍历数组
来源：http://hz.nwbrower.top/gtzepbogub.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xinyue.icu/gtvokyilmp.html

[R19] 数组长度
来源：http://hz.fzhhl.top/gtyrjzxlyw.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtfmjxthta.html

[R20] 关联数组（字典）
来源：http://hz.cdnleiting.top/gtngssareg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtansgypvx.html

[R21] 字符串长度
来源：http://hz.316326.xyz/gtzapsmgxe.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gtumomybzf.html

[R22] 截取子串
来源：http://hz.xinyue.icu/gtqpumbika.html

echo "${s:0:5}"
来源：http://hz.cdnleiting.top/gtfgiqqlfs.html

[R23] 字符串替换
来源：http://hz.aizwys.cn/gtstsdvxky.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.haohaochexian.top/gtbzujgklz.html

[R24] 大小写转换
来源：http://hz.gaohongyu789.top/gtcbkbsyln.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.haohaochexian.top/gthzciqqib.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtpkuvvbqz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ivvv.top/gtjntfschn.html

[R26] 命令替换
来源：http://hz.smart0.xyz/gtludvunjc.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258.top/gtvxusreug.html

[R27] 算术展开
来源：http://hz.sysykeji.top/gtbypqwhbc.html

echo $((1 + 2 * 3))
来源：http://hz.c1oappe.top/gteojuhdwh.html

[R28] 浮点运算
来源：http://hz.smart0.xyz/gtqkibsupw.html

echo "scale=2; 10/3" | bc
来源：http://hz.yangfankeji.com/gtigkodcvi.html

[R29] 定义函数
来源：http://hz.yonumen.top/gtzyjvmbyf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nanxinkj.top/gtqzspjaxs.html

[R30] 函数返回状态码
来源：http://hz.snrcjt.cn/gtxdttprkr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.0kj1m.cn/gtajlcuxyh.html

[R31] 局部变量
来源：http://hz.yj20258888.top/gtrabsfoji.html

f() { local x=1; echo "$x"; }
来源：http://hz.daxiang520.top/gtgnycsoek.html

[R32] 参数个数校验
来源：http://hz.zhongyouzk.top/gtytzgkzll.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtbmtbfdza.html

[R33] 捕获错误并提示行号
来源：http://hz.yonumen.top/gtmkyeesik.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangdashe.top/gtalswkqxx.html

[R34] 退出时清理
来源：http://hz.hnqzz.top/gtqmvgybdd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtsmwcjgtf.html

[R35] 后台执行并等待
来源：http://hz.haohaochexian.top/gtssysyaws.html


<!-- 参考信息 -->