代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gtwgaeenxq.html

);
来源：http://hz.316326.xyz/gtinaztxzo.html

[Q02] 创建带外键的表
来源：http://hz.yuanzhike.top/gtnhlldfdm.html

CREATE TABLE orders (
来源：http://hz.yj202588.top/gtxjuzwitg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtlfiijhzy.html

user_id INT NOT NULL,
来源：http://hz.hongshengwenyu.top/gtxxaidfat.html

amount DECIMAL(10, 2),
来源：http://hz.xziqi.cn/gtrlsyhllp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nwbrower.top/gtxrqrzfso.html

);
来源：http://hz.xuetiantiany.cn/gtschcdtmf.html

[Q03] 增加列
来源：http://hz.wangshuangyany.cn/gthkuvkbra.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xingfuxueyuan.xyz/gtljitgxub.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gtlhozeoos.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gtsnejntbf.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtgqjfycmh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtucdepbpn.html

[Q06] 删除列
来源：http://hz.c1oappe.top/gtiqsodtyv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.tanke756.top/gtlyoqecyb.html

[Q07] 删除表
来源：http://hz.hammf.cn/gtomblejld.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shuidangran.top/gtrjecpixv.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtatudvijz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zycfv.cn/gthuftapnx.html

[Q09] 创建唯一索引
来源：http://hz.cashguo.top/gtdkwsmutx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yongpay.top/gtveylxlvx.html

[Q10] 插入单行
来源：http://hz.gzhubu.top/gttuzbawzf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuanzx.com/gtsvsifsqj.html

[Q11] 一次插入多行
来源：http://hz.yj202588.top/gtpfezlcis.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dianchejie.cn/gtdpgryire.html

[Q12] 插入后取自增 ID
来源：http://hz.yuanzhike.top/gtwqkfoaht.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtfxgqngjs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.vqdsnc.cn/gtfpfbyktc.html

[Q13] 忽略重复插入
来源：http://hz.xuanzx.com/gtkqwuvcyu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jlsjyb.cn/gtgvtgwkop.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtbqefoywg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ybcxt.top/gtbvarscut.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fzhhl.top/gtpintemje.html

[Q15] 查询全部
来源：http://hz.ydzc1.top/gturzropuo.html

SELECT * FROM users;
来源：http://hz.zhijiandao.cn/gtzuijjuds.html

[Q16] 查询指定列
来源：http://hz.zycfv.cn/gtkcsnzcqg.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtxcyflkop.html

[Q17] 条件查询
来源：http://hz.jinghuilouyu.cn/gtqbzgeulu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tanke756.top/gtcihqjyix.html

[Q18] 模糊匹配
来源：http://hz.hnxiangtu.top/gtocyilzvj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yangfankeji.com/gtwvczhown.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gttbceraux.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hywenlv.cn/gtuueuhkvm.html

[Q20] IN 列表
来源：http://hz.0kj1m.cn/gtjnuqtrwy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shanyushiyangtech.top/gtrfbnylqa.html

[Q21] 空值判断
来源：http://hz.pengpengdd.cyou/gtkdptdwpz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinqigfzy.top/gtlxgykzzp.html

[Q22] 排序
来源：http://hz.yangfankeji.com/gtfdsmtlqd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sweek.top/gtwfvbopnn.html

[Q23] 分页
来源：http://hz.zhoulong.xyz/gtdrwurglu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258.top/gtwlwsorrr.html

[Q24] 去重
来源：http://hz.jinyuanbaomall.cn/gtaukhaeaj.html

SELECT DISTINCT city FROM users;
来源：http://hz.svipenyu.cn/gtnbvzwkhk.html

[Q25] 只取前 N 条
来源：http://hz.quarkkingdee.top/gtpvludsmd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenzaomai.com/gtatollhzu.html

[Q26] 计数
来源：http://hz.gotoacloud.top/gtjmzzwhtn.html

SELECT COUNT(*) FROM users;
来源：http://hz.feifeiyinyue.top/gtoldcgryk.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gtnuezvlxx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hfpthk.cn/gtnnsvwzws.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gttwhzsdii.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.wangdashe.top/gtvfvmiltf.html

