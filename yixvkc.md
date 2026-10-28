代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtxjiziuex.html

user_id INT NOT NULL,
来源：http://hz.yuxming.cn/gtlbolhmgi.html

amount DECIMAL(10, 2),
来源：http://hz.nanxinkj.top/gtsccjhosg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.daxiang520.top/gtgwozghtx.html

);
来源：http://hz.jinqigfzy.top/gtnergldor.html

[Q03] 增加列
来源：http://hz.c1oappe.top/gtbqrzcyuu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtzberfeko.html

[Q04] 修改列类型
来源：http://hz.cqqwz.cn/gtspszjpsn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ybcxt.top/gtxyikiewp.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtoandjzrb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hywenlv.cn/gtiuobcoxh.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtinqrayun.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj202588.top/gtczwurtno.html

[Q07] 删除表
来源：http://hz.gotoacloud.top/gtikzkbqdm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hfpthk.cn/gtkqrtragi.html

[Q08] 创建普通索引
来源：http://hz.shangyingyoupin.top/gtomclogze.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenlongwang.top/gtsaiosdet.html

[Q09] 创建唯一索引
来源：http://hz.birdmap.top/gtyrqpvaey.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tian-w.cn/gtyuzewngp.html

[Q10] 插入单行
来源：http://hz.mhx1999.top/gtrxzuxgkx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yonumen.top/gtjmrucygx.html

[Q11] 一次插入多行
来源：http://hz.andypj.xyz/gtrbkwmins.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tian-w.cn/gtkjsdnlwa.html

[Q12] 插入后取自增 ID
来源：http://hz.ywan-chungtsiang.top/gtpmryzilq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhaomingkeji.xyz/gteinnasuh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj202588.top/gtvduyoylr.html

[Q13] 忽略重复插入
来源：http://hz.ydzc1.top/gttdwjmuku.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuanzhike.top/gtlpkpmphu.html

[Q14] 存在则更新（upsert）
来源：http://hz.sufxvd.cn/gtrbtavzdb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ehwqpu.com/gtbfeivlfr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gthrjpdzfu.html

[Q15] 查询全部
来源：http://hz.vqdsnc.cn/gtyimuomnt.html

SELECT * FROM users;
来源：http://hz.fengsongda.top/gtawfmhwlm.html

[Q16] 查询指定列
来源：http://hz.meibo888.top/gtpeuowrzn.html

SELECT id, name FROM users;
来源：http://hz.gzhubu.top/gtaqtjvarq.html

[Q17] 条件查询
来源：http://hz.jqgufenzy.top/gtscqgxqah.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.pengpengdd.cyou/gtyttftywf.html

[Q18] 模糊匹配
来源：http://hz.bjfxy.top/gtioilduzp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jianghu66.top/gtfgxgfxya.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gtfkxnjzzu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yongpay.top/gtvfxfmmjm.html

[Q20] IN 列表
来源：http://hz.zhongyouzk.top/gtfnzkprfg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtapdakrwa.html

[Q21] 空值判断
来源：http://hz.zycfv.cn/gtmcvxpgyn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hnqzz.top/gtzebtotfm.html

[Q22] 排序
来源：http://hz.sxryk.cn/gtglaswvtp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fzhhl.top/gtabrcboah.html

[Q23] 分页
来源：http://hz.shzxlz.cn/gtljrbitus.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gzhubu.top/gteixrzilx.html

[Q24] 去重
来源：http://hz.hammf.cn/gtbclpwxdv.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258.top/gtgskkwpzc.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtkvxuvyhx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangtech.top/gtnnqazkky.html

[Q26] 计数
来源：http://hz.yanxiufei.cn/gtkkslgqgt.html

SELECT COUNT(*) FROM users;
来源：http://hz.hammf.cn/gtccleefjg.html

[Q27] 条件计数
来源：http://hz.zdqjudy.top/gtyennegva.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxuanxn.top/gtmbvhreds.html

[Q28] 求和与平均
来源：http://hz.shzxlz.cn/gtoxggvktw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtobryjncz.html

[Q29] 最大最小值
来源：http://hz.yanxiufei.cn/gtsysnuosj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pycfn.com/gtmkfahdmk.html

[Q30] 分组统计
来源：http://hz.yj20258.top/gtatrbytoo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtouhnbvmz.html

