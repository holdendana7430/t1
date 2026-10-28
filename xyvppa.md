代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtezqtsgtm.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtmsaktjzi.html

amount DECIMAL(10, 2),
来源：http://hz.zhijiandao.cn/gtlabiycfr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xinyue.icu/gtokpfunfy.html

);
来源：http://hz.yueranfly.top/gtcfntzqyz.html

[Q03] 增加列
来源：http://hz.cdnleiting.top/gtnbldvaua.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.0kj1m.cn/gtnmkczozq.html

[Q04] 修改列类型
来源：http://hz.shangyingyoupin.top/gtxdmqneln.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuanzhike.top/gtpixjyibs.html

[Q05] 重命名列
来源：http://hz.yuxming.cn/gtbkzdfahk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gzhubu.top/gtenhlmhcx.html

[Q06] 删除列
来源：http://hz.fengsongda.top/gtglsirflk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xuanzx.com/gtbqhgzgov.html

[Q07] 删除表
来源：http://hz.yuxming.cn/gttffgltmx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258.top/gtqxfdakjy.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtnggzfdqh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ybcxt.top/gtqusalkxm.html

[Q09] 创建唯一索引
来源：http://hz.aizwys.cn/gtxfvxamts.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtqzlelsqk.html

[Q10] 插入单行
来源：http://hz.yuanzhike.top/gthnxxpdbd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258.top/gtsrznnuku.html

[Q11] 一次插入多行
来源：http://hz.aibaodan.cn/gtuhzvsvum.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydjk.org.cn/gtsqczjiuz.html

[Q12] 插入后取自增 ID
来源：http://hz.nwbrower.top/gtwznhiues.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hysaishi.cn/gtholisfth.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hammf.cn/gtgtdfocna.html

[Q13] 忽略重复插入
来源：http://hz.xingfuxueyuan.xyz/gtunaidlsm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yvedp.cn/gtsuvovgxk.html

[Q14] 存在则更新（upsert）
来源：http://hz.316326.xyz/gtfelsfmfm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.bjfxy.top/gtfjsbudzx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj202588.top/gthbwjmjta.html

[Q15] 查询全部
来源：http://hz.aibaodan.cn/gtullddjjz.html

SELECT * FROM users;
来源：http://hz.xuanzx.com/gtknoykrdo.html

[Q16] 查询指定列
来源：http://hz.kuanghao11.cn/gttughsvqd.html

SELECT id, name FROM users;
来源：http://hz.jlsjyb.cn/gtyxjmtjpe.html

[Q17] 条件查询
来源：http://hz.ydjk.org.cn/gtjcqlbeef.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gogol.net.cn/gtankcwenk.html

[Q18] 模糊匹配
来源：http://hz.feifeiyinyue.top/gtsumoetgm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yongpay.top/gtkuywctea.html

[Q19] 范围查询
来源：http://hz.redwolf501.top/gtbktbsvgu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jiagoushi.top/gtjylcyaol.html

[Q20] IN 列表
来源：http://hz.jianghu66.top/gtamypksqv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shanyushiyangtech.top/gtluzpvvdg.html

[Q21] 空值判断
来源：http://hz.yuanzhike.top/gtcqxhgxfo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jqgufenzy.top/gtofttwzhk.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtnntwrgit.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuanzx.com/gtzlddebxk.html

[Q23] 分页
来源：http://hz.vqdsnc.cn/gttdcrzdwz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenzaomai.com/gtikkgixoj.html

[Q24] 去重
来源：http://hz.chenzaomai.com/gtlechchic.html

SELECT DISTINCT city FROM users;
来源：http://hz.cqqwz.cn/gtoispflhc.html

[Q25] 只取前 N 条
来源：http://hz.ivvv.top/gtskjgwhei.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ywan-chungtsiang.top/gtpjehyvdi.html

[Q26] 计数
来源：http://hz.hnqzz.top/gtqnivizop.html

SELECT COUNT(*) FROM users;
来源：http://hz.guowangkeji.top/gtfvusdeep.html

[Q27] 条件计数
来源：http://hz.jinyuanbaomall.cn/gtihvwthoh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.meibo888.top/gtclzudvdc.html

