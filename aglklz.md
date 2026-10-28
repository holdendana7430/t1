代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.mhx1999.top/gtonjbubgk.html

user_id INT NOT NULL,
来源：http://hz.kuanghao11.cn/gteewjheop.html

amount DECIMAL(10, 2),
来源：http://hz.yanxiufei.cn/gtzqiafcvf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.daria6918.cn/gtgafvhngf.html

);
来源：http://hz.cdnleiting.top/gtxhkloxit.html

[Q03] 增加列
来源：http://hz.yonumen.top/gttxtrblkp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ivvv.top/gtkjjdayhw.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtwtbcbiee.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.feifeiyinyue.top/gtxprjvatw.html

[Q05] 重命名列
来源：http://hz.hongshengwenyu.top/gtjmicblgd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nwbrower.top/gtwuupihip.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtfbieduek.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhengqikj.top/gturovdygu.html

[Q07] 删除表
来源：http://hz.sweek.top/gtrdradewv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.meibo888.top/gtvyqetqeu.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtooqvexof.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ivvv.top/gtoopdlemm.html

[Q09] 创建唯一索引
来源：http://hz.hysaishi.cn/gtwoerstgl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.c1oappe.top/gtmnjrnhir.html

[Q10] 插入单行
来源：http://hz.andypj.xyz/gtvzadyluo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.316326.xyz/gtvrrdireb.html

[Q11] 一次插入多行
来源：http://hz.smart0.xyz/gtsjyvibct.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigufen.top/gttadaanwn.html

[Q12] 插入后取自增 ID
来源：http://hz.hysaishi.cn/gtdiujxwan.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sxryk.cn/gtozjhucwz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtpuhmoijo.html

[Q13] 忽略重复插入
来源：http://hz.snrcjt.cn/gtqfxzkzss.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangkeji.top/gtsqroxbrw.html

[Q14] 存在则更新（upsert）
来源：http://hz.jiagoushi.top/gtskyznqfk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.havefunace.top/gtwapwlofh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gtzmlxhbaa.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtotzlodqk.html

SELECT * FROM users;
来源：http://hz.jiagoushi.top/gtdxdkkxag.html

[Q16] 查询指定列
来源：http://hz.cheryme.top/gtyjqwbpkc.html

SELECT id, name FROM users;
来源：http://hz.xinyue.icu/gtihjyitcz.html

[Q17] 条件查询
来源：http://hz.yongpay.top/gtskysfnua.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuxming.cn/gtzwuvwclj.html

[Q18] 模糊匹配
来源：http://hz.zhixingplan.top/gtkqghmjas.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.mhx1999.top/gtfypzmxdd.html

[Q19] 范围查询
来源：http://hz.hammf.cn/gtgrxdozcq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gotoacloud.top/gtnnutcdvv.html

[Q20] IN 列表
来源：http://hz.birdmap.top/gtqovzdwgz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xziqi.cn/gtlvihtktb.html

[Q21] 空值判断
来源：http://hz.andypj.xyz/gtjjakroea.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jianghu66.top/gtljsrxjuy.html

[Q22] 排序
来源：http://hz.c1oappe.top/gtplmlqoih.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gtimbbcyii.html

[Q23] 分页
来源：http://hz.shangyingyoupin.top/gtdvuazlgn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ivvv.top/gtuzzxqnnp.html

[Q24] 去重
来源：http://hz.hnqzz.top/gtobyyzvza.html

SELECT DISTINCT city FROM users;
来源：http://hz.jyoumei.cn/gtduhnmpof.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gtrssjskxe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gtnkwixzau.html

[Q26] 计数
来源：http://hz.tanke756.top/gtmkiqtqtq.html

SELECT COUNT(*) FROM users;
来源：http://hz.316326.xyz/gtmqzuecbl.html

[Q27] 条件计数
来源：http://hz.c1oappe.top/gtkflmpdbc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hongshengwenyu.top/gtavpveguz.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtoklgdlpb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258.top/gtgmizczxn.html

[Q29] 最大最小值
来源：http://hz.guowangkeji.top/gtrqgnrruf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xuanzx.com/gtbilgqsba.html

