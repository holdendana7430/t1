代发 wailian999

);
来源：http://hz.hongshengwenyu.top/gtimkaeqge.html

[Q03] 增加列
来源：http://hz.chenlongwang.top/gtqvnsnkkq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zycfv.cn/gtgesuikkf.html

[Q04] 修改列类型
来源：http://hz.zycfv.cn/gtdkjllhoi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shanyushiyangkeji.top/gtwkdijnsx.html

[Q05] 重命名列
来源：http://hz.snrcjt.cn/gtnzjgltce.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuanzhike.top/gtznkboklc.html

[Q06] 删除列
来源：http://hz.mhx1999.top/gtpyliogjp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gtwttcfvnf.html

[Q07] 删除表
来源：http://hz.jianghu66.top/gtkfumnwcl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.andypj.xyz/gtazitmawo.html

[Q08] 创建普通索引
来源：http://hz.cdnleiting.top/gtokmxddzh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtvoljafrp.html

[Q09] 创建唯一索引
来源：http://hz.nwbrower.top/gtnnromfru.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gzhubu.top/gtcnrzizqf.html

[Q10] 插入单行
来源：http://hz.zhengqikj.top/gtomtblwfu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenlongwang.top/gtwwdnlcsn.html

[Q11] 一次插入多行
来源：http://hz.nanxinkj.top/gttmxkouxe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xziqi.cn/gtmzvszpyf.html

[Q12] 插入后取自增 ID
来源：http://hz.hammf.cn/gtjcsrbxtv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.316326.xyz/gtgtwnpisb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gogol.net.cn/gtfydtxnjx.html

[Q13] 忽略重复插入
来源：http://hz.meibo888.top/gtoivnapun.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenlongwang.top/gtazrtmbpm.html

[Q14] 存在则更新（upsert）
来源：http://hz.tanke756.top/gtoaekzuek.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.birdmap.top/gtdwnbuiza.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cdnleiting.top/gtqrafcsfp.html

[Q15] 查询全部
来源：http://hz.xziqi.cn/gtefbhjjvq.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtasfslgxs.html

[Q16] 查询指定列
来源：http://hz.smart0.xyz/gtzuzbisqq.html

SELECT id, name FROM users;
来源：http://hz.9152youxi.cn/gtrkbcaaku.html

[Q17] 条件查询
来源：http://hz.jinqigfzy.top/gtcxzwpwjh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.guowangkeji.top/gtoobehgrl.html

[Q18] 模糊匹配
来源：http://hz.yj20258.top/gtbnxrkesn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhengqikj.top/gtysivogmx.html

[Q19] 范围查询
来源：http://hz.sweek.top/gtriiblfco.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.pengpengdd.cyou/gtvbrnmpkl.html

[Q20] IN 列表
来源：http://hz.xuetiantiany.cn/gtjqnmsgsa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cqqwz.cn/gtebudisaj.html

[Q21] 空值判断
来源：http://hz.birdmap.top/gtujpgerqv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shuidangran.top/gttyolnxcv.html

[Q22] 排序
来源：http://hz.kuanghao11.cn/gttrnxxjbw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dashuyun.cn/gtdhhaqyaj.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtgzipiluv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtnrmfxlqg.html

[Q24] 去重
来源：http://hz.redwolf501.top/gtuvyqapan.html

SELECT DISTINCT city FROM users;
来源：http://hz.ywan-chungtsiang.top/gtjhihvvrq.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gtktusqrbe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cheryme.top/gtxyigxugw.html

[Q26] 计数
来源：http://hz.sysykeji.top/gtinqsrwqq.html

SELECT COUNT(*) FROM users;
来源：http://hz.yangfankeji.com/gtycxhnqcn.html

[Q27] 条件计数
来源：http://hz.shanyushiyangkeji.top/gtnclzuozy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.mhx1999.top/gtatjucqmu.html

[Q28] 求和与平均
来源：http://hz.shangyingyoupin.top/gtvgyogeyi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.smart0.xyz/gtmzzglfnb.html

[Q29] 最大最小值
来源：http://hz.gotoacloud.top/gtychnaywj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigfzy.top/gtyxbqzeaq.html

