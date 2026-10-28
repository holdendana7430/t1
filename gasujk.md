代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sysykeji.top/gtonmiecrs.html

user_id INT NOT NULL,
来源：http://hz.dashuyun.cn/gtiboujjxb.html

amount DECIMAL(10, 2),
来源：http://hz.jianghu66.top/gtoomwylsc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.0kj1m.cn/gtxczmzdle.html

);
来源：http://hz.cdnleiting.top/gtuyresmgi.html

[Q03] 增加列
来源：http://hz.shanyushiyangkeji.top/gteaxguovh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigufen.top/gtvzvdgfpc.html

[Q04] 修改列类型
来源：http://hz.xuetiantiany.cn/gtdiicdkoq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj20258.top/gtphuqoatk.html

[Q05] 重命名列
来源：http://hz.pengpengdd.cyou/gtytqxlrzz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangkeji.top/gtuarzpnqc.html

[Q06] 删除列
来源：http://hz.aibaodan.cn/gtvwxuxpml.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhaomingkeji.xyz/gtbizxqvil.html

[Q07] 删除表
来源：http://hz.nanxinkj.top/gthgifthem.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guannengcc.top/gtretmfvix.html

[Q08] 创建普通索引
来源：http://hz.feifeiyinyue.top/gtglmfmcyy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yongpay.top/gtbqxhpshx.html

[Q09] 创建唯一索引
来源：http://hz.zhoulong.xyz/gtsitrblzn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sweek.top/gtvsyxgweo.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gtqvaipywz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtwalfvnuq.html

[Q11] 一次插入多行
来源：http://hz.jinghuilouyu.cn/gtkwewrlsm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj202588.top/gtzfjzqqyg.html

[Q12] 插入后取自增 ID
来源：http://hz.chenzaomai.com/gtozpiglhj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nwbrower.top/gtqbxugaxj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ywan-chungtsiang.top/gtvmrnskdo.html

[Q13] 忽略重复插入
来源：http://hz.zhongyouzk.top/gtwlrrwavf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yvedp.cn/gtkjuxssik.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinyuanbaomall.cn/gtxhumojib.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ppjwa.cn/gtaljhowaq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenjidiqi.icu/gtqfxgktqb.html

[Q15] 查询全部
来源：http://hz.svipenyu.cn/gtnknzsyap.html

SELECT * FROM users;
来源：http://hz.zhongyouzk.top/gtfqjnojeq.html

[Q16] 查询指定列
来源：http://hz.meibo888.top/gtkqyctqje.html

SELECT id, name FROM users;
来源：http://hz.kuanghao11.cn/gtegtyuqyf.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtjskjriho.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cheryme.top/gtysrymvne.html

[Q18] 模糊匹配
来源：http://hz.jinghuilouyu.cn/gteguhclei.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shzxlz.cn/gtqeegximg.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gtufgthfxa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.fzhhl.top/gtgkdjwxqf.html

[Q20] IN 列表
来源：http://hz.tian-w.cn/gtzeujkvan.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shanyushiyangkeji.top/gtqqvspthy.html

[Q21] 空值判断
来源：http://hz.sysykeji.top/gtmswqcpyo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fengsongda.top/gttkcynvgs.html

[Q22] 排序
来源：http://hz.dianchejie.cn/gtbimfdjfj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gaohongyu789.top/gtnudywhcf.html

[Q23] 分页
来源：http://hz.hfpthk.cn/gtcbtrmdqv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgfzy.top/gtwdpnpdol.html

[Q24] 去重
来源：http://hz.dashuyun.cn/gtcctnupzh.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gtyaimtjtj.html

[Q25] 只取前 N 条
来源：http://hz.jyoumei.cn/gtyvavuokj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tianlin.xyz/gtljyrqele.html

[Q26] 计数
来源：http://hz.jqgfzy.top/gttzqimmmr.html

SELECT COUNT(*) FROM users;
来源：http://hz.haohaochexian.top/gtpbfmohby.html

[Q27] 条件计数
来源：http://hz.yuxming.cn/gtwdnrokan.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cheryme.top/gtzloiqkvf.html