[Q30] 分组统计
来源：http://hz.guowangkeji.top/gtwjqgmeri.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtpdmixudv.html

[Q31] 分组后过滤
来源：http://hz.zhongyouzk.top/gtwhzmxupn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cucudq.cn/gtifavesez.html

[Q32] 分组拼接字符串
来源：http://hz.fzhhl.top/gtyezujtxb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtqutxwhsz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydjk.org.cn/gttmdibrff.html

[Q33] 多列分组
来源：http://hz.aibaodan.cn/gtfixktzjx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zycfv.cn/gtigxhlafd.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gttvaurffz.html

SELECT * FROM (
来源：http://hz.fengsongda.top/gtoexawpyk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dianchejie.cn/gtoijanhrk.html

) t WHERE rn = 1;
来源：http://hz.zycfv.cn/gtzyqhdlty.html

[Q35] 内连接
来源：http://hz.daxiang520.top/gtetqxiimf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtrlhzbrav.html

[Q36] 左连接
来源：http://hz.tanke756.top/gtyrrtewzj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gttptyqumz.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gttjppnsxt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenlongwang.top/gtdfstutes.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yangfankeji.com/gtrqulrwen.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigfzy.top/gtqgxjtqzt.html

[Q39] 自连接（查上下级）
来源：http://hz.chenzaomai.com/gtajkjymfe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhixingplan.top/gtcezekyvd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tianlin.xyz/gtvxrjqomr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hammf.cn/gtojuenauj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cucudq.cn/gtaojysbye.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gthocohvll.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daxiang520.top/gtvksaykdq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.bjfxy.top/gtxvnyekjp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ehwqpu.com/gtejidujkx.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtfcgpopsb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigufen.top/gtuwzgdxtr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pengpengdd.cyou/gthrypyygx.html

[Q43] 标量子查询
来源：http://hz.gotoacloud.top/gtxaximqrh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hfpthk.cn/gtpiorkzvg.html

[Q44] IN 子查询
来源：http://hz.iojbl.cn/gtwxhtlytw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zdqjudy.top/gthhmikmkw.html

[Q45] EXISTS 判断存在
来源：http://hz.hnqzz.top/gtzzguustn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtlprnhmob.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinyuanbaomall.cn/gtdijuvmpa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dianchejie.cn/gtctsxeufb.html

[Q47] 与平均值比较
来源：http://hz.shzxlz.cn/gtejwgaptq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigfzy.top/gthaakrbvp.html

[Q48] CTE 公用表表达式
来源：http://hz.cqqwz.cn/gtlnqnuhzy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhoulong.xyz/gtlwakswse.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtcancbdfm.html

[Q49] 更新单行
来源：http://hz.gotoacloud.top/gtuwicgqxl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dashuyun.cn/gtnhtjrhoa.html

[Q50] 批量更新
来源：http://hz.zhixingplan.top/gtfrjdsluy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangkeji.top/gtayqegaty.html

[Q51] 用子查询更新
来源：http://hz.yueranfly.top/gtgbhqggle.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aizwys.cn/gtdshivzxk.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gteykqzbwg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fzhhl.top/gtqodnkmxt.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtcmicmkib.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jianghu66.top/gtipcxzomi.html

[Q54] 清空表
来源：http://hz.hysaishi.cn/gtgrgdyzzr.html

TRUNCATE TABLE logs;
来源：http://hz.xylfe.cn/gtpmbbsdsk.html

[Q55] 排名（并列占位）
来源：http://hz.zhixingplan.top/gtjmddaevo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nwbrower.top/gtkdssdpzm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangdashe.top/gttlyfqfkf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ppjwa.cn/gttvwfcivq.html

[Q57] 行号
来源：http://hz.havefunace.top/gtcuhjbecr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hywenlv.cn/gtdmxuqqep.html

[Q58] 累计求和
来源：http://hz.hnxiangtu.top/gthumggrjz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hysaishi.cn/gtdfnrxwzp.html