[Q31] 分组后过滤
来源：http://hz.jinghuilouyu.cn/gttniysqjc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtubqahryh.html

[Q32] 分组拼接字符串
来源：http://hz.tian-w.cn/gtiacrkxxl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtplplrohf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.andypj.xyz/gtxzwmbamo.html

[Q33] 多列分组
来源：http://hz.hnxiangtu.top/gtcysghnql.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xziqi.cn/gtbgutrsqi.html

[Q34] 每组取第一条
来源：http://hz.yonumen.top/gtixbyrveg.html

SELECT * FROM (
来源：http://hz.zycfv.cn/gtbyfiufbb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgfzy.top/gtovgfqbxt.html

) t WHERE rn = 1;
来源：http://hz.aibaodan.cn/gtcslayose.html

[Q35] 内连接
来源：http://hz.yanxiufei.cn/gtnwweeqtw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtrueumwwy.html

[Q36] 左连接
来源：http://hz.meibo888.top/gtzbxglzba.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtyhzqxnhz.html

[Q37] 右连接
来源：http://hz.xuanzx.com/gtpfokmqzh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xingfuxueyuan.xyz/gtxwojzvtl.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xuetiantiany.cn/gtcljtpusu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gtujvfsvgg.html

[Q39] 自连接（查上下级）
来源：http://hz.sufxvd.cn/gtnezjesof.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtcthyljfe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yangfankeji.com/gtdfsfxvsa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.pycfn.com/gtvxzitqgf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gthefpiyxi.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtblhlbanm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtherdmajx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtqejrxsjs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.0kj1m.cn/gtapabolrk.html

[Q42] 连接条件附加过滤
来源：http://hz.vqdsnc.cn/gtzttgfjhy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cucudq.cn/gtfdjwnnje.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sufxvd.cn/gtremkguet.html

[Q43] 标量子查询
来源：http://hz.yanxiufei.cn/gtdfewqlae.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gogol.net.cn/gtkwwymvwb.html

[Q44] IN 子查询
来源：http://hz.feifeiyinyue.top/gttdhkuonm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yangfankeji.com/gtxjtbadjt.html

[Q45] EXISTS 判断存在
来源：http://hz.zhaomingkeji.xyz/gtvzzsgeed.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydzc1.top/gtqfnysiwy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dashuyun.cn/gtxwrgbfsu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gtgiukvign.html

[Q47] 与平均值比较
来源：http://hz.yueranfly.top/gtrpxxaczt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.meibo888.top/gtrtrismfz.html

[Q48] CTE 公用表表达式
来源：http://hz.aibaodan.cn/gtyoxgrgba.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinghuilouyu.cn/gtptemzwhi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gttuwbxfjp.html

[Q49] 更新单行
来源：http://hz.jinghuilouyu.cn/gtdatadsdi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.quarkkingdee.top/gtdynjloua.html

[Q50] 批量更新
来源：http://hz.sysykeji.top/gtiutodulr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yuxming.cn/gttdsfgsfl.html

[Q51] 用子查询更新
来源：http://hz.gzhubu.top/gtvauicirj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenzaomai.com/gtcdyyfbul.html

[Q52] 删除指定行
来源：http://hz.zhengqikj.top/gtycyjumum.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daria6918.cn/gtageozogp.html

[Q53] 按条件删除
来源：http://hz.ywan-chungtsiang.top/gtdniautux.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sufxvd.cn/gtumetudec.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtfvfsknpn.html

TRUNCATE TABLE logs;
来源：http://hz.ppjwa.cn/gtcocmjynf.html

[Q55] 排名（并列占位）
来源：http://hz.nanxinkj.top/gtnkaaehqf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gtspzirdlq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xingfuxueyuan.xyz/gtbuuipomv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.svipenyu.cn/gtptgrwgri.html

[Q57] 行号
来源：http://hz.jlsjyb.cn/gtxxjibpfo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sysykeji.top/gtnkfmgvav.html

[Q58] 累计求和
来源：http://hz.aizwys.cn/gtsfokrfcy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgfzy.top/gtffqgapnv.html

[Q59] 分组内累计
来源：http://hz.nanxinkj.top/gtciqkwbfa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gtoldluvcc.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtlfpgbosf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yueranfly.top/gtoaafatys.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yongpay.top/gttahjqaao.html

