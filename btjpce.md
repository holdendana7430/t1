代发 wailian999

);
来源：http://hz.zhoulong.xyz/gtghrrhdzx.html

[Q03] 增加列
来源：http://hz.ywan-chungtsiang.top/gtxrjkmfkz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.snrcjt.cn/gtaqnsqked.html

[Q04] 修改列类型
来源：http://hz.pycfn.com/gtuyrmjywp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ivvv.top/gtrcnqkfnj.html

[Q05] 重命名列
来源：http://hz.cashguo.top/gtkzanzovr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sxryk.cn/gtznukfxtv.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtizyttdnu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.52xcode.cn/gtcwkotvow.html

[Q07] 删除表
来源：http://hz.dianchejie.cn/gtrkjuknqn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.birdmap.top/gtdacwdyve.html

[Q08] 创建普通索引
来源：http://hz.yj20258888.top/gtblbyheog.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtntdzphae.html

[Q09] 创建唯一索引
来源：http://hz.cucudq.cn/gtfkzdgbgv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtjavzcpyl.html

[Q10] 插入单行
来源：http://hz.yvedp.cn/gtzkbqkjhn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cheryme.top/gthfozxqlq.html

[Q11] 一次插入多行
来源：http://hz.sysykeji.top/gtximuhwaj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigufen.top/gthozxzehc.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gtiejdslvu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pycfn.com/gtlbkcztqu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtvlsbjmrd.html

[Q13] 忽略重复插入
来源：http://hz.smart0.xyz/gttrvgvicm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gtkelruxgw.html

[Q14] 存在则更新（upsert）
来源：http://hz.havefunace.top/gtvfylyxwb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nanxinkj.top/gtfwvzhoix.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.snrcjt.cn/gtdvomhxzs.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtlghmxtnw.html

SELECT * FROM users;
来源：http://hz.tianlin.xyz/gtrszmtigs.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtpygucqjh.html

SELECT id, name FROM users;
来源：http://hz.hywenlv.cn/gtiplatftp.html

[Q17] 条件查询
来源：http://hz.hnqzz.top/gtkercpzlu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxuanxn.top/gtljueicdq.html

[Q18] 模糊匹配
来源：http://hz.yangfankeji.com/gtylxmzspv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtkgntstfb.html

[Q19] 范围查询
来源：http://hz.meibo888.top/gtbvhzvzll.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtiqkhxnog.html

[Q20] IN 列表
来源：http://hz.guannengcc.top/gtfhizeezp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuanzx.com/gtofaxpjxq.html

[Q21] 空值判断
来源：http://hz.cucudq.cn/gtrhpcljbq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cheryme.top/gtaaioztjv.html

[Q22] 排序
来源：http://hz.gotoacloud.top/gtwzuvuhbm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinqigufen.top/gtmypyhddg.html

[Q23] 分页
来源：http://hz.havefunace.top/gtcrniylkd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ybcxt.top/gttvowfgie.html

[Q24] 去重
来源：http://hz.ywan-chungtsiang.top/gtjtyaekir.html

SELECT DISTINCT city FROM users;
来源：http://hz.jiagoushi.top/gtmozgzshv.html

[Q25] 只取前 N 条
来源：http://hz.guowangkeji.top/gtcxcovpfo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gtmwmoampq.html

[Q26] 计数
来源：http://hz.guowangkeji.top/gtsfurgbaz.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhiwuduotai.top/gtzwssptfe.html

[Q27] 条件计数
来源：http://hz.daria6918.cn/gtbmyapepc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtyfwnhikd.html

[Q28] 求和与平均
来源：http://hz.smart0.xyz/gtfwehpfqc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtpulbefij.html

[Q29] 最大最小值
来源：http://hz.feifeiyinyue.top/gtkrfgfiel.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yangfankeji.com/gthlrfmesw.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gthzuyrepp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtzpvmdgze.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtqyeggydo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.9152youxi.cn/gtxmozyafz.html