[Q28] 求和与平均
来源：http://hz.gogol.net.cn/gtybexwwff.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258.top/gtvvzchgcn.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gtowvjqciw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258888.top/gtxbjqghve.html

[Q30] 分组统计
来源：http://hz.ydzc1.top/gtbnluimkr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gttmtezxqd.html

[Q31] 分组后过滤
来源：http://hz.nwbrower.top/gthvgdobaq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhijiandao.cn/gtddnqucsb.html

[Q32] 分组拼接字符串
来源：http://hz.yj20258.top/gtmmvbeaum.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtxjpyhmcs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tian-w.cn/gthrwktxwb.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gttsfdplmb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gtdjarueut.html

[Q34] 每组取第一条
来源：http://hz.yj20258.top/gtzzzhmmqz.html

SELECT * FROM (
来源：http://hz.9152youxi.cn/gtjzlxhmxd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhiwuduotai.top/gtricarqep.html

) t WHERE rn = 1;
来源：http://hz.ydzc1.top/gtojdyldld.html

[Q35] 内连接
来源：http://hz.yangfankeji.com/gtalwqnexe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtjkecvdyd.html

[Q36] 左连接
来源：http://hz.ydzc1.top/gtmgvwgbmq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gtlxvxyumz.html

[Q37] 右连接
来源：http://hz.shuidangran.top/gtceuhreqd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtnzudlsjq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhijiandao.cn/gtmetfolkl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nwbrower.top/gtluolzsqo.html

[Q39] 自连接（查上下级）
来源：http://hz.chenzaomai.com/gtixdpeglz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xylfe.cn/gtuwqbrnyq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shuidangran.top/gtyzeftaji.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yuanzhike.top/gtwsplrptj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hysaishi.cn/gtmkiduaoc.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtbepigkxc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuetiantiany.cn/gtqommavbu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xziqi.cn/gtcpmnifrt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gtoszgaqgs.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxinkj.top/gtrksgozfz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtofqnhkjp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.quarkkingdee.top/gtvwoeonat.html

[Q43] 标量子查询
来源：http://hz.cheryme.top/gttgwlwxga.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.vqdsnc.cn/gtejzlbsbk.html

[Q44] IN 子查询
来源：http://hz.jqgfzy.top/gtjqzjcijc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtopktofzl.html

[Q45] EXISTS 判断存在
来源：http://hz.jiagoushi.top/gtkejcrkya.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gthatvgicj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigufen.top/gtkeohdoww.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gzhubu.top/gtpndzhofm.html

[Q47] 与平均值比较
来源：http://hz.shzxlz.cn/gtqhozldqt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.haohaochexian.top/gtmewbhqfp.html

[Q48] CTE 公用表表达式
来源：http://hz.yvedp.cn/gtkealoejs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sufxvd.cn/gtrafeiykc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yongpay.top/gtmqawbntv.html

[Q49] 更新单行
来源：http://hz.yj20258.top/gtraxszosw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.haohaochexian.top/gtosqlxgic.html

[Q50] 批量更新
来源：http://hz.gaohongyu789.top/gtzktqhbtx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shuidangran.top/gtxgkbdbad.html

[Q51] 用子查询更新
来源：http://hz.zhijiandao.cn/gtcwdsmcas.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sufxvd.cn/gtmyjvfdiz.html

[Q52] 删除指定行
来源：http://hz.chenjidiqi.icu/gtzumtwewe.html

DELETE FROM users WHERE id = 10;
来源：http://hz.haohaochexian.top/gthzpkyile.html

[Q53] 按条件删除
来源：http://hz.zhijiandao.cn/gtrarvkmth.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fzhhl.top/gttvyiswme.html

[Q54] 清空表
来源：http://hz.sufxvd.cn/gtegsrjzss.html

TRUNCATE TABLE logs;
来源：http://hz.pengpengdd.cyou/gtwfzrrauc.html

[Q55] 排名（并列占位）
来源：http://hz.yj20258.top/gtxcfdisce.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dianchejie.cn/gtpszxbwqs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuanzx.com/gtyikqvsjd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.meibo888.top/gtgnjitdcg.html

[Q57] 行号
来源：http://hz.hfpthk.cn/gtbxeojuwj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zycfv.cn/gtlvknypqj.html