[Q29] 最大最小值
来源：http://hz.yvedp.cn/gtuwrhcfca.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxuanxn.top/gthlwiwoko.html

[Q30] 分组统计
来源：http://hz.xingfuxueyuan.xyz/gtkkccidcr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtrqxypdqp.html

[Q31] 分组后过滤
来源：http://hz.gotoacloud.top/gtqzbacoqj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cucudq.cn/gtbnolcupk.html

[Q32] 分组拼接字符串
来源：http://hz.ybcxt.top/gtxukiraci.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gthtaqiwba.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pengpengdd.cyou/gtknekpwbr.html

[Q33] 多列分组
来源：http://hz.sufxvd.cn/gtuugblcbj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.meibo888.top/gtiuobnago.html

[Q34] 每组取第一条
来源：http://hz.gotoacloud.top/gtcxtfcpkg.html

SELECT * FROM (
来源：http://hz.hfpthk.cn/gtfgcmeuzj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnxiangtu.top/gtlukyuelb.html

) t WHERE rn = 1;
来源：http://hz.yj202588.top/gtqgcwhsgp.html

[Q35] 内连接
来源：http://hz.birdmap.top/gtsgtzcjge.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gttagyjzhi.html

[Q36] 左连接
来源：http://hz.guannengcc.top/gtkacqbfqh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gtgxrbouwv.html

[Q37] 右连接
来源：http://hz.zhoulong.xyz/gtuhychcta.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cdnleiting.top/gtkplcllwl.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hywenlv.cn/gtjvurvcsn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.smart0.xyz/gthiwfuber.html

[Q39] 自连接（查上下级）
来源：http://hz.zhijiandao.cn/gtoeczgsps.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtpglspzpf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hywenlv.cn/gtuhrbnygv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtloykvexp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shuidangran.top/gtfokfcieu.html

[Q41] 多表连接
来源：http://hz.zhaomingkeji.xyz/gtshxwbnfo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.aizwys.cn/gtlwvqemjb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.havefunace.top/gtsyyozzvm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinghuilouyu.cn/gtqhollndy.html

[Q42] 连接条件附加过滤
来源：http://hz.yvedp.cn/gtaplggwrd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenlongwang.top/gtgijhwjxg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ivvv.top/gtbvbbhqze.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtwtcflkkl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.vqdsnc.cn/gtddjqnpxr.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtqfxcdsgc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hfpthk.cn/gtkdoibnpd.html

[Q45] EXISTS 判断存在
来源：http://hz.zhijiandao.cn/gtfrzsqecq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtgcuqmyjt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtkrnzevmj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtlslwlyui.html

[Q47] 与平均值比较
来源：http://hz.zdqjudy.top/gtggrodoua.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jyoumei.cn/gtvluhpzrn.html

[Q48] CTE 公用表表达式
来源：http://hz.wangshuangyany.cn/gtloilvzys.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhoulong.xyz/gtogwtozzc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tianlin.xyz/gtakxcpruv.html

[Q49] 更新单行
来源：http://hz.hywenlv.cn/gtmsnjxarr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.9152youxi.cn/gtftwdorur.html

[Q50] 批量更新
来源：http://hz.cheryme.top/gthugonvxe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pengpengdd.cyou/gtptffzzgf.html

[Q51] 用子查询更新
来源：http://hz.shzxlz.cn/gtpbxzlezg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenlongwang.top/gtfgnqgweh.html

[Q52] 删除指定行
来源：http://hz.ywan-chungtsiang.top/gtvdikkkey.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj202588.top/gtlvoxuhwm.html

[Q53] 按条件删除
来源：http://hz.quarkkingdee.top/gtvnzurcwh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtrflcemhf.html

[Q54] 清空表
来源：http://hz.birdmap.top/gtwbdgjftt.html

TRUNCATE TABLE logs;
来源：http://hz.zhengqikj.top/gtuvuuggfo.html