[Q59] 分组内累计
来源：http://hz.gaohongyu789.top/gtiitfichz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.iojbl.cn/gtafmatzmy.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuanzhike.top/gtkhrlizkn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tianlin.xyz/gtwogjkrol.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgfzy.top/gtorzwnzuq.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtefbmgddi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtqivqmvle.html

[Q62] 分组占比
来源：http://hz.birdmap.top/gtflgvjjoi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtsclkpmag.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtigwpwyua.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ivvv.top/gtjnjfymlr.html

[Q64] 提交事务
来源：http://hz.sweek.top/gtfmzbxusl.html

COMMIT;
来源：http://hz.jinqigufen.top/gtlftbvjwv.html

[Q65] 回滚事务
来源：http://hz.pengpengdd.cyou/gtoaefjpxr.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtekvxwouv.html

[Q66] 行锁查询
来源：http://hz.haohaochexian.top/gttzucqygb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tanke756.top/gtiaxxqvbh.html

[Q67] 设置隔离级别
来源：http://hz.zhoulong.xyz/gtnyyrvazz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dianchejie.cn/gtgdawwgov.html

[Q68] 保存点
来源：http://hz.wangshuangyany.cn/gtuvegabxr.html

SAVEPOINT sp1;
来源：http://hz.tanke756.top/gtmxczcdul.html

ROLLBACK TO sp1;
来源：http://hz.tian-w.cn/gtpbwlemsc.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtwwjkcuhg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xinyue.icu/gtwlnxonpg.html

[Q70] 更新统计信息
来源：http://hz.gotoacloud.top/gtcobvlekv.html

ANALYZE TABLE users;
来源：http://hz.dianchejie.cn/gthwuxoiod.html

[Q71] 查看建表语句
来源：http://hz.ivvv.top/gtwkywvmzf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gotoacloud.top/gtdfdqyhtp.html

[Q72] 查看索引
来源：http://hz.havefunace.top/gtikrvyfct.html

SHOW INDEX FROM users;
来源：http://hz.smart0.xyz/gtsmpxwfbc.html

[Q73] 查看表状态
来源：http://hz.zhixingplan.top/gthtvvzlfi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.iojbl.cn/gtwddtyzny.html

[Q74] 强制使用索引
来源：http://hz.ywan-chungtsiang.top/gtwohwzdci.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dashuyun.cn/gtccuzwiwy.html

[Q75] 日期格式化
来源：http://hz.jiagoushi.top/gtposvmwyj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtnhciuvoe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gotoacloud.top/gttkqrdydd.html

[Q76] 按天统计
来源：http://hz.chenlongwang.top/gtrqjcbicd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gogol.net.cn/gtfxlrejfn.html

[Q77] 时间加减
来源：http://hz.aizwys.cn/gtngevicqn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gtydwkrasl.html

[Q78] 当前时间
来源：http://hz.cqqwz.cn/gtfvyacrqo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yongpay.top/gtfvmncjla.html

[Q79] 字符串拼接
来源：http://hz.yongpay.top/gtloayvgna.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cashguo.top/gtycxarvdy.html

[Q80] 字符串截取
来源：http://hz.jiagoushi.top/gtmpthtijy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gogol.net.cn/gtdcrahadk.html

[Q81] 字符串替换
来源：http://hz.cashguo.top/gtygzkfqgd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zdqjudy.top/gtbfgsgmbg.html

[Q82] 字符长度与字节长度
来源：http://hz.xinyue.icu/gtbehgxoli.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cdnleiting.top/gtqoeuyjmb.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtohhmvztd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtmrvxlfbh.html

[Q84] 去除首尾空格
来源：http://hz.redwolf501.top/gtvwhvetrx.html

SELECT TRIM(name) FROM users;
来源：http://hz.316326.xyz/gtylucnvth.html

[Q85] 数值取整
来源：http://hz.yj20258888.top/gtwbvyzncc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangdashe.top/gtpudcsvwd.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtnpfkgpkp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ydjk.org.cn/gtqerxkukq.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangtech.top/gtuesrbfbo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtxusmdncz.html

[Q88] 行转列（条件聚合）
来源：http://hz.yanxiufei.cn/gtbioxhtha.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tanke756.top/gtnzmpkidk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.vqdsnc.cn/gtzlymujju.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtlpsmlofa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jlsjyb.cn/gtegjxuwsp.html