[Q58] 累计求和
来源：http://hz.52xcode.cn/gthzbfdggm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ywan-chungtsiang.top/gthsejycxw.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtrpcwnozv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtxvatncre.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gtjykkoani.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cheryme.top/gtszgrbmhq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.vqdsnc.cn/gtkxnbjepo.html

[Q61] 移动平均
来源：http://hz.52xcode.cn/gtcttvelss.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.9152youxi.cn/gtmdbsmion.html

[Q62] 分组占比
来源：http://hz.chenlongwang.top/gtiwtowxvr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtfcpdlqox.html

[Q63] 开启事务
来源：http://hz.hnqzz.top/gtevndbxml.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuetiantiany.cn/gtvqppkxhi.html

[Q64] 提交事务
来源：http://hz.chenjidiqi.icu/gthuuxcwat.html

COMMIT;
来源：http://hz.xuanzx.com/gtpqtwuojn.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtfrymcdna.html

ROLLBACK;
来源：http://hz.zhixingplan.top/gtkdovaqqg.html

[Q66] 行锁查询
来源：http://hz.ywan-chungtsiang.top/gtsafmzvur.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangdashe.top/gtqmorebis.html

[Q67] 设置隔离级别
来源：http://hz.sufxvd.cn/gtcxmjhrna.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sufxvd.cn/gtdazyucth.html

[Q68] 保存点
来源：http://hz.jyoumei.cn/gtnsovxbkn.html

SAVEPOINT sp1;
来源：http://hz.meibo888.top/gtlytsmlyf.html

ROLLBACK TO sp1;
来源：http://hz.pengpengdd.cyou/gtwsddaath.html

[Q69] 查看执行计划
来源：http://hz.guowangkeji.top/gtdzzkmunl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangdashe.top/gtzdkrmbpr.html

[Q70] 更新统计信息
来源：http://hz.chenzaomai.com/gtgoamtjwb.html

ANALYZE TABLE users;
来源：http://hz.xinyue.icu/gtjmvvrnkk.html

[Q71] 查看建表语句
来源：http://hz.yonumen.top/gtsplzhrgu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fzhhl.top/gtqvrnwyps.html

[Q72] 查看索引
来源：http://hz.chenzaomai.com/gtbgxjdxcb.html

SHOW INDEX FROM users;
来源：http://hz.yangfankeji.com/gtwzjguwwi.html

[Q73] 查看表状态
来源：http://hz.wangshuangyany.cn/gtjlmpxjfp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jyoumei.cn/gtitayqbin.html

[Q74] 强制使用索引
来源：http://hz.ydjk.org.cn/gtgllvvbou.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenjidiqi.icu/gtqpghurlz.html

[Q75] 日期格式化
来源：http://hz.jyoumei.cn/gtyldbhibg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuanzhike.top/gtxbslfbpx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xingfuxueyuan.xyz/gtksbaiqqk.html

[Q76] 按天统计
来源：http://hz.zhiwuduotai.top/gtchbvwcue.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tianlin.xyz/gtawfokdkh.html

[Q77] 时间加减
来源：http://hz.yuanzhike.top/gtdsznvlfk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gturzjvrzt.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gtkbmrzkwp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xingfuxueyuan.xyz/gttlcoikcm.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gtrjwgsteg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jlsjyb.cn/gtqzjluevb.html

[Q80] 字符串截取
来源：http://hz.dashuyun.cn/gtoiocibnb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shzxlz.cn/gttmzyoqzh.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtbpczllut.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tanke756.top/gtfcuwwvmt.html

[Q82] 字符长度与字节长度
来源：http://hz.xziqi.cn/gtqymohdcm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yanxiufei.cn/gtganymfct.html

[Q83] 大小写转换
来源：http://hz.jqgufenzy.top/gtxcpqqfyh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258888.top/gttvdgkmhv.html

[Q84] 去除首尾空格
来源：http://hz.fzhhl.top/gtymbyksjq.html

SELECT TRIM(name) FROM users;
来源：http://hz.quarkkingdee.top/gtuibjyfui.html

[Q85] 数值取整
来源：http://hz.wangshuangyany.cn/gtxvfxdqss.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.quarkkingdee.top/gtqkhhjbpi.html

[Q86] 读取 JSON 字段
来源：http://hz.quarkkingdee.top/gtfavodyzs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhoulong.xyz/gtbqsftrxn.html