[Q28] 求和与平均
来源：http://hz.0kj1m.cn/gtgjlaolbl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenjidiqi.icu/gtcfijvsfs.html

[Q29] 最大最小值
来源：http://hz.cqqwz.cn/gtfstwmnjr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xylfe.cn/gtdkrktmim.html

[Q30] 分组统计
来源：http://hz.yuanzhike.top/gtayszvvog.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtikbhslvv.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtkeljexbp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.mhx1999.top/gtxphwmrot.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigufen.top/gtnvtpsyeb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtezqlhqra.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yangfankeji.com/gtqoqwycim.html

[Q33] 多列分组
来源：http://hz.c1oappe.top/gtcgxvuslu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tanke756.top/gtsrrzdwof.html

[Q34] 每组取第一条
来源：http://hz.shzxlz.cn/gtjzxpxuhm.html

SELECT * FROM (
来源：http://hz.jinyuanbaomall.cn/gtgtbeeqju.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtrrkfidhl.html

) t WHERE rn = 1;
来源：http://hz.ehwqpu.com/gtuqfgmvza.html

[Q35] 内连接
来源：http://hz.jiagoushi.top/gtgsxhsvyu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenjidiqi.icu/gtkowkpjxd.html

[Q36] 左连接
来源：http://hz.tian-w.cn/gtrdiwiust.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtoablddxp.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtleqxykkd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gtdrjksqpf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gtmfzbform.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ybcxt.top/gtbrngzhqc.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gtzcftpoeg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtkicwihus.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangshuangyany.cn/gtkocsoisw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hnxiangtu.top/gtmvgxcvni.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhiwuduotai.top/gtcxhxlajh.html

[Q41] 多表连接
来源：http://hz.sweek.top/gtsmyofxra.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xinyue.icu/gtoaumyket.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258.top/gtqkxnnnsi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xziqi.cn/gtbljbtkuh.html

[Q42] 连接条件附加过滤
来源：http://hz.dianchejie.cn/gtubrxosgp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nanxinkj.top/gtdjjzbcns.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtiuvjtmvh.html

[Q43] 标量子查询
来源：http://hz.hysaishi.cn/gtkxxmuyqs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tanke756.top/gtupomgmdv.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gtelamjrfi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.9152youxi.cn/gttepnshac.html

[Q45] EXISTS 判断存在
来源：http://hz.dianchejie.cn/gtnawjzmhu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtebhkswkl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtohkksevh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtbqqcvjqg.html

[Q47] 与平均值比较
来源：http://hz.hnqzz.top/gtiftvgcbr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgfzy.top/gtwwwnjggc.html

[Q48] CTE 公用表表达式
来源：http://hz.jlsjyb.cn/gtiqxxlgfd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aizwys.cn/gtcatuetcf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhixingplan.top/gtvsefmmfi.html

[Q49] 更新单行
来源：http://hz.gotoacloud.top/gthzblhvih.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cucudq.cn/gthyeigofu.html

[Q50] 批量更新
来源：http://hz.zhiwuduotai.top/gtsgletnga.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guannengcc.top/gtwlvnxiwz.html

[Q51] 用子查询更新
来源：http://hz.zhongyouzk.top/gtfbksejgg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.birdmap.top/gtzmfxkhcn.html

[Q52] 删除指定行
来源：http://hz.xuanzx.com/gtmfekfjyp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gaohongyu789.top/gtnxbcmcog.html

[Q53] 按条件删除
来源：http://hz.aizwys.cn/gtafmllayp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.haohaochexian.top/gtjspnqrec.html

[Q54] 清空表
来源：http://hz.ybcxt.top/gthrgmfjye.html

TRUNCATE TABLE logs;
来源：http://hz.wangshuangyany.cn/gtqbwowavy.html

[Q55] 排名（并列占位）
来源：http://hz.cheryme.top/gtnphzqnox.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuanzhike.top/gtqsdpbsrc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuetiantiany.cn/gtwpzcgier.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuanzhike.top/gthdyuswld.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtkmdhcjrc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gotoacloud.top/gtxwmoqlut.html

[Q58] 累计求和
来源：http://hz.xylfe.cn/gthxsbmdkx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yueranfly.top/gtzjuycqhy.html

