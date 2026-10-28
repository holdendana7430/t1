代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gttgfprvgb.html

user_id INT NOT NULL,
来源：http://hz.daxiang520.top/gtylnetwjw.html

amount DECIMAL(10, 2),
来源：http://hz.xziqi.cn/gtpoybujmp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtaomlenty.html

);
来源：http://hz.yj20258.top/gtctwfphpe.html

[Q03] 增加列
来源：http://hz.jiagoushi.top/gtmfgdtfoj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.snrcjt.cn/gtxzfwophn.html

[Q04] 修改列类型
来源：http://hz.shzxlz.cn/gtjwjxjkya.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.kuanghao11.cn/gtbltlzrnz.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtuiyerxlt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.316326.xyz/gtsoutseab.html

[Q06] 删除列
来源：http://hz.guowangkeji.top/gtkwabmkba.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ppjwa.cn/gtdzsgtlmz.html

[Q07] 删除表
来源：http://hz.cqqwz.cn/gtloojtsej.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gaohongyu789.top/gtovyjoqnp.html

[Q08] 创建普通索引
来源：http://hz.kuanghao11.cn/gtcwfmssff.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtzqenzzxm.html

[Q09] 创建唯一索引
来源：http://hz.yj20258888.top/gtcwocmjgk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtsgrxudnx.html

[Q10] 插入单行
来源：http://hz.hnxiangtu.top/gtrneqrzkt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yongpay.top/gtsrcrcnqj.html

[Q11] 一次插入多行
来源：http://hz.xylfe.cn/gtmjgrdybb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuanzx.com/gtchmirllv.html

[Q12] 插入后取自增 ID
来源：http://hz.yj202588.top/gtgpixbrqd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sufxvd.cn/gtnnqokwtd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhengqikj.top/gtxcpijbay.html

[Q13] 忽略重复插入
来源：http://hz.tanke756.top/gtoslovdjm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gtseagawnj.html

[Q14] 存在则更新（upsert）
来源：http://hz.cdnleiting.top/gttgmhyzqe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gtpgdsjptb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.bjfxy.top/gtfbykxsdr.html

[Q15] 查询全部
来源：http://hz.wangdashe.top/gtmsjljdpq.html

SELECT * FROM users;
来源：http://hz.zhaomingkeji.xyz/gtositntlr.html

[Q16] 查询指定列
来源：http://hz.wangdashe.top/gtmqbjeqic.html

SELECT id, name FROM users;
来源：http://hz.0kj1m.cn/gtiksuydfb.html

[Q17] 条件查询
来源：http://hz.daxiang520.top/gttlhixufj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtqmazzypi.html

[Q18] 模糊匹配
来源：http://hz.hfpthk.cn/gtwlkbelbf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.meibo888.top/gtnxwkswdo.html

[Q19] 范围查询
来源：http://hz.yj20258888.top/gtckevfyvx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.havefunace.top/gtkorucyyd.html

[Q20] IN 列表
来源：http://hz.yj20258.top/gtbiqawoja.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jianghu66.top/gtijlujqbp.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtyjucxwxv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinqigufen.top/gtjeshqkof.html

[Q22] 排序
来源：http://hz.smart0.xyz/gtakuiscjd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cucudq.cn/gtosvwdrpf.html

[Q23] 分页
来源：http://hz.316326.xyz/gtbpissflq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.fzhhl.top/gtmoplfyow.html

[Q24] 去重
来源：http://hz.sweek.top/gtgvqcpwuw.html

SELECT DISTINCT city FROM users;
来源：http://hz.0kj1m.cn/gtxckcjuha.html

[Q25] 只取前 N 条
来源：http://hz.ivvv.top/gtcqckciok.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gtzkftrwlh.html

[Q26] 计数
来源：http://hz.yonumen.top/gtbzbvmrqu.html

SELECT COUNT(*) FROM users;
来源：http://hz.cucudq.cn/gtyqppjnof.html

[Q27] 条件计数
来源：http://hz.smart0.xyz/gtssvbfbjs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tianlin.xyz/gtoqswdpdr.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtanzedvja.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtfcpjpmmr.html