[Q32] 分组拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtneycvtjl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gteoglmfuo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.52xcode.cn/gtlwzxdnzb.html

[Q33] 多列分组
来源：http://hz.zhiwuduotai.top/gthwqooesw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cheryme.top/gtdclpupdl.html

[Q34] 每组取第一条
来源：http://hz.gaohongyu789.top/gtgmauuqau.html

SELECT * FROM (
来源：http://hz.dashuyun.cn/gtzkrpvuiz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gtkbdafvlq.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtgxpmovow.html

[Q35] 内连接
来源：http://hz.yongpay.top/gtyuizcugd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gtxlwgiper.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtncvtudmh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.havefunace.top/gthcsreuhu.html

[Q37] 右连接
来源：http://hz.shzxlz.cn/gtemiblzge.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dianchejie.cn/gtfwxztcgi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daria6918.cn/gtasxvoors.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jlsjyb.cn/gtreidrxeg.html

[Q39] 自连接（查上下级）
来源：http://hz.ydzc1.top/gtydkeybrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.havefunace.top/gtwioicxcj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.svipenyu.cn/gtghdionaq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxinkj.top/gtfmwgktyh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yangfankeji.com/gtjfqwsexw.html

[Q41] 多表连接
来源：http://hz.cucudq.cn/gtovbgngea.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtczmmdunx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtxmsewkxi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.vqdsnc.cn/gtgrhwrmrl.html

[Q42] 连接条件附加过滤
来源：http://hz.bjfxy.top/gtcbeyzzes.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gtipvsftxi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hnxiangtu.top/gtjclbhxce.html

[Q43] 标量子查询
来源：http://hz.birdmap.top/gtraoajrlh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenjidiqi.icu/gtqrhlihhd.html

[Q44] IN 子查询
来源：http://hz.jinqigfzy.top/gtqexziedl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgufenzy.top/gtuwnxtojc.html

[Q45] EXISTS 判断存在
来源：http://hz.sxryk.cn/gtfagorfle.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gtrrurnfti.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sxryk.cn/gtidblxsbr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtgkvittyq.html

[Q47] 与平均值比较
来源：http://hz.guowangkeji.top/gtnyyccort.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xinyue.icu/gtgavptabb.html

[Q48] CTE 公用表表达式
来源：http://hz.feifeiyinyue.top/gtczrtnjqz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuetiantiany.cn/gtqlsuxuaw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yuxming.cn/gtajopbqpk.html

[Q49] 更新单行
来源：http://hz.sweek.top/gtmtghposv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xziqi.cn/gtavgowimf.html

[Q50] 批量更新
来源：http://hz.ydzc1.top/gtmudvlrlf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jlsjyb.cn/gtnnbygpiq.html

[Q51] 用子查询更新
来源：http://hz.feifeiyinyue.top/gtliknngwh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtarhzimdx.html

[Q52] 删除指定行
来源：http://hz.jinqigfzy.top/gtofhdwsae.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gtzlbfanox.html

[Q53] 按条件删除
来源：http://hz.zycfv.cn/gtkilvepot.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sufxvd.cn/gtzxspzmtu.html

[Q54] 清空表
来源：http://hz.jlsjyb.cn/gtqqayoinn.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtaoeqbwkx.html

[Q55] 排名（并列占位）
来源：http://hz.jqgfzy.top/gtahunvcqp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.iojbl.cn/gtkdfiixzi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yonumen.top/gtyydxxalk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ppjwa.cn/gtymskclhr.html

[Q57] 行号
来源：http://hz.tian-w.cn/gtyxekueqt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.dashuyun.cn/gtypzfbrrx.html

[Q58] 累计求和
来源：http://hz.pycfn.com/gtdoivhzxc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangshuangyany.cn/gtpfbazgmp.html

[Q59] 分组内累计
来源：http://hz.xuanzx.com/gtypmlnmwe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tianlin.xyz/gtxqbbgrwh.html

[Q60] 取上一行 / 下一行
来源：http://hz.aibaodan.cn/gtcttitjpw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ppjwa.cn/gttnyeyozw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ivvv.top/gttahcghfa.html

[Q61] 移动平均
来源：http://hz.zdqjudy.top/gtjwxxrupm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhengqikj.top/gtlguygzoa.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gtpumfscyv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtqbyfqnvd.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtvidrmmzi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuanzhike.top/gteiexbqbh.html

[Q64] 提交事务
来源：http://hz.zhixingplan.top/gtvypkddbh.html

COMMIT;
来源：http://hz.daria6918.cn/gtknmgbrxh.html

[Q65] 回滚事务
来源：http://hz.svipenyu.cn/gtbnqvhsnw.html

ROLLBACK;
来源：http://hz.hnxiangtu.top/gtuftjxuje.html

[Q66] 行锁查询
来源：http://hz.andypj.xyz/gthxgxpees.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cqqwz.cn/gtxiikcxhh.html

[Q67] 设置隔离级别
来源：http://hz.hongshengwenyu.top/gtbadodekl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtbbrskdng.html

[Q68] 保存点
来源：http://hz.yanxiufei.cn/gtqnextmxm.html

SAVEPOINT sp1;
来源：http://hz.quarkkingdee.top/gtogtwbffo.html

ROLLBACK TO sp1;
来源：http://hz.sweek.top/gtzxykztkr.html

[Q69] 查看执行计划
来源：http://hz.yj20258888.top/gtojxqiyts.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shuidangran.top/gtnofntxwz.html

[Q70] 更新统计信息
来源：http://hz.gaohongyu789.top/gtmpxgugcw.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangkeji.top/gtqcxktexc.html

[Q71] 查看建表语句
来源：http://hz.gaohongyu789.top/gtoxmhtwqs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtdsqomvyg.html

[Q72] 查看索引
来源：http://hz.jinqigufen.top/gtldteajja.html

SHOW INDEX FROM users;
来源：http://hz.yonumen.top/gtwsznwqwv.html

[Q73] 查看表状态
来源：http://hz.dashuyun.cn/gtgdgwanqn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cashguo.top/gtdmlskaaa.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtfgiofrmj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinghuilouyu.cn/gtcfhorehn.html

[Q75] 日期格式化
来源：http://hz.vqdsnc.cn/gtylcikmon.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.vqdsnc.cn/gtdjbwndnc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hywenlv.cn/gtpnockvmv.html

[Q76] 按天统计
来源：http://hz.yonumen.top/gtoaykagil.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.0kj1m.cn/gtyurdrpgg.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gtvsolowai.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ivvv.top/gtfabblplp.html

[Q78] 当前时间
来源：http://hz.xylfe.cn/gtocqspyvt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ydjk.org.cn/gtyfdcpywd.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangtech.top/gtvfeqrabf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigufen.top/gtwuorbwtt.html

[Q80] 字符串截取
来源：http://hz.hongshengwenyu.top/gtseqaulbq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydzc1.top/gtbkcwrcde.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gtfrgszrfg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtrqudgxzr.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gtqvcymwkw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtjvpuvbtv.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtmtivaxan.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gtgvfsgabo.html

[Q84] 去除首尾空格
来源：http://hz.52xcode.cn/gtdzcrtuqy.html

SELECT TRIM(name) FROM users;
来源：http://hz.svipenyu.cn/gttrmrhdqa.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtxmxarbzr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tianlin.xyz/gtmpkoakor.html

[Q86] 读取 JSON 字段
来源：http://hz.hnxiangtu.top/gtwmpygdvf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hammf.cn/gtvselyyhb.html

[Q87] JSON 字段做条件
来源：http://hz.xinyue.icu/gtdleiagqd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.kuanghao11.cn/gtzgdtylap.html

[Q88] 行转列（条件聚合）
来源：http://hz.birdmap.top/gtvtvhfaof.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yanxiufei.cn/gtfpoooyem.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxuanxn.top/gtjhuvaplk.html

[Q89] 判断表是否存在
来源：http://hz.316326.xyz/gtgmebjtqi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gtzfewdola.html

[Q90] 生成序号列
来源：http://hz.yj20258888.top/gtdmpyxmvy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigufen.top/gtxdspnnnw.html

================================================================================
来源：http://hz.pycfn.com/gtbufpmitz.html

R. Bash 专题
来源：http://hz.hnxiangtu.top/gtfdxfxfss.html

================================================================================
来源：http://hz.hnxiangtu.top/gthzmkhvxd.html

[R01] shebang 与严格模式
来源：http://hz.redwolf501.top/gtapljoamk.html

#!/usr/bin/env bash
来源：http://hz.xuetiantiany.cn/gtlbgdbsvz.html

set -euo pipefail
来源：http://hz.xylfe.cn/gttgsnmelb.html

[R02] 变量赋值与使用
来源：http://hz.ywan-chungtsiang.top/gteqdsxcpm.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangtech.top/gtzhdxukbt.html

[R03] 只读变量
来源：http://hz.gaohongyu789.top/gtyvocbxgy.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtjwpdliyf.html

[R04] 位置参数
来源：http://hz.jianghu66.top/gtkwalpxxp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cucudq.cn/gtclhgaspz.html

[R05] 参数默认值
来源：http://hz.sxryk.cn/gtyxcxvntk.html

name="${1:-default}"
来源：http://hz.ydzc1.top/gtvfnohnfq.html

[R06] 判断命令是否存在
来源：http://hz.jinqigfzy.top/gtmudfzybn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.quarkkingdee.top/gtjtucmqua.html

[R07] if 判断文件
来源：http://hz.vqdsnc.cn/gtifnqzgnn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ehwqpu.com/gtmadgjrih.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtqteoebws.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgufenzy.top/gtyecflaeb.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtfljdefnh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinghuilouyu.cn/gtayeikrso.html

[R10] 正则匹配
来源：http://hz.yanxiufei.cn/gtnskcbgtx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj202588.top/gtmfqwmbpr.html

[R11] case 多分支
来源：http://hz.yvedp.cn/gtnsfpmxwd.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gtafdocshw.html

start) echo "启动" ;;
来源：http://hz.zhaomingkeji.xyz/gtgfkmeiyl.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtudgktdxk.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gtudadwjhg.html