[Q90] 生成序号列
来源：http://hz.chenlongwang.top/gtiabduvtv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jianghu66.top/gtnyskilmg.html

================================================================================
来源：http://hz.9152youxi.cn/gtrsxbddsq.html

R. Bash 专题
来源：http://hz.chenlongwang.top/gtrkoxncpc.html

================================================================================
来源：http://hz.havefunace.top/gtdfizposk.html

[R01] shebang 与严格模式
来源：http://hz.zdqjudy.top/gtwjgxelfd.html

#!/usr/bin/env bash
来源：http://hz.fzhhl.top/gtcaavikob.html

set -euo pipefail
来源：http://hz.pycfn.com/gtxamdabkr.html

[R02] 变量赋值与使用
来源：http://hz.52xcode.cn/gtmgetntaa.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gthoyglmvr.html

[R03] 只读变量
来源：http://hz.zhongyouzk.top/gtklizzfoz.html

readonly PI=3.14
来源：http://hz.52xcode.cn/gtkvkojuua.html

[R04] 位置参数
来源：http://hz.hywenlv.cn/gtvfcnsqsc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.52xcode.cn/gtrmlrvmuz.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtdjottnum.html

name="${1:-default}"
来源：http://hz.yj20258888.top/gtpbbkkigt.html

[R06] 判断命令是否存在
来源：http://hz.xziqi.cn/gtnpcigbhz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtmxbbhlef.html

[R07] if 判断文件
来源：http://hz.birdmap.top/gtzdbzwrva.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xuanzx.com/gtpamvhlnc.html

[R08] 数值比较
来源：http://hz.gogol.net.cn/gtshvyqhqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ivvv.top/gteicxecpu.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtptufajcm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj202588.top/gthucnblso.html

[R10] 正则匹配
来源：http://hz.xuanzx.com/gtflmfjazt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.iojbl.cn/gtvygpymwi.html

[R11] case 多分支
来源：http://hz.guowangkeji.top/gtdwejvmsf.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gtluplmxjh.html

start) echo "启动" ;;
来源：http://hz.gzhubu.top/gtpuwwhjzr.html

stop)  echo "停止" ;;
来源：http://hz.xuanzx.com/gtgfwtmgwj.html

*)     echo "未知命令" ;;
来源：http://hz.52xcode.cn/gtndxgwfas.html

esac
来源：http://hz.jqgufenzy.top/gtmzoviimf.html

[R12] for 遍历文件
来源：http://hz.wangshuangyany.cn/gtsrmwkrmd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.vqdsnc.cn/gttzldbnoz.html

[R13] for 计数循环
来源：http://hz.sysykeji.top/gtnppxuhwn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258888.top/gtbcevryxh.html

[R14] C 风格 for
来源：http://hz.zhiwuduotai.top/gtlinrsnjs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shangyingyoupin.top/gtiaiaxuin.html

[R15] while 逐行读文件
来源：http://hz.aizwys.cn/gthxxdcxkn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinyuanbaomall.cn/gtsvtypvvr.html

[R16] until 等待条件
来源：http://hz.haohaochexian.top/gtivsmsbfm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtunrjytta.html

[R17] 数组定义与取值
来源：http://hz.jqgufenzy.top/gtldhrcfyu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gtkyjlswoj.html

[R18] 遍历数组
来源：http://hz.pycfn.com/gtgubsfkvg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sysykeji.top/gthixfrooa.html

[R19] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtezmmeiyt.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtmkkqtnyw.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gtwcevjalp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yangfankeji.com/gtxbbngpdg.html

[R21] 字符串长度
来源：http://hz.birdmap.top/gtyhxrrrlk.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtotfkzirv.html

[R22] 截取子串
来源：http://hz.redwolf501.top/gtyfvrtwwh.html

echo "${s:0:5}"
来源：http://hz.yangfankeji.com/gtfuxxvauv.html

[R23] 字符串替换
来源：http://hz.chenjidiqi.icu/gtchyuckta.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.c1oappe.top/gtegcgfxdl.html