[Q59] 分组内累计
来源：http://hz.sxryk.cn/gtyrbxuzbi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuetiantiany.cn/gtkxkdripx.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydjk.org.cn/gtyaulvbzb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.haohaochexian.top/gtytshqshw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtmehjiumm.html

[Q61] 移动平均
来源：http://hz.cdnleiting.top/gtcdkjqewl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gotoacloud.top/gtoncfmjfc.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtaewbfdhm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtntdgzwwj.html

[Q63] 开启事务
来源：http://hz.iojbl.cn/gtoxclgoom.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhijiandao.cn/gtdyshgvfp.html

[Q64] 提交事务
来源：http://hz.tian-w.cn/gtxxhlvoln.html

COMMIT;
来源：http://hz.guannengcc.top/gtmugbvawg.html

[Q65] 回滚事务
来源：http://hz.hnqzz.top/gtqshwvevg.html

ROLLBACK;
来源：http://hz.zhoulong.xyz/gtjurzztyf.html

[Q66] 行锁查询
来源：http://hz.chenjidiqi.icu/gtrjjybbfq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhiwuduotai.top/gtelwibuug.html

[Q67] 设置隔离级别
来源：http://hz.xziqi.cn/gttxutrfjm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtldnemztu.html

[Q68] 保存点
来源：http://hz.zhixingplan.top/gtppsdoupf.html

SAVEPOINT sp1;
来源：http://hz.hfpthk.cn/gtygyaxwyx.html

ROLLBACK TO sp1;
来源：http://hz.zhaomingkeji.xyz/gtdgtpgnpr.html

[Q69] 查看执行计划
来源：http://hz.chenjidiqi.icu/gtvokgerwn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tian-w.cn/gtxwvqrxiz.html

[Q70] 更新统计信息
来源：http://hz.birdmap.top/gtcradtxnx.html

ANALYZE TABLE users;
来源：http://hz.wangdashe.top/gtxylkmgwt.html

[Q71] 查看建表语句
来源：http://hz.yj20258888.top/gtjbbyqobx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gttfjozljz.html

[Q72] 查看索引
来源：http://hz.hnqzz.top/gtlvwwjnwn.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtkhxoyqkv.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtsezaeycw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ivvv.top/gtnjjlwtoz.html

[Q74] 强制使用索引
来源：http://hz.tianlin.xyz/gtmxidscid.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenzaomai.com/gtftzkbrut.html

[Q75] 日期格式化
来源：http://hz.ivvv.top/gtxctyamkm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hongshengwenyu.top/gtgoicearl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dashuyun.cn/gtrmbqcfjh.html

[Q76] 按天统计
来源：http://hz.cucudq.cn/gtzhtbjdba.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yangfankeji.com/gtsdkdkvib.html

[Q77] 时间加减
来源：http://hz.hysaishi.cn/gtkeqgiszb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jiagoushi.top/gtjoywjzwo.html

[Q78] 当前时间
来源：http://hz.zhoulong.xyz/gtitalnvzm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gotoacloud.top/gtnyznnngs.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtdczipprf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hywenlv.cn/gtlcysdmvi.html

[Q80] 字符串截取
来源：http://hz.xylfe.cn/gtgsddjmbn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenjidiqi.icu/gthgjfveap.html

[Q81] 字符串替换
来源：http://hz.daria6918.cn/gtllvihmyt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258.top/gthttdhjpe.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gtovvetqja.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ppjwa.cn/gtlrywfick.html

[Q83] 大小写转换
来源：http://hz.ydjk.org.cn/gtutbqzufn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.smart0.xyz/gthoagprsl.html

[Q84] 去除首尾空格
来源：http://hz.ybcxt.top/gteysabrov.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigfzy.top/gtzamdbyfv.html

[Q85] 数值取整
来源：http://hz.haohaochexian.top/gtccixnskj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtqdmxqkhw.html

[Q86] 读取 JSON 字段
来源：http://hz.yuxming.cn/gterlqcygm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tian-w.cn/gtenljriqu.html

[Q87] JSON 字段做条件
来源：http://hz.dianchejie.cn/gtzqmjydim.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shuidangran.top/gtujhnqjgv.html