[Q55] 排名（并列占位）
来源：http://hz.yueranfly.top/gtrbdsdobq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ppjwa.cn/gtwsryzjpf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sysykeji.top/gtezjslhmb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cqqwz.cn/gtaomvohpo.html

[Q57] 行号
来源：http://hz.jyoumei.cn/gtyysihjhk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgfzy.top/gtipbldync.html

[Q58] 累计求和
来源：http://hz.zhongyouzk.top/gtoiztawnp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhaomingkeji.xyz/gttpqlkise.html

[Q59] 分组内累计
来源：http://hz.haohaochexian.top/gtsfimkgtw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pengpengdd.cyou/gtcyebeuvh.html

[Q60] 取上一行 / 下一行
来源：http://hz.gzhubu.top/gtvjqystek.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangkeji.top/gthblxtqlg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cqqwz.cn/gtoepebqwt.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtvlabears.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhongyouzk.top/gtxdradcvi.html

[Q62] 分组占比
来源：http://hz.yueranfly.top/gtxgnpvuln.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtjtmyqgto.html

[Q63] 开启事务
来源：http://hz.316326.xyz/gturgbisdl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.c1oappe.top/gtidqzzagb.html

[Q64] 提交事务
来源：http://hz.iojbl.cn/gtrbwiwrep.html

COMMIT;
来源：http://hz.ppjwa.cn/gtpljenczo.html

[Q65] 回滚事务
来源：http://hz.gogol.net.cn/gtpisudgrz.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtxzaatwgb.html

[Q66] 行锁查询
来源：http://hz.dashuyun.cn/gtjgpwxlhr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.smart0.xyz/gthmpywqmc.html

[Q67] 设置隔离级别
来源：http://hz.wangdashe.top/gtzwajvayu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangtech.top/gtwvgdaipx.html

[Q68] 保存点
来源：http://hz.snrcjt.cn/gttngnhmbk.html

SAVEPOINT sp1;
来源：http://hz.zhongyouzk.top/gtckxpbvlm.html

ROLLBACK TO sp1;
来源：http://hz.nanxuanxn.top/gtadtpzpxu.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtzqxrwirz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shzxlz.cn/gttchfdxyx.html

[Q70] 更新统计信息
来源：http://hz.gogol.net.cn/gtsbejiuyl.html

ANALYZE TABLE users;
来源：http://hz.ivvv.top/gtkesfyqyq.html

[Q71] 查看建表语句
来源：http://hz.guannengcc.top/gttmcpirqg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dashuyun.cn/gtyxmllbxa.html

[Q72] 查看索引
来源：http://hz.jlsjyb.cn/gtoevirwoq.html

SHOW INDEX FROM users;
来源：http://hz.yanxiufei.cn/gtlpvjshqz.html

[Q73] 查看表状态
来源：http://hz.nwbrower.top/gtxquwulbb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yueranfly.top/gtkscssrds.html

[Q74] 强制使用索引
来源：http://hz.cqqwz.cn/gtwfuxiedv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuetiantiany.cn/gtspbwctbp.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gtcvarvpoh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gotoacloud.top/gtdhimhrwr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gzhubu.top/gtyqfdgesu.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gtvhslfmja.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ehwqpu.com/gtmpamvwyx.html

[Q77] 时间加减
来源：http://hz.sysykeji.top/gtrmqczyic.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yonumen.top/gtvtgccmqo.html

[Q78] 当前时间
来源：http://hz.ydzc1.top/gtoudiqiht.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xingfuxueyuan.xyz/gtppusxvig.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtcyluwsna.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sysykeji.top/gtjrokuwak.html

[Q80] 字符串截取
来源：http://hz.zhongyouzk.top/gtsmmlhcie.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxuanxn.top/gttoerpttt.html

[Q81] 字符串替换
来源：http://hz.zhijiandao.cn/gtjkyrwmyp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yanxiufei.cn/gtohtlvdec.html

[Q82] 字符长度与字节长度
来源：http://hz.sufxvd.cn/gtxmqjlcww.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.c1oappe.top/gtbaulnrpq.html