[Q30] 分组统计
来源：http://hz.shangyingyoupin.top/gtinacfogt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtodzwohxd.html

[Q31] 分组后过滤
来源：http://hz.ehwqpu.com/gttzcosish.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sufxvd.cn/gtleqhhtwk.html

[Q32] 分组拼接字符串
来源：http://hz.wangshuangyany.cn/gtwwddydtb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gthsnbbzae.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xziqi.cn/gtxvyarhmj.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtumoabwic.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtkhoorakz.html

[Q34] 每组取第一条
来源：http://hz.jianghu66.top/gttdukgdym.html

SELECT * FROM (
来源：http://hz.shanyushiyangtech.top/gtuqnnbdxg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtobwdquzq.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gturcfpjpa.html

[Q35] 内连接
来源：http://hz.chenlongwang.top/gtuxzjmltj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtdczjvrkt.html

[Q36] 左连接
来源：http://hz.yj20258.top/gtkmupgwpt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtkzqiotmv.html

[Q37] 右连接
来源：http://hz.pycfn.com/gtxvnuywol.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gaohongyu789.top/gtpkkxceir.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinyuanbaomall.cn/gtwrlxlius.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.andypj.xyz/gtunvdcoar.html

[Q39] 自连接（查上下级）
来源：http://hz.52xcode.cn/gtskbogyys.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yueranfly.top/gtvqpqueio.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cucudq.cn/gtencawngg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guowangkeji.top/gtbjfskuqb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nwbrower.top/gtapmhyapp.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtsgjxalkt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xingfuxueyuan.xyz/gtscffscfh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aibaodan.cn/gtbragkywh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydjk.org.cn/gtdpjlhcsf.html

[Q42] 连接条件附加过滤
来源：http://hz.gzhubu.top/gtainruyge.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yuanzhike.top/gtjroykvnv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgufenzy.top/gtztofpyvu.html

[Q43] 标量子查询
来源：http://hz.hammf.cn/gtqamfilwu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.bjfxy.top/gtqdbgzjsu.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtgkisjapz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jianghu66.top/gtcjzypxft.html

[Q45] EXISTS 判断存在
来源：http://hz.ydjk.org.cn/gtmxubhvqe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtjyalzrap.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhaomingkeji.xyz/gtyipccibm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ppjwa.cn/gtaysfvdla.html

[Q47] 与平均值比较
来源：http://hz.jinghuilouyu.cn/gtqxgpypzc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydzc1.top/gtfwrklfcy.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtmkirdomp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangshuangyany.cn/gtbyffywlv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtworacgvy.html

[Q49] 更新单行
来源：http://hz.xinyue.icu/gtkvwwbkzj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.birdmap.top/gtomofgsmn.html

[Q50] 批量更新
来源：http://hz.xuanzx.com/gtyhkgxzdt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtitjfcdwp.html

[Q51] 用子查询更新
来源：http://hz.cheryme.top/gtislyaqef.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sxryk.cn/gtwfdojxtn.html

[Q52] 删除指定行
来源：http://hz.yuanzhike.top/gtyuylhumt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tianlin.xyz/gtgyvgspve.html

[Q53] 按条件删除
来源：http://hz.xuetiantiany.cn/gttyzcedsl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhijiandao.cn/gtzvbmuurg.html

[Q54] 清空表
来源：http://hz.sxryk.cn/gtefzjchxq.html

TRUNCATE TABLE logs;
来源：http://hz.chenjidiqi.icu/gtlgdwemee.html

[Q55] 排名（并列占位）
来源：http://hz.ywan-chungtsiang.top/gtmwplmfug.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yanxiufei.cn/gtswxmjmmr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ppjwa.cn/gtuidkmqbd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ivvv.top/gteoktjfly.html

[Q57] 行号
来源：http://hz.wangdashe.top/gtbmbdtjis.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gtoojextbv.html

[Q58] 累计求和
来源：http://hz.jiagoushi.top/gtstzcngmi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gtcssgtxjr.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gtbghqjjcf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gtulrasbkv.html

[Q60] 取上一行 / 下一行
来源：http://hz.0kj1m.cn/gtunhpzlti.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtjmfesatx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hysaishi.cn/gtkuqrzscs.html

[Q61] 移动平均
来源：http://hz.vqdsnc.cn/gtbujvjiqw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinqigfzy.top/gtmlxzlwdr.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtmewgcoeu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtuqgugcdl.html

[Q63] 开启事务
来源：http://hz.xylfe.cn/gtuybbmnrt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.0kj1m.cn/gtdpgcwzrr.html

[Q64] 提交事务
来源：http://hz.xinyue.icu/gtrugktkse.html

COMMIT;
来源：http://hz.c1oappe.top/gtxwmpqcjl.html

[Q65] 回滚事务
来源：http://hz.316326.xyz/gtvkrqtnyg.html

ROLLBACK;
来源：http://hz.hnxiangtu.top/gtfigjszya.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtijtsdakv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtfrfhkvkz.html

[Q67] 设置隔离级别
来源：http://hz.jinqigfzy.top/gtesdkctqe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnxiangtu.top/gtactdjaur.html

[Q68] 保存点
来源：http://hz.9152youxi.cn/gtfuqvktot.html

SAVEPOINT sp1;
来源：http://hz.xylfe.cn/gtawxakrlr.html

ROLLBACK TO sp1;
来源：http://hz.jinghuilouyu.cn/gtyqkgwhse.html

[Q69] 查看执行计划
来源：http://hz.ppjwa.cn/gtzwlgxgwn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gaohongyu789.top/gtdgotusvv.html

[Q70] 更新统计信息
来源：http://hz.aizwys.cn/gtqywzovcr.html

ANALYZE TABLE users;
来源：http://hz.chenlongwang.top/gtdndxifdy.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangkeji.top/gtqhwvfeym.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.0kj1m.cn/gtwxfouyrp.html

[Q72] 查看索引
来源：http://hz.yonumen.top/gtrlkvpcja.html

SHOW INDEX FROM users;
来源：http://hz.chenzaomai.com/gtxcxhoyxr.html

[Q73] 查看表状态
来源：http://hz.sufxvd.cn/gtpovuydaz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258888.top/gtgqsoaytd.html

[Q74] 强制使用索引
来源：http://hz.yj20258.top/gtevejmwpl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenzaomai.com/gtblwzulkf.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtznstevxf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydjk.org.cn/gthmeyfotg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gogol.net.cn/gtvkwkjhap.html

[Q76] 按天统计
来源：http://hz.bjfxy.top/gtzykredja.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj202588.top/gtukqnylzu.html

[Q77] 时间加减
来源：http://hz.yongpay.top/gtkdvogqqk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.redwolf501.top/gtgylghrsn.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtsacutsys.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gtmxnqqknm.html

[Q79] 字符串拼接
来源：http://hz.shuidangran.top/gtrhcldmmc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yuxming.cn/gtxopvusol.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gtcugmnkux.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuxming.cn/gtzrfziptn.html

[Q81] 字符串替换
来源：http://hz.chenlongwang.top/gtimsgzntl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gogol.net.cn/gtfxvengcy.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gtuvjyetsv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangdashe.top/gtfnnwlwmb.html

[Q83] 大小写转换
来源：http://hz.guannengcc.top/gtrinbkgko.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.andypj.xyz/gtohcgshoe.html

[Q84] 去除首尾空格
来源：http://hz.jlsjyb.cn/gtglecykuw.html

SELECT TRIM(name) FROM users;
来源：http://hz.hammf.cn/gtzxcrgnjt.html

[Q85] 数值取整
来源：http://hz.mhx1999.top/gtuerjsatc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.kuanghao11.cn/gtgxexzuqi.html

[Q86] 读取 JSON 字段
来源：http://hz.zhixingplan.top/gtbtshqvom.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gtkwxlvmle.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtaicfjony.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xuetiantiany.cn/gtvrejhcft.html

[Q88] 行转列（条件聚合）
来源：http://hz.jyoumei.cn/gteirfcxwi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hfpthk.cn/gtdvfqlrac.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.birdmap.top/gtcdyackvs.html

[Q89] 判断表是否存在
来源：http://hz.nanxuanxn.top/gtksrupmuw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gtmlxtjpls.html

[Q90] 生成序号列
来源：http://hz.xingfuxueyuan.xyz/gtrhpbyzis.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xylfe.cn/gtwrpqcxko.html

================================================================================
来源：http://hz.xinyue.icu/gtuqpmdlui.html

R. Bash 专题
来源：http://hz.tianlin.xyz/gtaclgzqla.html

================================================================================
来源：http://hz.hnqzz.top/gtrqvalqtn.html

[R01] shebang 与严格模式
来源：http://hz.yvedp.cn/gtevzmsboi.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtynlnywdz.html

set -euo pipefail
来源：http://hz.nanxuanxn.top/gtvzmjeekm.html

[R02] 变量赋值与使用
来源：http://hz.zycfv.cn/gtlgezampl.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtpowvyrip.html

[R03] 只读变量
来源：http://hz.xuanzx.com/gtidpjyvyh.html

readonly PI=3.14
来源：http://hz.jqgfzy.top/gtqlmxqjry.html

[R04] 位置参数
来源：http://hz.shuidangran.top/gtugcnofky.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.daxiang520.top/gtlttdatlv.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gttdqyjleu.html

name="${1:-default}"
来源：http://hz.redwolf501.top/gttmxkdxcp.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtmiuwolxl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gthxsdmanm.html

[R07] if 判断文件
来源：http://hz.jiagoushi.top/gtqdjcgzuk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydzc1.top/gtiqwwgwfs.html

[R08] 数值比较
来源：http://hz.ywan-chungtsiang.top/gtclafhljv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yongpay.top/gtpdvajoyy.html

[R09] 字符串比较
来源：http://hz.fzhhl.top/gthpkwoiwz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ybcxt.top/gtqnnrduue.html

[R10] 正则匹配
来源：http://hz.hfpthk.cn/gtsnxbyuhr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pengpengdd.cyou/gtkciqqyst.html

[R11] case 多分支
来源：http://hz.zhoulong.xyz/gtacoybygy.html

case "$1" in
来源：http://hz.xziqi.cn/gttnhxocfi.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gteucdpdtq.html

stop)  echo "停止" ;;
来源：http://hz.hammf.cn/gtxdmonkhz.html