[Q29] 最大最小值
来源：http://hz.xuanzx.com/gtkhjdvkgc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gtjuayyhmp.html

[Q30] 分组统计
来源：http://hz.0kj1m.cn/gtdudpcgqo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtnbnmxgfv.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtecwcknfh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jlsjyb.cn/gtjgvqqngv.html

[Q32] 分组拼接字符串
来源：http://hz.daxiang520.top/gtaqctwqmf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtlnorkdvk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigufen.top/gtlnpjuzgs.html

[Q33] 多列分组
来源：http://hz.feifeiyinyue.top/gtglbacymd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.meibo888.top/gtfntdaxvb.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtcjrarttn.html

SELECT * FROM (
来源：http://hz.jinqigfzy.top/gtmsnbazzg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dianchejie.cn/gtcggtfoeq.html

) t WHERE rn = 1;
来源：http://hz.sysykeji.top/gtmnxskxix.html

[Q35] 内连接
来源：http://hz.nanxuanxn.top/gthdblfssp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cqqwz.cn/gtwxlguxyd.html

[Q36] 左连接
来源：http://hz.dashuyun.cn/gtebzmjpie.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtwdpbegvb.html

[Q37] 右连接
来源：http://hz.ehwqpu.com/gtkrfrcajp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gtfnqkzlah.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangshuangyany.cn/gtzhgdplnv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydzc1.top/gtpzjfhxam.html

[Q39] 自连接（查上下级）
来源：http://hz.gogol.net.cn/gtetpfauhw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydjk.org.cn/gtykqyxxoo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.birdmap.top/gtoznsmhdj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtwqvoqjxt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fzhhl.top/gtsfpdmhsm.html

[Q41] 多表连接
来源：http://hz.cheryme.top/gtgwhjrhjc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cucudq.cn/gtcmxigsnd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hammf.cn/gtxuofsbqj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daxiang520.top/gtbijynlgi.html

[Q42] 连接条件附加过滤
来源：http://hz.gaohongyu789.top/gtxktaodkr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnqzz.top/gtuibfpllo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daxiang520.top/gtfouhhsdv.html

[Q43] 标量子查询
来源：http://hz.zhoulong.xyz/gtiwjhhbid.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gtfcqciexf.html

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtonrpaxkk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fengsongda.top/gtkehtfeir.html

[Q45] EXISTS 判断存在
来源：http://hz.316326.xyz/gtbqyonsww.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtaromnwuj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fzhhl.top/gtpwwdqnox.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtnlwmvisq.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangkeji.top/gtruwxfpow.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ybcxt.top/gtyogafmkq.html

[Q48] CTE 公用表表达式
来源：http://hz.yonumen.top/gtqmyyrcws.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.0kj1m.cn/gtdvzkhnpr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aizwys.cn/gtmmkpqqoi.html

[Q49] 更新单行
来源：http://hz.fzhhl.top/gtivlcfkav.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yongpay.top/gtaffxyiuc.html

[Q50] 批量更新
来源：http://hz.ivvv.top/gtugnhjugt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.havefunace.top/gtsorqndha.html

[Q51] 用子查询更新
来源：http://hz.yj202588.top/gtobfmjhyy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cashguo.top/gtnropgfox.html

[Q52] 删除指定行
来源：http://hz.kuanghao11.cn/gtaagzpijp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ehwqpu.com/gtlmwplfdm.html

[Q53] 按条件删除
来源：http://hz.cdnleiting.top/gtetdbouwu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.vqdsnc.cn/gtsjzxxhmv.html

[Q54] 清空表
来源：http://hz.hnxiangtu.top/gtoypxfius.html

TRUNCATE TABLE logs;
来源：http://hz.zhijiandao.cn/gtzkpdmmbr.html

[Q55] 排名（并列占位）
来源：http://hz.redwolf501.top/gtfjasxrgt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yvedp.cn/gtlwzhelhb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cashguo.top/gtmwvwoqlk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.andypj.xyz/gtkciuroxw.html