[Q83] 大小写转换
来源：http://hz.nanxuanxn.top/gtlejxtpoq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.316326.xyz/gtjesvtjre.html

[Q84] 去除首尾空格
来源：http://hz.jianghu66.top/gtacfrvjvd.html

SELECT TRIM(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtfzcowxzf.html

[Q85] 数值取整
来源：http://hz.xziqi.cn/gtkiockdvy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sufxvd.cn/gtmdaecosz.html

[Q86] 读取 JSON 字段
来源：http://hz.jyoumei.cn/gtnxzvvmlh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.feifeiyinyue.top/gtcnqymcgv.html

[Q87] JSON 字段做条件
来源：http://hz.jinghuilouyu.cn/gteygduywf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tian-w.cn/gtauvohajo.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhijiandao.cn/gtceiwfrbn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhixingplan.top/gtwklvilxz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ywan-chungtsiang.top/gtxhxghtaf.html

[Q89] 判断表是否存在
来源：http://hz.ywan-chungtsiang.top/gtiqpnrtlu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jlsjyb.cn/gtasujydrr.html

[Q90] 生成序号列
来源：http://hz.jinqigufen.top/gtcphdsdyi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.dianchejie.cn/gtmwfzvkon.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdqoyvbrw.html

R. Bash 专题
来源：http://hz.zdqjudy.top/gtbbccpvwf.html

================================================================================
来源：http://hz.nwbrower.top/gtdojbgaov.html

[R01] shebang 与严格模式
来源：http://hz.yuxming.cn/gtlbojbxor.html

#!/usr/bin/env bash
来源：http://hz.zdqjudy.top/gtpgnekugn.html

set -euo pipefail
来源：http://hz.0kj1m.cn/gtsrbmzvuy.html

[R02] 变量赋值与使用
来源：http://hz.wangdashe.top/gtyikeiprp.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gtotyoyktt.html

[R03] 只读变量
来源：http://hz.jinghuilouyu.cn/gtrzukbwzc.html

readonly PI=3.14
来源：http://hz.kuanghao11.cn/gtbymcfdxs.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtwwqgrttu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtyhqvlfjv.html

[R05] 参数默认值
来源：http://hz.52xcode.cn/gtbmhkbmbt.html

name="${1:-default}"
来源：http://hz.meibo888.top/gtidhyppef.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtvgeutmwl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yanxiufei.cn/gtuffcbssi.html

[R07] if 判断文件
来源：http://hz.jinqigfzy.top/gtdqlnpapx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangshuangyany.cn/gtcalazwzc.html

[R08] 数值比较
来源：http://hz.shanyushiyangkeji.top/gtnjqxjqdi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinghuilouyu.cn/gtitaepiyl.html

[R09] 字符串比较
来源：http://hz.daria6918.cn/gtsvxgbrst.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.mhx1999.top/gtpixcwkrl.html

[R10] 正则匹配
来源：http://hz.shuidangran.top/gtvcwvoctk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.feifeiyinyue.top/gtusrhsurl.html

[R11] case 多分支
来源：http://hz.tanke756.top/gtwbpsezco.html

case "$1" in
来源：http://hz.quarkkingdee.top/gtsybuuszt.html

start) echo "启动" ;;
来源：http://hz.andypj.xyz/gtwlneklnu.html

stop)  echo "停止" ;;
来源：http://hz.ydjk.org.cn/gtfrucsnko.html

*)     echo "未知命令" ;;
来源：http://hz.jlsjyb.cn/gtezmlpmiy.html

esac
来源：http://hz.zhiwuduotai.top/gtnwnwiing.html

[R12] for 遍历文件
来源：http://hz.cashguo.top/gtmkjzfngr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cucudq.cn/gtobnjgrcc.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtwtaslaxz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fengsongda.top/gthyktxkli.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gtizgqkfmt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yvedp.cn/gtotkcjopj.html

[R15] while 逐行读文件
来源：http://hz.tanke756.top/gtgphewims.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.feifeiyinyue.top/gtjkpqrsvz.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtqbfvfqet.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tian-w.cn/gtmtavltyp.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtmbcmgovd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nwbrower.top/gtglbnwkjc.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gtsfnxvxpx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinyuanbaomall.cn/gtphkpewpy.html