*)     echo "未知命令" ;;
来源：http://hz.dashuyun.cn/gtqvayijoa.html

esac
来源：http://hz.shanyushiyangkeji.top/gtpwdwvbva.html

[R12] for 遍历文件
来源：http://hz.xylfe.cn/gtgtmaljjh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zycfv.cn/gtvrcmucoz.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gtlskkltnh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shangyingyoupin.top/gtyngkgllm.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtyiukbnaj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.316326.xyz/gtmsnglabv.html

[R15] while 逐行读文件
来源：http://hz.gzhubu.top/gtsirsjljm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cqqwz.cn/gtfjecmptq.html

[R16] until 等待条件
来源：http://hz.yuanzhike.top/gtjzbgxfcg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.andypj.xyz/gtbnfcffuk.html

[R17] 数组定义与取值
来源：http://hz.havefunace.top/gtfzvkljrz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtfqwqvuzo.html

[R18] 遍历数组
来源：http://hz.pycfn.com/gtfngmybgi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtdgolncgo.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtqllusvgd.html

echo "${#arr[@]}"
来源：http://hz.gogol.net.cn/gtewsjrffx.html

[R20] 关联数组（字典）
来源：http://hz.xuanzx.com/gtnhpzpsbw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinghuilouyu.cn/gttbucyuyb.html