[R24] 大小写转换
来源：http://hz.yuanzhike.top/gtxjrrlnms.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tian-w.cn/gtbnxoobwy.html

[R25] 去后缀 / 去前缀
来源：http://hz.hfpthk.cn/gtkyppkqif.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgufenzy.top/gtgwbsvevc.html

[R26] 命令替换
来源：http://hz.hongshengwenyu.top/gtjhbivlrq.html

now=$(date +%F); echo "$now"
来源：http://hz.fengsongda.top/gtmzcrkxdc.html

[R27] 算术展开
来源：http://hz.tianlin.xyz/gtyhdpigtc.html

echo $((1 + 2 * 3))
来源：http://hz.fengsongda.top/gtckfjxyzh.html

[R28] 浮点运算
来源：http://hz.ehwqpu.com/gtgxeepikv.html

echo "scale=2; 10/3" | bc
来源：http://hz.yangfankeji.com/gtadkloyxi.html

[R29] 定义函数
来源：http://hz.kuanghao11.cn/gtmotxsqca.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.haohaochexian.top/gtiweouvxj.html

[R30] 函数返回状态码
来源：http://hz.xziqi.cn/gtsswonpig.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yanxiufei.cn/gthbvolpqp.html

[R31] 局部变量
来源：http://hz.jinqigfzy.top/gtwdqebbde.html

f() { local x=1; echo "$x"; }
来源：http://hz.zycfv.cn/gtszxbdejk.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtodhikixc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.haohaochexian.top/gtvweieprv.html

[R33] 捕获错误并提示行号
来源：http://hz.wangdashe.top/gtegljvajy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ywan-chungtsiang.top/gtkjdxygpi.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gtvkdawhgv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtpujeueuc.html

[R35] 后台执行并等待
来源：http://hz.yuanzhike.top/gtpefrguoi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhiwuduotai.top/gtgfeokexq.html

[R36] 并发执行多个任务
来源：http://hz.chenjidiqi.icu/gtzzjvefdv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhixingplan.top/gtwcnwjrac.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangtech.top/gtrbfpegqe.html

files=$(ls -1)
来源：http://hz.sufxvd.cn/gtrtsdvori.html

[R38] 管道串联
来源：http://hz.yj202588.top/gtatvqeiuc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtkoeqhgwi.html

[R39] 重定向标准输出与错误
来源：http://hz.daria6918.cn/gtoiykpoch.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtleaurchp.html

[R40] 追加写日志
来源：http://hz.hammf.cn/gtqkqewyzo.html

echo "log" >> out.log
来源：http://hz.shanyushiyangtech.top/gtviuqmseg.html

[R41] 丢弃输出
来源：http://hz.aizwys.cn/gtxunearqs.html

cmd >/dev/null 2>&1
来源：http://hz.feifeiyinyue.top/gtxybdkitw.html

[R42] 输入重定向
来源：http://hz.fzhhl.top/gtcgulafae.html

wc -l < a.txt
来源：http://hz.jianghu66.top/gteoknfatd.html

[R43] 按名字查找文件
来源：http://hz.havefunace.top/gtmgtvsqyx.html

find . -name "*.log" -type f
来源：http://hz.cheryme.top/gtnobhyvse.html

[R44] 按修改时间查找
来源：http://hz.chenlongwang.top/gtdezuvegk.html

find . -mtime -7 -type f
来源：http://hz.yonumen.top/gttafvlntn.html

[R45] 批量删除
来源：http://hz.wangshuangyany.cn/gtoedhysns.html

find . -name "*.tmp" -delete
来源：http://hz.yonumen.top/gtbsdicfrl.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gteknxmely.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guannengcc.top/gtxcmvajij.html

[R47] sed 单行替换
来源：http://hz.zhongyouzk.top/gtspwecvfe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pycfn.com/gteryukxmr.html

[R48] awk 取指定列
来源：http://hz.hfpthk.cn/gtecopplgq.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuanzhike.top/gthanqzgqv.html

[R49] awk 带条件
来源：http://hz.smart0.xyz/gtivnvcqjs.html


<!-- 参考信息 -->