[R19] 数组长度
来源：http://hz.zhengqikj.top/gtjsoetmya.html

echo "${#arr[@]}"
来源：http://hz.cucudq.cn/gtugqdddtl.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtxoqbbrtj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cqqwz.cn/gtcvseoqzu.html

[R21] 字符串长度
来源：http://hz.hysaishi.cn/gtlyqdwvlw.html

echo "${#s}"
来源：http://hz.316326.xyz/gtjujthjgi.html

[R22] 截取子串
来源：http://hz.fzhhl.top/gtveqqqjbl.html

echo "${s:0:5}"
来源：http://hz.ppjwa.cn/gtlrmufkrz.html

[R23] 字符串替换
来源：http://hz.xylfe.cn/gtfatzjbor.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cheryme.top/gtjnuiehxt.html

[R24] 大小写转换
来源：http://hz.quarkkingdee.top/gtexrujlrp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nwbrower.top/gtlfoferem.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtwokkcdva.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ybcxt.top/gtvtogkjni.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gtlcldbonn.html

now=$(date +%F); echo "$now"
来源：http://hz.cashguo.top/gthoylraez.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtwqsnurle.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangkeji.top/gtfldujgzd.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gtqhllwbcm.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinyuanbaomall.cn/gtnjfivzfr.html

[R29] 定义函数
来源：http://hz.svipenyu.cn/gtfucupswl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aibaodan.cn/gtvxkuolfi.html

[R30] 函数返回状态码
来源：http://hz.guowangkeji.top/gtjkgllyet.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258.top/gtxswlfaxb.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtwvpfuauc.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenjidiqi.icu/gtdzglsokn.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtqzqksdve.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yvedp.cn/gtqzsqkopp.html

[R33] 捕获错误并提示行号
来源：http://hz.guannengcc.top/gturnlnysf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hysaishi.cn/gturvsropa.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtotrsqprt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gttznutzqi.html

[R35] 后台执行并等待
来源：http://hz.aibaodan.cn/gtaqtcncpp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.c1oappe.top/gtobvyfvtx.html

[R36] 并发执行多个任务
来源：http://hz.zhiwuduotai.top/gtdgrvgxrj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.c1oappe.top/gtvzqzcicc.html

[R37] 把输出赋给变量
来源：http://hz.kuanghao11.cn/gtrewigxzf.html

files=$(ls -1)
来源：http://hz.jinqigfzy.top/gtwczsfcey.html

[R38] 管道串联
来源：http://hz.jiagoushi.top/gtlnsekwlj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtdxebyfyw.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtwaxwagvg.html

cmd > out.log 2>&1
来源：http://hz.vqdsnc.cn/gtdiiflkte.html

[R40] 追加写日志
来源：http://hz.cdnleiting.top/gtnwvzyndr.html

echo "log" >> out.log
来源：http://hz.xinyue.icu/gtvqvugynz.html

[R41] 丢弃输出
来源：http://hz.shzxlz.cn/gtmvinmkph.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gtwqcmncdc.html

[R42] 输入重定向
来源：http://hz.tianlin.xyz/gtvvdzyvvk.html

wc -l < a.txt
来源：http://hz.hnxiangtu.top/gtovcsnlct.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtcyzugopx.html

find . -name "*.log" -type f
来源：http://hz.hnqzz.top/gtaymarqqr.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gtnkpkwgtd.html

find . -mtime -7 -type f
来源：http://hz.guannengcc.top/gthhblzueu.html

[R45] 批量删除
来源：http://hz.shanyushiyangtech.top/gtccwixhpn.html

find . -name "*.tmp" -delete
来源：http://hz.iojbl.cn/gtxragxfas.html

[R46] 递归替换文件内容
来源：http://hz.zhiwuduotai.top/gtwommlals.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hongshengwenyu.top/gtlqwmwscy.html

[R47] sed 单行替换
来源：http://hz.xziqi.cn/gteouniuht.html


<!-- 参考信息 -->