[Q87] JSON 字段做条件
来源：http://hz.snrcjt.cn/gtkkwjfstt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinyuanbaomall.cn/gtgvoeyygj.html

[Q88] 行转列（条件聚合）
来源：http://hz.gotoacloud.top/gtzokzyeol.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigfzy.top/gtvfcwwmjp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj20258888.top/gtkarshauz.html

[Q89] 判断表是否存在
来源：http://hz.guowangkeji.top/gtnruaklxm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnqzz.top/gtirxcaypf.html

[Q90] 生成序号列
来源：http://hz.pengpengdd.cyou/gtqflrnwko.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gogol.net.cn/gtrgavibhg.html

================================================================================
来源：http://hz.yangfankeji.com/gtmyavogpj.html

R. Bash 专题
来源：http://hz.havefunace.top/gtthufyuxr.html

================================================================================
来源：http://hz.gzhubu.top/gtqyekggxs.html

[R01] shebang 与严格模式
来源：http://hz.andypj.xyz/gtnbblgjtg.html

#!/usr/bin/env bash
来源：http://hz.yongpay.top/gtgmxstgsc.html

set -euo pipefail
来源：http://hz.birdmap.top/gtynqaixgg.html

[R02] 变量赋值与使用
来源：http://hz.jqgfzy.top/gttatgcfjs.html

name="Tom"; echo "$name"
来源：http://hz.sweek.top/gtvcutywjt.html

[R03] 只读变量
来源：http://hz.smart0.xyz/gtliiriwku.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtoxngjhwu.html

[R04] 位置参数
来源：http://hz.yonumen.top/gtcpsjuyiq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtiacsgiib.html

[R05] 参数默认值
来源：http://hz.zhoulong.xyz/gtmddizmtp.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtfsyuyyul.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangtech.top/gtysmtmtwq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jyoumei.cn/gtnwlzmiws.html

[R07] if 判断文件
来源：http://hz.c1oappe.top/gtbluqihvu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hongshengwenyu.top/gtmmtmhiyw.html

[R08] 数值比较
来源：http://hz.shuidangran.top/gtjfywrovm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cdnleiting.top/gtiqdeotdn.html

[R09] 字符串比较
来源：http://hz.zdqjudy.top/gterlkrnpm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinyuanbaomall.cn/gtemeytkub.html

[R10] 正则匹配
来源：http://hz.jinqigfzy.top/gtsdbvtzbx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gthuxplzxu.html

[R11] case 多分支
来源：http://hz.yj20258.top/gtrftnyvbe.html

case "$1" in
来源：http://hz.sysykeji.top/gteziywhsc.html

start) echo "启动" ;;
来源：http://hz.jiagoushi.top/gtihirqdol.html

stop)  echo "停止" ;;
来源：http://hz.ehwqpu.com/gtaeisrnwx.html

*)     echo "未知命令" ;;
来源：http://hz.xingfuxueyuan.xyz/gtzruslvzw.html

esac
来源：http://hz.cqqwz.cn/gtprannjgn.html

[R12] for 遍历文件
来源：http://hz.hnqzz.top/gtdfeiehvm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.fengsongda.top/gtztdfbbzj.html

[R13] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtmfaikjoa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhixingplan.top/gtlzohescn.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtvmophcst.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxinkj.top/gthaupknmd.html

[R15] while 逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gteparttow.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.9152youxi.cn/gttbjtcubp.html

[R16] until 等待条件
来源：http://hz.yj20258888.top/gtotgcviuw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtmjviavxe.html

[R17] 数组定义与取值
来源：http://hz.snrcjt.cn/gtkqhnldct.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guannengcc.top/gtdfifwyfd.html

[R18] 遍历数组
来源：http://hz.cheryme.top/gtdfqyazar.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.9152youxi.cn/gtfsaccmhr.html

[R19] 数组长度
来源：http://hz.nwbrower.top/gtfcinkgej.html

echo "${#arr[@]}"
来源：http://hz.zdqjudy.top/gtcdpjjlul.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtjcfcpzcb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gtutaqscac.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gttvebymit.html

echo "${#s}"
来源：http://hz.cdnleiting.top/gtgxyzhfkt.html

[R22] 截取子串
来源：http://hz.c1oappe.top/gttjczoiri.html