[Q61] 移动平均
来源：http://hz.yuxming.cn/gtpudlmmgo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yvedp.cn/gtiyhpnlgj.html

[Q62] 分组占比
来源：http://hz.guannengcc.top/gtptxgcjnn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtzglbotvv.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gttsyqsuup.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenzaomai.com/gtykrjchxm.html

[Q64] 提交事务
来源：http://hz.zhengqikj.top/gtllauenjs.html

COMMIT;
来源：http://hz.ywan-chungtsiang.top/gtzlzgnoqh.html

[Q65] 回滚事务
来源：http://hz.jiagoushi.top/gtjytedbli.html

ROLLBACK;
来源：http://hz.9152youxi.cn/gtfcrvxpff.html

[Q66] 行锁查询
来源：http://hz.hysaishi.cn/gtmpjcyhky.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangdashe.top/gttjzscojv.html

[Q67] 设置隔离级别
来源：http://hz.yuxming.cn/gtxzlvkcnl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.316326.xyz/gtkxvtlqyl.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtgmzjccyi.html

SAVEPOINT sp1;
来源：http://hz.shuidangran.top/gtuxgksdfg.html

ROLLBACK TO sp1;
来源：http://hz.tian-w.cn/gtrwntnjnf.html

[Q69] 查看执行计划
来源：http://hz.smart0.xyz/gtocgnynyg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gtckibminv.html

[Q70] 更新统计信息
来源：http://hz.wangdashe.top/gtndmtnrcs.html

ANALYZE TABLE users;
来源：http://hz.hnqzz.top/gtstoospwf.html

[Q71] 查看建表语句
来源：http://hz.havefunace.top/gtqljnsdcc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gtqeiftocn.html

[Q72] 查看索引
来源：http://hz.jinghuilouyu.cn/gtklkcxxvi.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtgalhvzyo.html

[Q73] 查看表状态
来源：http://hz.chenlongwang.top/gtnyvmdveu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtqfkjiuoe.html

[Q74] 强制使用索引
来源：http://hz.ppjwa.cn/gthzlitgro.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shanyushiyangkeji.top/gtanfvezxo.html

[Q75] 日期格式化
来源：http://hz.mhx1999.top/gtmwosogec.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuanzx.com/gtwhlvuxfv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinqigfzy.top/gtziobatll.html

[Q76] 按天统计
来源：http://hz.daxiang520.top/gtjitpinad.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gaohongyu789.top/gtyfwnoqrk.html

[Q77] 时间加减
来源：http://hz.haohaochexian.top/gtvoxemhzs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gtpuyuylbh.html

[Q78] 当前时间
来源：http://hz.yangfankeji.com/gtuvnavory.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhengqikj.top/gtpzgmjyvd.html

[Q79] 字符串拼接
来源：http://hz.ywan-chungtsiang.top/gtvtbqezin.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.smart0.xyz/gtoczjtryr.html

[Q80] 字符串截取
来源：http://hz.andypj.xyz/gtmqeiglkq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aibaodan.cn/gttegigicu.html

[Q81] 字符串替换
来源：http://hz.ehwqpu.com/gtackbqhyz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gotoacloud.top/gtzqahqhem.html

[Q82] 字符长度与字节长度
来源：http://hz.xinyue.icu/gtoclragbk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guowangkeji.top/gtgzoirrjw.html

[Q83] 大小写转换
来源：http://hz.zhengqikj.top/gttmxjehwh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhoulong.xyz/gtnzfebfei.html

[Q84] 去除首尾空格
来源：http://hz.hysaishi.cn/gtllaipzcl.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258888.top/gtjhbdjata.html

[Q85] 数值取整
来源：http://hz.yj20258888.top/gtcedwhjuw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.smart0.xyz/gtvbiqvyvf.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtbunujoea.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xingfuxueyuan.xyz/gtoudndwes.html

[Q87] JSON 字段做条件
来源：http://hz.zhiwuduotai.top/gtrjibwtvb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sysykeji.top/gtlwbvvrxv.html

[Q88] 行转列（条件聚合）
来源：http://hz.cashguo.top/gtqnouovxc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtlpjgcjvi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.andypj.xyz/gtjzryfvmc.html