[Q88] 行转列（条件聚合）
来源：http://hz.shzxlz.cn/gtogpeitcm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hfpthk.cn/gtqomxhwun.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhiwuduotai.top/gtqfkrzqcw.html

[Q89] 判断表是否存在
来源：http://hz.wangshuangyany.cn/gtuvhmzfne.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxinkj.top/gtcloafsbq.html

[Q90] 生成序号列
来源：http://hz.daria6918.cn/gtklhbecpm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhiwuduotai.top/gtusavxzlm.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbbtxnnmt.html

R. Bash 专题
来源：http://hz.daria6918.cn/gtalhkfqeq.html

================================================================================
来源：http://hz.zycfv.cn/gtjboaalrs.html

[R01] shebang 与严格模式
来源：http://hz.jinghuilouyu.cn/gtzwvgqauo.html

#!/usr/bin/env bash
来源：http://hz.yonumen.top/gtfdittqzs.html

set -euo pipefail
来源：http://hz.nanxuanxn.top/gtwixecxng.html

[R02] 变量赋值与使用
来源：http://hz.guowangkeji.top/gtqivlppnv.html

name="Tom"; echo "$name"
来源：http://hz.gogol.net.cn/gtiystqvjf.html

[R03] 只读变量
来源：http://hz.shanyushiyangkeji.top/gttbrkwypy.html

readonly PI=3.14
来源：http://hz.xuetiantiany.cn/gtcuawelzc.html

[R04] 位置参数
来源：http://hz.zycfv.cn/gtxjshmkdm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ybcxt.top/gtmujtjlti.html

[R05] 参数默认值
来源：http://hz.xingfuxueyuan.xyz/gtpgdqaaum.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtjjyqhicg.html

[R06] 判断命令是否存在
来源：http://hz.sweek.top/gtpwzighrg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.9152youxi.cn/gttkxwpree.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gthdhqqwnl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shangyingyoupin.top/gtiiyaxvrw.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtnbsbydfi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guowangkeji.top/gtdlkgvzsh.html

[R09] 字符串比较
来源：http://hz.chenjidiqi.icu/gtdnilvrnj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtszxiqunh.html

[R10] 正则匹配
来源：http://hz.snrcjt.cn/gtytnebjlf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtwuzmfqpc.html

[R11] case 多分支
来源：http://hz.hysaishi.cn/gtdztfonbp.html

case "$1" in
来源：http://hz.gzhubu.top/gtzfaswvpn.html

start) echo "启动" ;;
来源：http://hz.yongpay.top/gtmyqufkys.html

stop)  echo "停止" ;;
来源：http://hz.shuidangran.top/gtpczbguyp.html

*)     echo "未知命令" ;;
来源：http://hz.jiagoushi.top/gtqyvsuquw.html

esac
来源：http://hz.xingfuxueyuan.xyz/gtltgjotvu.html

[R12] for 遍历文件
来源：http://hz.hammf.cn/gtoojqbnhp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydzc1.top/gtdelzgypw.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtjbptqzli.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.redwolf501.top/gtgqsusptc.html

[R14] C 风格 for
来源：http://hz.xuanzx.com/gtpzfezsrf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xylfe.cn/gtmixpkdpe.html

[R15] while 逐行读文件
来源：http://hz.hfpthk.cn/gtmazmzamu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tanke756.top/gttzntcupi.html

[R16] until 等待条件
来源：http://hz.xylfe.cn/gtgxyistah.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.9152youxi.cn/gtyuobfakh.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gtobgaizyv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtvxbruajm.html

[R18] 遍历数组
来源：http://hz.dashuyun.cn/gtgpatbsuz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cdnleiting.top/gtcovktthq.html

[R19] 数组长度
来源：http://hz.hnxiangtu.top/gtcdhzxlbn.html

echo "${#arr[@]}"
来源：http://hz.chenlongwang.top/gtegkrbkjw.html

[R20] 关联数组（字典）
来源：http://hz.hfpthk.cn/gtmwkgcxqm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sysykeji.top/gtrfpzuxtr.html

[R21] 字符串长度
来源：http://hz.hnqzz.top/gtoomwlwoo.html