esac
来源：http://hz.yj20258888.top/gtwqecjyka.html

[R12] for 遍历文件
来源：http://hz.vqdsnc.cn/gtaltotzev.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yonumen.top/gtmykpfxea.html

[R13] for 计数循环
来源：http://hz.yj202588.top/gtxatszdrw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnxiangtu.top/gtgznqjclj.html

[R14] C 风格 for
来源：http://hz.xinyue.icu/gtfhkufmth.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dianchejie.cn/gtgsaxddon.html

[R15] while 逐行读文件
来源：http://hz.aibaodan.cn/gtcyaenhsf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.feifeiyinyue.top/gtosryacne.html

[R16] until 等待条件
来源：http://hz.daxiang520.top/gtecwryaao.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dashuyun.cn/gtcjikcsty.html

[R17] 数组定义与取值
来源：http://hz.cucudq.cn/gthjzozryl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shzxlz.cn/gtilhujqne.html

[R18] 遍历数组
来源：http://hz.redwolf501.top/gtlggfizzz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tanke756.top/gtdpwdhwve.html

[R19] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtumvwpoul.html

echo "${#arr[@]}"
来源：http://hz.jqgufenzy.top/gtfcvrlieh.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gtfebkzrtd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.mhx1999.top/gtkccmlpuq.html