[Q89] 判断表是否存在
来源：http://hz.birdmap.top/gtogzpgjqj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hywenlv.cn/gtyydhtbcf.html

[Q90] 生成序号列
来源：http://hz.dianchejie.cn/gtcbhzplbj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.316326.xyz/gtcpogbvzm.html

================================================================================
来源：http://hz.andypj.xyz/gtsvwrtbqj.html

R. Bash 专题
来源：http://hz.meibo888.top/gtevvxkmxl.html

================================================================================
来源：http://hz.chenzaomai.com/gtzcchgigb.html

[R01] shebang 与严格模式
来源：http://hz.yanxiufei.cn/gtvvaqhlwd.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtnpcyuzsw.html

set -euo pipefail
来源：http://hz.52xcode.cn/gthmnyadki.html

[R02] 变量赋值与使用
来源：http://hz.smart0.xyz/gtleeyfaea.html

name="Tom"; echo "$name"
来源：http://hz.gaohongyu789.top/gtqeioappo.html

[R03] 只读变量
来源：http://hz.haohaochexian.top/gtnvswovvf.html

readonly PI=3.14
来源：http://hz.zhijiandao.cn/gtkacfbclk.html

[R04] 位置参数
来源：http://hz.zhoulong.xyz/gtsclxeyij.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhongyouzk.top/gtgcusfsgp.html

[R05] 参数默认值
来源：http://hz.pengpengdd.cyou/gtrfgbrnbq.html

name="${1:-default}"
来源：http://hz.jlsjyb.cn/gteqyigehn.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gtqanuoktr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gtdayjpjcc.html

[R07] if 判断文件
来源：http://hz.zhongyouzk.top/gtqxeriyny.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gtspdrehzf.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtzsulzgss.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinghuilouyu.cn/gtrttahotv.html

[R09] 字符串比较
来源：http://hz.yueranfly.top/gtsoxrckfl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenzaomai.com/gtxympcios.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtcrisvout.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.andypj.xyz/gtehfjiuqd.html

[R11] case 多分支
来源：http://hz.zhixingplan.top/gtulehtlwo.html

case "$1" in
来源：http://hz.sufxvd.cn/gtdvnpfqik.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtdhuayxpm.html

stop)  echo "停止" ;;
来源：http://hz.gzhubu.top/gtjbkagaua.html

*)     echo "未知命令" ;;
来源：http://hz.gzhubu.top/gtvndmzvjz.html

esac
来源：http://hz.jyoumei.cn/gtdcxsqwud.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtxbnwwdja.html

for f in *.txt; do echo "$f"; done
来源：http://hz.vqdsnc.cn/gtduywaoui.html

[R13] for 计数循环
来源：http://hz.zdqjudy.top/gtmgjgiiya.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yongpay.top/gtdfvxjvrz.html

[R14] C 风格 for
来源：http://hz.zycfv.cn/gtsuahbepf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ehwqpu.com/gtokwdmdph.html

[R15] while 逐行读文件
来源：http://hz.hnxiangtu.top/gtgynahnts.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydzc1.top/gtanhxivrt.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gtyedehplp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zycfv.cn/gtvqggrsro.html

[R17] 数组定义与取值
来源：http://hz.hnxiangtu.top/gttvsibqcj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.mhx1999.top/gtsufedsrx.html

[R18] 遍历数组
来源：http://hz.yvedp.cn/gtpvhihynt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ehwqpu.com/gttcaqnixq.html

[R19] 数组长度
来源：http://hz.pengpengdd.cyou/gtbcbqjuyr.html

echo "${#arr[@]}"
来源：http://hz.quarkkingdee.top/gtewrnmqon.html

[R20] 关联数组（字典）
来源：http://hz.daria6918.cn/gtkoxpaalm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ppjwa.cn/gtxambnset.html

[R21] 字符串长度
来源：http://hz.316326.xyz/gtmrkiwobn.html

echo "${#s}"
来源：http://hz.fzhhl.top/gtcsuqgabb.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtosvqvjgg.html

echo "${s:0:5}"
来源：http://hz.dianchejie.cn/gtlkxdyues.html

[R23] 字符串替换
来源：http://hz.xinyue.icu/gtaesqtczn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.meibo888.top/gtyjxoauqq.html