echo "${#s}"
来源：http://hz.tanke756.top/gtmvwrvnyb.html

[R22] 截取子串
来源：http://hz.yongpay.top/gtklzajnxo.html

echo "${s:0:5}"
来源：http://hz.hnxiangtu.top/gtijodznxb.html

[R23] 字符串替换
来源：http://hz.fzhhl.top/gtiafukdai.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xziqi.cn/gtdlaukeja.html

[R24] 大小写转换
来源：http://hz.gzhubu.top/gtsjpbtrkk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.feifeiyinyue.top/gtipjxpyxo.html

[R25] 去后缀 / 去前缀
来源：http://hz.tianlin.xyz/gtqrefmofc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sxryk.cn/gtnxjoksqx.html

[R26] 命令替换
来源：http://hz.xinyue.icu/gtccsrxzyz.html

now=$(date +%F); echo "$now"
来源：http://hz.sysykeji.top/gtwjwfukfu.html

[R27] 算术展开
来源：http://hz.hysaishi.cn/gtnkdgwyky.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtwjluehgt.html

[R28] 浮点运算
来源：http://hz.yj202588.top/gteckafrik.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtxzjqlafd.html

[R29] 定义函数
来源：http://hz.ehwqpu.com/gthnzmrmvc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenjidiqi.icu/gtqbcrwevm.html

[R30] 函数返回状态码
来源：http://hz.meibo888.top/gtdfxffnok.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtodgrnufk.html

[R31] 局部变量
来源：http://hz.hnxiangtu.top/gtmpqblcbp.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtiuqplihl.html

[R32] 参数个数校验
来源：http://hz.hywenlv.cn/gtawohzknv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xylfe.cn/gtxnrkmfjj.html

[R33] 捕获错误并提示行号
来源：http://hz.daria6918.cn/gteyciydzq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sxryk.cn/gtmfkodhli.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtpcwbtrxg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guannengcc.top/gthnmqzvsf.html

[R35] 后台执行并等待
来源：http://hz.sweek.top/gtosrdipza.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gogol.net.cn/gtqlzgrgcc.html

[R36] 并发执行多个任务
来源：http://hz.jyoumei.cn/gtfkkpqfww.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hysaishi.cn/gtqrgphaps.html

[R37] 把输出赋给变量
来源：http://hz.hysaishi.cn/gtykywmwgm.html

files=$(ls -1)
来源：http://hz.yongpay.top/gtyopbqmmv.html

[R38] 管道串联
来源：http://hz.zycfv.cn/gtilnnkrmi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cheryme.top/gtdxieombh.html

[R39] 重定向标准输出与错误
来源：http://hz.yongpay.top/gtlmnaskmy.html

cmd > out.log 2>&1
来源：http://hz.jianghu66.top/gtmwbrocbv.html

[R40] 追加写日志
来源：http://hz.yvedp.cn/gtenjdnpju.html

echo "log" >> out.log
来源：http://hz.yonumen.top/gtazyeiklw.html

[R41] 丢弃输出
来源：http://hz.mhx1999.top/gtssgsfiav.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtugkoswvg.html

[R42] 输入重定向
来源：http://hz.sweek.top/gtldqqgwgh.html

wc -l < a.txt
来源：http://hz.shzxlz.cn/gtucxfezru.html

[R43] 按名字查找文件
来源：http://hz.xinyue.icu/gtslwwemuf.html

find . -name "*.log" -type f
来源：http://hz.yj20258888.top/gtzqsnncxs.html

[R44] 按修改时间查找
来源：http://hz.ydzc1.top/gtmjbiqddv.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtluyrnupm.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gtztwwmmsk.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtoeuuzbeh.html

[R46] 递归替换文件内容
来源：http://hz.yueranfly.top/gtogerlson.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnxiangtu.top/gtghlzfuwi.html

[R47] sed 单行替换
来源：http://hz.yueranfly.top/gtshjrippi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yanxiufei.cn/gttsdpconu.html

[R48] awk 取指定列
来源：http://hz.haohaochexian.top/gtxchzcfrr.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtvapbkbni.html

[R49] awk 带条件
来源：http://hz.jinghuilouyu.cn/gtxvtyzbns.html


<!-- 参考信息 -->