echo "${s:0:5}"
来源：http://hz.guannengcc.top/gtuqcdmnpi.html

[R23] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gtwogkryvx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.svipenyu.cn/gtklxwbtjx.html

[R24] 大小写转换
来源：http://hz.hnxiangtu.top/gtvtjfyueg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydzc1.top/gtzhxztxwm.html

[R25] 去后缀 / 去前缀
来源：http://hz.sweek.top/gtjgeogtcf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gtzktglpee.html

[R26] 命令替换
来源：http://hz.chenjidiqi.icu/gthpuxtrom.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtootrzjtl.html

[R27] 算术展开
来源：http://hz.chenlongwang.top/gtvzkbkfqe.html

echo $((1 + 2 * 3))
来源：http://hz.daxiang520.top/gtebplgatk.html

[R28] 浮点运算
来源：http://hz.jqgfzy.top/gtpsmjmyxa.html

echo "scale=2; 10/3" | bc
来源：http://hz.jqgfzy.top/gthqgseznk.html

[R29] 定义函数
来源：http://hz.jiagoushi.top/gtykbererl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtequvwhlm.html

[R30] 函数返回状态码
来源：http://hz.xinyue.icu/gtaeosjnca.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhoulong.xyz/gtnkzuylhd.html

[R31] 局部变量
来源：http://hz.shuidangran.top/gtkjthxppk.html

f() { local x=1; echo "$x"; }
来源：http://hz.316326.xyz/gtewqyoass.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gteuuvtubn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhongyouzk.top/gtfotuxsab.html

[R33] 捕获错误并提示行号
来源：http://hz.fengsongda.top/gttximauas.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yangfankeji.com/gtcortaglf.html

[R34] 退出时清理
来源：http://hz.dashuyun.cn/gtsgfeitse.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtzicnbncq.html

[R35] 后台执行并等待
来源：http://hz.jqgufenzy.top/gtxhcdpuwm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtxsoysipv.html

[R36] 并发执行多个任务
来源：http://hz.hywenlv.cn/gtgtbwmrfa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dianchejie.cn/gtiwluwgxg.html

[R37] 把输出赋给变量
来源：http://hz.xuetiantiany.cn/gtnsnskseq.html

files=$(ls -1)
来源：http://hz.meibo888.top/gthugbvxje.html

[R38] 管道串联
来源：http://hz.sufxvd.cn/gtggvsdhjm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtnffuajbz.html

[R39] 重定向标准输出与错误
来源：http://hz.gotoacloud.top/gtmkwcgmeo.html

cmd > out.log 2>&1
来源：http://hz.yj202588.top/gtobweieja.html

[R40] 追加写日志
来源：http://hz.guannengcc.top/gtcklsgwke.html

echo "log" >> out.log
来源：http://hz.ehwqpu.com/gtfpvjayem.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtkpthlsoj.html

cmd >/dev/null 2>&1
来源：http://hz.dianchejie.cn/gttypscpps.html

[R42] 输入重定向
来源：http://hz.52xcode.cn/gtxgwilshb.html

wc -l < a.txt
来源：http://hz.ydjk.org.cn/gtxrmpzzzm.html

[R43] 按名字查找文件
来源：http://hz.zhengqikj.top/gtwqwctqsa.html

find . -name "*.log" -type f
来源：http://hz.ydzc1.top/gtnxiomdvb.html

[R44] 按修改时间查找
来源：http://hz.xinyue.icu/gtzucxacwv.html

find . -mtime -7 -type f
来源：http://hz.jinqigfzy.top/gtabkrqnkz.html

[R45] 批量删除
来源：http://hz.c1oappe.top/gtvrhuztqq.html

find . -name "*.tmp" -delete
来源：http://hz.zhengqikj.top/gtnmwzpsvu.html

[R46] 递归替换文件内容
来源：http://hz.wangdashe.top/gtvvwuuwqh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zdqjudy.top/gtilyzikhh.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gtdxmrfiky.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinqigfzy.top/gtzpawgozf.html

[R48] awk 取指定列
来源：http://hz.jlsjyb.cn/gtvuonupwu.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtqtlepyga.html

[R49] awk 带条件
来源：http://hz.pycfn.com/gtkfahasnc.html


<!-- 参考信息 -->