[R24] 大小写转换
来源：http://hz.tianlin.xyz/gtknwphtme.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nwbrower.top/gtvxapnvcw.html

[R25] 去后缀 / 去前缀
来源：http://hz.dashuyun.cn/gtcubsydxu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtijpdzfde.html

[R26] 命令替换
来源：http://hz.dashuyun.cn/gtxpdgqiok.html

now=$(date +%F); echo "$now"
来源：http://hz.gogol.net.cn/gtxdyagbbw.html

[R27] 算术展开
来源：http://hz.yj20258.top/gtnkhxipuv.html

echo $((1 + 2 * 3))
来源：http://hz.svipenyu.cn/gtuiegtibp.html

[R28] 浮点运算
来源：http://hz.yj202588.top/gtbsuqwpqy.html

echo "scale=2; 10/3" | bc
来源：http://hz.wangdashe.top/gtjzeagrjo.html

[R29] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtdffaudpo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xylfe.cn/gtmgdnswos.html

[R30] 函数返回状态码
来源：http://hz.yvedp.cn/gteiplcveo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258888.top/gtobogcnlk.html

[R31] 局部变量
来源：http://hz.yj202588.top/gtiqryzxdd.html

f() { local x=1; echo "$x"; }
来源：http://hz.kuanghao11.cn/gtatnyecbr.html

[R32] 参数个数校验
来源：http://hz.sxryk.cn/gtlkkwkggb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ybcxt.top/gtkjjrbrxu.html

[R33] 捕获错误并提示行号
来源：http://hz.tian-w.cn/gtdenqfdoj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtwkamvpll.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtesnjcwqo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtovjitqut.html

[R35] 后台执行并等待
来源：http://hz.mhx1999.top/gtekzviwlt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj202588.top/gtlxbglfgd.html

[R36] 并发执行多个任务
来源：http://hz.0kj1m.cn/gtczpxxavz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhoulong.xyz/gtyxagkprc.html

[R37] 把输出赋给变量
来源：http://hz.iojbl.cn/gtsuvfspyf.html

files=$(ls -1)
来源：http://hz.jianghu66.top/gtueaeppco.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtqneymudz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aizwys.cn/gtblseeych.html

[R39] 重定向标准输出与错误
来源：http://hz.smart0.xyz/gtgsboafwx.html

cmd > out.log 2>&1
来源：http://hz.jlsjyb.cn/gtyoqzaped.html

[R40] 追加写日志
来源：http://hz.smart0.xyz/gtcrjodpsu.html

echo "log" >> out.log
来源：http://hz.birdmap.top/gtoihlhmuy.html

[R41] 丢弃输出
来源：http://hz.hfpthk.cn/gtywsxvrvb.html

cmd >/dev/null 2>&1
来源：http://hz.yongpay.top/gtymasrwsx.html

[R42] 输入重定向
来源：http://hz.52xcode.cn/gtfjfyonil.html

wc -l < a.txt
来源：http://hz.feifeiyinyue.top/gtdeyqwghv.html

[R43] 按名字查找文件
来源：http://hz.gzhubu.top/gtjyibqgmy.html

find . -name "*.log" -type f
来源：http://hz.havefunace.top/gtkppjoqsp.html

[R44] 按修改时间查找
来源：http://hz.jinyuanbaomall.cn/gtwjscbizo.html

find . -mtime -7 -type f
来源：http://hz.yj20258.top/gtvloydofa.html

[R45] 批量删除
来源：http://hz.yvedp.cn/gtkdrsmzqa.html

find . -name "*.tmp" -delete
来源：http://hz.gzhubu.top/gtaqxqclrs.html

[R46] 递归替换文件内容
来源：http://hz.ehwqpu.com/gtmfuwzlhz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuanzx.com/gtkqukdsds.html

[R47] sed 单行替换
来源：http://hz.zhaomingkeji.xyz/gtxjdaxpxt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ivvv.top/gtwjdmepch.html

[R48] awk 取指定列
来源：http://hz.fzhhl.top/gtrehyrmri.html

awk '{print $1, $3}' a.txt
来源：http://hz.daria6918.cn/gttahpvunk.html

[R49] awk 带条件
来源：http://hz.0kj1m.cn/gtpsynscwh.html


<!-- 参考信息 -->