[R21] 字符串长度
来源：http://hz.jinqigufen.top/gtwhtfrosa.html

echo "${#s}"
来源：http://hz.zhixingplan.top/gtqhgazhra.html

[R22] 截取子串
来源：http://hz.iojbl.cn/gtxjwljhfy.html

echo "${s:0:5}"
来源：http://hz.cashguo.top/gtycpiupvb.html

[R23] 字符串替换
来源：http://hz.sufxvd.cn/gtlfshxrfx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhaomingkeji.xyz/gthirfdtdg.html

[R24] 大小写转换
来源：http://hz.cdnleiting.top/gtzasjghmw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gthzuslpwv.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258888.top/gtlztigioa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.9152youxi.cn/gtifrkgjhn.html

[R26] 命令替换
来源：http://hz.andypj.xyz/gtektsngjy.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gttdzbdhqd.html

[R27] 算术展开
来源：http://hz.hnxiangtu.top/gtrpelhseb.html

echo $((1 + 2 * 3))
来源：http://hz.ehwqpu.com/gtpygjklmx.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtrocjjkeh.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangkeji.top/gtrdtennvc.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtztpfqjhp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cheryme.top/gtoozkwaju.html

[R30] 函数返回状态码
来源：http://hz.vqdsnc.cn/gtiakypjkb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.havefunace.top/gtlhnzkcxb.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gtswogbypv.html