[Q57] 行号
来源：http://hz.xuanzx.com/gthhztnvit.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.quarkkingdee.top/gttggogfon.html

[Q58] 累计求和
来源：http://hz.xuanzx.com/gtphvabzbm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daxiang520.top/gtazsretff.html

[Q59] 分组内累计
来源：http://hz.zhengqikj.top/gtlyirqgdc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gotoacloud.top/gtlmcnxhqx.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenjidiqi.icu/gtlwrcgvds.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.snrcjt.cn/gtgzpxiauf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnxiangtu.top/gtnurldsfa.html

[Q61] 移动平均
来源：http://hz.yonumen.top/gtpdhcfnrp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtpqhrnuww.html

[Q62] 分组占比
来源：http://hz.yangfankeji.com/gtofcwfvno.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtwszhtcbw.html

[Q63] 开启事务
来源：http://hz.zycfv.cn/gtcfknracn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xingfuxueyuan.xyz/gtdhtvyjto.html

[Q64] 提交事务
来源：http://hz.nanxuanxn.top/gtmlaptslq.html

COMMIT;
来源：http://hz.shzxlz.cn/gtozqxjobu.html

[Q65] 回滚事务
来源：http://hz.sufxvd.cn/gtdinefzcl.html

ROLLBACK;
来源：http://hz.cashguo.top/gtwsifohhf.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangtech.top/gtqjhtwupc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hammf.cn/gtukgpgtcv.html

[Q67] 设置隔离级别
来源：http://hz.jyoumei.cn/gtjajijbmw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258888.top/gtuyhcrpld.html

[Q68] 保存点
来源：http://hz.pengpengdd.cyou/gtqddgwwfe.html

SAVEPOINT sp1;
来源：http://hz.yuanzhike.top/gtwhyyaafe.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtatpzbeef.html

[Q69] 查看执行计划
来源：http://hz.bjfxy.top/gtbmboltuq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yongpay.top/gtbvjgqzeo.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gttbqpfkxw.html

ANALYZE TABLE users;
来源：http://hz.xylfe.cn/gtfucbshhy.html

[Q71] 查看建表语句
来源：http://hz.hammf.cn/gtoxpaupsr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sufxvd.cn/gtkulifawp.html

[Q72] 查看索引
来源：http://hz.sufxvd.cn/gtzuyxfmsv.html

SHOW INDEX FROM users;
来源：http://hz.chenjidiqi.icu/gtanmhmlyx.html

[Q73] 查看表状态
来源：http://hz.hywenlv.cn/gtymltnksz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtvvvmsuxs.html

[Q74] 强制使用索引
来源：http://hz.yj20258.top/gthpiboreq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hysaishi.cn/gtwhpvppjo.html

[Q75] 日期格式化
来源：http://hz.havefunace.top/gtqmjltaor.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangdashe.top/gtwcvfmilq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cashguo.top/gtsiqrmzmg.html

[Q76] 按天统计
来源：http://hz.jiagoushi.top/gtixibovdi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yvedp.cn/gtvmsdhamy.html

[Q77] 时间加减
来源：http://hz.cheryme.top/gtbruxptmx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtvtrpmmrz.html

[Q78] 当前时间
来源：http://hz.zhiwuduotai.top/gtzrhkdejc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ywan-chungtsiang.top/gtrozwzviq.html

[Q79] 字符串拼接
来源：http://hz.xuetiantiany.cn/gtcsfdpyzd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258.top/gtdprgfpla.html

[Q80] 字符串截取
来源：http://hz.9152youxi.cn/gtkyxzsyxq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ppjwa.cn/gtxwvsfxol.html

[Q81] 字符串替换
来源：http://hz.wangdashe.top/gtenbkdweb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gtmdrcgngc.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gthqfipenl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuxming.cn/gtqkkssxji.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtobjfypax.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258.top/gtrxhlqaod.html

[Q84] 去除首尾空格
来源：http://hz.pengpengdd.cyou/gtiektwvxr.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtlchgrkws.html