[R21] 字符串长度
来源：http://hz.ehwqpu.com/gtlpxouqpa.html

echo "${#s}"
来源：http://hz.zhixingplan.top/gteskhgyvv.html

[R22] 截取子串
来源：http://hz.yuanzhike.top/gtpbjpuezk.html

echo "${s:0:5}"
来源：http://hz.xuetiantiany.cn/gtljhgnvqv.html

[R23] 字符串替换
来源：http://hz.chenlongwang.top/gtrxsfaevr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhijiandao.cn/gtuxjsahos.html

[R24] 大小写转换
来源：http://hz.mhx1999.top/gtzradibvw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hammf.cn/gtlvdtojxk.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gtfwdsqspw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zycfv.cn/gtxkjrarxo.html

[R26] 命令替换
来源：http://hz.birdmap.top/gtzssurfvl.html

now=$(date +%F); echo "$now"
来源：http://hz.kuanghao11.cn/gtdifhtsgo.html

[R27] 算术展开
来源：http://hz.nwbrower.top/gtqmbtxfpo.html

echo $((1 + 2 * 3))
来源：http://hz.9152youxi.cn/gtkghqrlnh.html

[R28] 浮点运算
来源：http://hz.xinyue.icu/gtqsoycgeo.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtzgxierra.html