f() { local x=1; echo "$x"; }
来源：http://hz.hywenlv.cn/gtcwkyirpu.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtdxqakljj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gzhubu.top/gtkitfvwxs.html

[R33] 捕获错误并提示行号
来源：http://hz.xingfuxueyuan.xyz/gtqpuosbjs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtmgmxvniz.html

[R34] 退出时清理
来源：http://hz.hywenlv.cn/gtjhsbajlq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gttqcsysqg.html

[R35] 后台执行并等待
来源：http://hz.yvedp.cn/gteoeyigka.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gotoacloud.top/gtfkfmznka.html

[R36] 并发执行多个任务
来源：http://hz.havefunace.top/gtvyinewrb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenjidiqi.icu/gtmhjoucxj.html

[R37] 把输出赋给变量
来源：http://hz.birdmap.top/gtbxhyhbjo.html

files=$(ls -1)
来源：http://hz.cheryme.top/gteaotjvvw.html

[R38] 管道串联
来源：http://hz.zhaomingkeji.xyz/gtriuvobfp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtqoppldxc.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangtech.top/gtnrnlvoyv.html

cmd > out.log 2>&1
来源：http://hz.zdqjudy.top/gtbzhedzam.html

[R40] 追加写日志
来源：http://hz.jinghuilouyu.cn/gtzwdgeqjb.html

echo "log" >> out.log
来源：http://hz.mhx1999.top/gtctlllrbw.html

[R41] 丢弃输出
来源：http://hz.zhixingplan.top/gtgjgazxzj.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtrgwbfvss.html

[R42] 输入重定向
来源：http://hz.xuanzx.com/gtxaxizkie.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtlhzfmojd.html

[R43] 按名字查找文件
来源：http://hz.cashguo.top/gtgjkloezd.html

find . -name "*.log" -type f
来源：http://hz.havefunace.top/gtfaodcyzj.html

[R44] 按修改时间查找
来源：http://hz.xylfe.cn/gtxxqdxtwe.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtudkfqmsj.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtxfhzjwvv.html

find . -name "*.tmp" -delete
来源：http://hz.jqgufenzy.top/gtjjzqjvqj.html

[R46] 递归替换文件内容
来源：http://hz.tian-w.cn/gtfzpucich.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gticcxusqd.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtyvnqzbye.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.meibo888.top/gtnzmfybth.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtfzctqaiv.html

awk '{print $1, $3}' a.txt
来源：http://hz.aizwys.cn/gtbbfhocib.html

[R49] awk 带条件
来源：http://hz.c1oappe.top/gtibrydzry.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daria6918.cn/gtsjqeivez.html

[R50] awk 求和
来源：http://hz.zhongyouzk.top/gtefxyxgtf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jqgfzy.top/gtiorlcvpw.html

[R51] 排序去重取前几
来源：http://hz.yuxming.cn/gtjwhjlrlr.html


<!-- 参考信息 -->