[Q85] 数值取整
来源：http://hz.hfpthk.cn/gtisywtqgd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gtuitfjhcj.html

[Q86] 读取 JSON 字段
来源：http://hz.zhoulong.xyz/gtkevcifks.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yongpay.top/gttblvjnyo.html

[Q87] JSON 字段做条件
来源：http://hz.haohaochexian.top/gtqrzkqjvc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtikwhxuyj.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigufen.top/gtwibcvgpj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.0kj1m.cn/gtccxhlepw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj202588.top/gtbuwekaqg.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtxaenelto.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtqpjzmorq.html

[Q90] 生成序号列
来源：http://hz.jinyuanbaomall.cn/gtkngfoybm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shuidangran.top/gtwnlsbjjy.html

================================================================================
来源：http://hz.cashguo.top/gtfefwbswy.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtzmwxafiq.html

================================================================================
来源：http://hz.tanke756.top/gtappuuobl.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gtunukltus.html

#!/usr/bin/env bash
来源：http://hz.yuanzhike.top/gtcdseqphe.html

set -euo pipefail
来源：http://hz.yuxming.cn/gtcpnpeukn.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangtech.top/gtnjlqfiep.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gtwpxndibj.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtxtrtisdr.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtbpgjtvra.html

[R04] 位置参数
来源：http://hz.yongpay.top/gtquqhlqgx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sweek.top/gtyxcrkcra.html

[R05] 参数默认值
来源：http://hz.gogol.net.cn/gtjonsjhxr.html

name="${1:-default}"
来源：http://hz.zhongyouzk.top/gtxnwwlwsh.html

[R06] 判断命令是否存在
来源：http://hz.ppjwa.cn/gttewfdmmy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fengsongda.top/gtmmgxnyvw.html

[R07] if 判断文件
来源：http://hz.bjfxy.top/gtgiprfhvs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xziqi.cn/gtapbislrp.html

[R08] 数值比较
来源：http://hz.jinqigufen.top/gtxfgqivzv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gtxheylbpn.html

[R09] 字符串比较
来源：http://hz.zhengqikj.top/gttckpnusr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ivvv.top/gtwdmnztmx.html

[R10] 正则匹配
来源：http://hz.yueranfly.top/gtcquzhfxb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dianchejie.cn/gtcaqedvus.html

[R11] case 多分支
来源：http://hz.guannengcc.top/gtstliykls.html

case "$1" in
来源：http://hz.snrcjt.cn/gtwhemocai.html

start) echo "启动" ;;
来源：http://hz.zdqjudy.top/gtmzyxmcoq.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtigrjpatb.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigfzy.top/gtytnxicqy.html

esac
来源：http://hz.jiagoushi.top/gtzzmikplm.html

[R12] for 遍历文件
来源：http://hz.jinqigfzy.top/gtjfhdsjbf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yvedp.cn/gtlgtaufwb.html

[R13] for 计数循环
来源：http://hz.redwolf501.top/gthlisquzj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.daria6918.cn/gtdjkqakev.html

[R14] C 风格 for
来源：http://hz.zhongyouzk.top/gtcgopjmad.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dashuyun.cn/gtqzkblnvy.html

[R15] while 逐行读文件
来源：http://hz.cheryme.top/gtmtpgamqg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.vqdsnc.cn/gtzgvsghcv.html

[R16] until 等待条件
来源：http://hz.jinqigufen.top/gtnnzmjsck.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hnxiangtu.top/gtfccowruo.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtbxzxqlfl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhaomingkeji.xyz/gttvbghiss.html

[R18] 遍历数组
来源：http://hz.snrcjt.cn/gtpdwocyvx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtygvldmkt.html

[R19] 数组长度
来源：http://hz.ehwqpu.com/gtxjiqddjd.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtahcmsehq.html

[R20] 关联数组（字典）
来源：http://hz.mhx1999.top/gteuqfmtzr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuanzx.com/gtwfovpmpi.html

[R21] 字符串长度
来源：http://hz.ybcxt.top/gttozzwxvc.html

echo "${#s}"
来源：http://hz.shanyushiyangkeji.top/gtxtbzjrhs.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtactvimtd.html