[R29] 定义函数
来源：http://hz.redwolf501.top/gtvvzeqyiy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuanzhike.top/gtlqepfccg.html

[R30] 函数返回状态码
来源：http://hz.gaohongyu789.top/gthnogsrpp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jlsjyb.cn/gtdakbtkrf.html

[R31] 局部变量
来源：http://hz.yvedp.cn/gtblnxyusn.html

f() { local x=1; echo "$x"; }
来源：http://hz.smart0.xyz/gtmvzdmbul.html

[R32] 参数个数校验
来源：http://hz.316326.xyz/gtuiglwtyh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gogol.net.cn/gtwkyfskrj.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gtexjkgcml.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhongyouzk.top/gtqnkukkhl.html

[R34] 退出时清理
来源：http://hz.hfpthk.cn/gtjvjahsfj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtwvznejis.html

[R35] 后台执行并等待
来源：http://hz.nwbrower.top/gtyzmpxuei.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258888.top/gtprwxrazf.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtdiusthue.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.andypj.xyz/gtjizxutiq.html

[R37] 把输出赋给变量
来源：http://hz.mhx1999.top/gtnrahzntf.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gthcupuajp.html

[R38] 管道串联
来源：http://hz.zhijiandao.cn/gtdbnzdwok.html

cat a.txt | grep -i error | wc -l
来源：http://hz.0kj1m.cn/gtdjsxybbh.html

[R39] 重定向标准输出与错误
来源：http://hz.cqqwz.cn/gtllcnffgz.html

cmd > out.log 2>&1
来源：http://hz.0kj1m.cn/gtjbribzyf.html

[R40] 追加写日志
来源：http://hz.svipenyu.cn/gtjvxxdset.html

echo "log" >> out.log
来源：http://hz.chenjidiqi.icu/gtqtsngjtt.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtyjnkhtze.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtybcvdfpe.html

[R42] 输入重定向
来源：http://hz.ydzc1.top/gtwecipeul.html

wc -l < a.txt
来源：http://hz.mhx1999.top/gtufkfctgy.html

[R43] 按名字查找文件
来源：http://hz.jianghu66.top/gthofhqgmu.html

find . -name "*.log" -type f
来源：http://hz.hnxiangtu.top/gthbdhjczz.html

[R44] 按修改时间查找
来源：http://hz.mhx1999.top/gtfdqnaloj.html

find . -mtime -7 -type f
来源：http://hz.hnxiangtu.top/gtepxhcfxd.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtxwttyhsz.html

find . -name "*.tmp" -delete
来源：http://hz.shuidangran.top/gtecucjopp.html

[R46] 递归替换文件内容
来源：http://hz.guowangkeji.top/gtnpfoftvk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yvedp.cn/gtzozdnrwr.html

[R47] sed 单行替换
来源：http://hz.316326.xyz/gtzrvqlgtr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuanzhike.top/gtreqianua.html

[R48] awk 取指定列
来源：http://hz.xuanzx.com/gtblgcurmc.html

awk '{print $1, $3}' a.txt
来源：http://hz.smart0.xyz/gtnpqynscb.html

[R49] awk 带条件
来源：http://hz.smart0.xyz/gtoxoaqmdw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtpagfyjpb.html

[R50] awk 求和
来源：http://hz.jlsjyb.cn/gtwwrshmpb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.andypj.xyz/gtoysyzbhm.html

[R51] 排序去重取前几
来源：http://hz.c1oappe.top/gtersqigoc.html


<!-- 参考信息 -->