echo "${s:0:5}"
来源：http://hz.gotoacloud.top/gtwmefujpc.html

[R23] 字符串替换
来源：http://hz.jinqigfzy.top/gtbkmfphxt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj202588.top/gtcexhjqpr.html

[R24] 大小写转换
来源：http://hz.smart0.xyz/gtabhaxfre.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nwbrower.top/gtqbbnhaua.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj202588.top/gtufizmeda.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hammf.cn/gtcbikimxg.html

[R26] 命令替换
来源：http://hz.cashguo.top/gtkighdpoa.html

now=$(date +%F); echo "$now"
来源：http://hz.yanxiufei.cn/gtyqlonnph.html

[R27] 算术展开
来源：http://hz.wangshuangyany.cn/gtksvsrogm.html

echo $((1 + 2 * 3))
来源：http://hz.xuetiantiany.cn/gtacsaiupu.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gtgnhxrmbz.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenzaomai.com/gtbymutfmb.html

[R29] 定义函数
来源：http://hz.yj202588.top/gtvdfeczqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zdqjudy.top/gtrmhhbraa.html

[R30] 函数返回状态码
来源：http://hz.sufxvd.cn/gtddxdrbxm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daxiang520.top/gtwtkfzkbt.html

[R31] 局部变量
来源：http://hz.zhiwuduotai.top/gtkubrddxy.html

f() { local x=1; echo "$x"; }
来源：http://hz.gotoacloud.top/gtbvqyvngn.html

[R32] 参数个数校验
来源：http://hz.yuxming.cn/gtwkajjfjb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gthqccowgo.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gtfikjvawg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.bjfxy.top/gtgyotlcnb.html

[R34] 退出时清理
来源：http://hz.xuanzx.com/gtxfucopqc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtssnhypdc.html

[R35] 后台执行并等待
来源：http://hz.316326.xyz/gtjatuyozc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258.top/gtxpxwwpxn.html

[R36] 并发执行多个任务
来源：http://hz.jinghuilouyu.cn/gtmpjafaqh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhoulong.xyz/gtkqlkptuy.html

[R37] 把输出赋给变量
来源：http://hz.hfpthk.cn/gtbgldcctw.html

files=$(ls -1)
来源：http://hz.xziqi.cn/gtfihwskyz.html

[R38] 管道串联
来源：http://hz.ivvv.top/gtbwrasavs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cqqwz.cn/gtcbzyqckn.html

[R39] 重定向标准输出与错误
来源：http://hz.52xcode.cn/gtryloaeyj.html

cmd > out.log 2>&1
来源：http://hz.0kj1m.cn/gtsdfqxawo.html

[R40] 追加写日志
来源：http://hz.quarkkingdee.top/gtqvkbtggm.html

echo "log" >> out.log
来源：http://hz.zhongyouzk.top/gtmzttkucj.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gtbkikmhve.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtvhmgehnp.html

[R42] 输入重定向
来源：http://hz.yvedp.cn/gtexpkgkqr.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtvyxxuqkx.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtyykdhpmc.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtarfjtarn.html

[R44] 按修改时间查找
来源：http://hz.jinyuanbaomall.cn/gtayuwgnxm.html

find . -mtime -7 -type f
来源：http://hz.zhixingplan.top/gtcddnsbpp.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtnubmdwmd.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtmfcwcszm.html

[R46] 递归替换文件内容
来源：http://hz.zhengqikj.top/gtxugjfneu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pengpengdd.cyou/gtlzgmyxco.html

[R47] sed 单行替换
来源：http://hz.sxryk.cn/gtaceojlvo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.feifeiyinyue.top/gtwxhgebjt.html

[R48] awk 取指定列
来源：http://hz.hfpthk.cn/gtrnccbjga.html

awk '{print $1, $3}' a.txt
来源：http://hz.dashuyun.cn/gtfnuuzxgn.html

[R49] awk 带条件
来源：http://hz.c1oappe.top/gtgfwunnqm.html


<!-- 参考信息 -->