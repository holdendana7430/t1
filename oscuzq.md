代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtikvoykxf.html

user_id INT NOT NULL,
来源：http://hz.yvedp.cn/gtqbqitepx.html

amount DECIMAL(10, 2),
来源：http://hz.xinyue.icu/gtwtunzxvk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.9152youxi.cn/gtiqdcehag.html

);
来源：http://hz.iojbl.cn/gthcaqobxj.html

[Q03] 增加列
来源：http://hz.zhaomingkeji.xyz/gtfldhodna.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cashguo.top/gtlcgriplc.html

[Q04] 修改列类型
来源：http://hz.ehwqpu.com/gtbhrhyyuf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhengqikj.top/gtgrmxygxl.html

[Q05] 重命名列
来源：http://hz.ppjwa.cn/gtnnrdozkd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jianghu66.top/gtcdwuccsi.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtclfvtwgc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangdashe.top/gtegixjbcz.html

[Q07] 删除表
来源：http://hz.zhongyouzk.top/gtktajdqgw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yvedp.cn/gtbvgfeqdx.html

[Q08] 创建普通索引
来源：http://hz.wangshuangyany.cn/gtidahuxoe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gturmjhogb.html

[Q09] 创建唯一索引
来源：http://hz.redwolf501.top/gtjlvdphyc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fengsongda.top/gtfdfdovlw.html

[Q10] 插入单行
来源：http://hz.meibo888.top/gtsahzmsfz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuxming.cn/gtfjsldqxa.html

[Q11] 一次插入多行
来源：http://hz.hongshengwenyu.top/gtprjhbrgy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gtpopwivsg.html

[Q12] 插入后取自增 ID
来源：http://hz.sxryk.cn/gtahwburlf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.guowangkeji.top/gtrscczuwq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.havefunace.top/gtvrqtkcco.html

[Q13] 忽略重复插入
来源：http://hz.hywenlv.cn/gtidjdwtcc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.snrcjt.cn/gtbeyktkcv.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuxming.cn/gtaditnpah.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gtdrhpoqmi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinghuilouyu.cn/gtuqxvauzf.html

[Q15] 查询全部
来源：http://hz.sufxvd.cn/gtxsnmwgul.html

SELECT * FROM users;
来源：http://hz.zhixingplan.top/gtjluaglqu.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtnkbepcio.html

SELECT id, name FROM users;
来源：http://hz.hammf.cn/gtiswtmtnu.html

[Q17] 条件查询
来源：http://hz.havefunace.top/gtonarptxf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.vqdsnc.cn/gtdiqcxpae.html

[Q18] 模糊匹配
来源：http://hz.svipenyu.cn/gtszhntgid.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtdlyhfjlq.html

[Q19] 范围查询
来源：http://hz.yangfankeji.com/gtefyancbp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gtfslsuppt.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gtpaehmhly.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gtozwphljq.html

[Q21] 空值判断
来源：http://hz.cqqwz.cn/gttfureumu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jlsjyb.cn/gtgsffshwo.html

[Q22] 排序
来源：http://hz.xinyue.icu/gtlgnugiuu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gthcaimqjk.html

[Q23] 分页
来源：http://hz.zhixingplan.top/gtfimhygkd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.svipenyu.cn/gthcwfsshn.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gtqtcieuxu.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenjidiqi.icu/gtwuhhofvp.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtaegcvveu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jianghu66.top/gtugqodaev.html

[Q26] 计数
来源：http://hz.redwolf501.top/gtcmlkhhzb.html

SELECT COUNT(*) FROM users;
来源：http://hz.svipenyu.cn/gtcbwnzlpz.html

[Q27] 条件计数
来源：http://hz.shanyushiyangkeji.top/gtptpszyhg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gotoacloud.top/gtylhwlfej.html

[Q28] 求和与平均
来源：http://hz.hnxiangtu.top/gtlchcwhgq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daxiang520.top/gtlbdawrow.html

[Q29] 最大最小值
来源：http://hz.vqdsnc.cn/gtdoidkdyy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.havefunace.top/gtyhkuhcud.html

[Q30] 分组统计
来源：http://hz.0kj1m.cn/gtqfuqybtq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtkkqjwfrn.html

[Q31] 分组后过滤
来源：http://hz.xingfuxueyuan.xyz/gtmjvchoss.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.svipenyu.cn/gthfilgyjy.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigufen.top/gtwmrjnnfy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtoqmgoqii.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shuidangran.top/gtfzxtjzbi.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtbyepztok.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yongpay.top/gtiuguvkwv.html

[Q34] 每组取第一条
来源：http://hz.316326.xyz/gttcahruwc.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtwdcpamdg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtsemndeaw.html

) t WHERE rn = 1;
来源：http://hz.aizwys.cn/gtrgihuzck.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtwwkzpgne.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtjlafwbyi.html

[Q36] 左连接
来源：http://hz.daxiang520.top/gtagsiayni.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gttcimvjoq.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtznaipesb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shangyingyoupin.top/gtittdxqyv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gttaglhqnx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cdnleiting.top/gtiggwgtzw.html

[Q39] 自连接（查上下级）
来源：http://hz.ivvv.top/gtsfxwqbep.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtslhpwjif.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jianghu66.top/gtzkumubsa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.c1oappe.top/gttvhupcqt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xylfe.cn/gtdjxkigcz.html

[Q41] 多表连接
来源：http://hz.fengsongda.top/gteolxxlbt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cdnleiting.top/gtippgdenn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinghuilouyu.cn/gtiscrxiyf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnqzz.top/gtyovzvhpa.html

[Q42] 连接条件附加过滤
来源：http://hz.zhongyouzk.top/gtekmvjnqk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.quarkkingdee.top/gtfbxujtmo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fzhhl.top/gtecrcnubh.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtyetbcfky.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangkeji.top/gtvimxnlir.html

[Q44] IN 子查询
来源：http://hz.xylfe.cn/gtarlycpoh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangkeji.top/gtuaqnydhc.html

[Q45] EXISTS 判断存在
来源：http://hz.fzhhl.top/gtaxajwmqy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtmpnwogur.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cdnleiting.top/gtyhxvppqb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gtccmdtwaf.html

[Q47] 与平均值比较
来源：http://hz.dianchejie.cn/gtoiymivnd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gogol.net.cn/gtgmxqwfsu.html

[Q48] CTE 公用表表达式
来源：http://hz.chenlongwang.top/gtlpyvmhnx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zdqjudy.top/gtgfbqnszt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtocxqjcbe.html

[Q49] 更新单行
来源：http://hz.yj20258.top/gtdcrnhore.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hysaishi.cn/gtxstdsaku.html

[Q50] 批量更新
来源：http://hz.ydjk.org.cn/gtqgmgbvmm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ydjk.org.cn/gtcmdnnyay.html

[Q51] 用子查询更新
来源：http://hz.cashguo.top/gtesppysbr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigfzy.top/gtveqmhwvh.html

[Q52] 删除指定行
来源：http://hz.dashuyun.cn/gtrhymlvbh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gtoydyqwcb.html

[Q53] 按条件删除
来源：http://hz.zycfv.cn/gtfnwfvwyb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj202588.top/gtrktpynhk.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtpxamalkn.html

TRUNCATE TABLE logs;
来源：http://hz.chenzaomai.com/gtmnfgrubk.html

[Q55] 排名（并列占位）
来源：http://hz.yuxming.cn/gtqcyzqqld.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydzc1.top/gtcvsjmeyg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gzhubu.top/gtastessqb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.redwolf501.top/gtifozhyje.html

[Q57] 行号
来源：http://hz.sysykeji.top/gtkovafdyq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xinyue.icu/gtqiwsrcvx.html

[Q58] 累计求和
来源：http://hz.birdmap.top/gtgrrpgsgm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtvvulwrko.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gtkebzyrey.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sysykeji.top/gttahimnsj.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtqtkhbolq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jiagoushi.top/gtpjiiopmu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fengsongda.top/gtpqbkrmmc.html

[Q61] 移动平均
来源：http://hz.gotoacloud.top/gtzwwdoeyi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gthbowtrjy.html

[Q62] 分组占比
来源：http://hz.cqqwz.cn/gtrqqyljsg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtcaxcsnzd.html

[Q63] 开启事务
来源：http://hz.mhx1999.top/gtfwjtraei.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtbkkqftru.html

[Q64] 提交事务
来源：http://hz.jqgfzy.top/gtfbleykhj.html

COMMIT;
来源：http://hz.bjfxy.top/gtnhgsgqcz.html

[Q65] 回滚事务
来源：http://hz.dianchejie.cn/gtuttfpkcf.html

ROLLBACK;
来源：http://hz.xinyue.icu/gtbrmtyhek.html

[Q66] 行锁查询
来源：http://hz.jinqigfzy.top/gtacnyhkym.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gtxmnhawgp.html

[Q67] 设置隔离级别
来源：http://hz.xylfe.cn/gtaukomvbx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xinyue.icu/gttujvoeeq.html

[Q68] 保存点
来源：http://hz.hfpthk.cn/gtbpjpbzfe.html

SAVEPOINT sp1;
来源：http://hz.wangdashe.top/gthicnykym.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gttwniloho.html

[Q69] 查看执行计划
来源：http://hz.yuanzhike.top/gtmvpvfosq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jianghu66.top/gtgdhkykhq.html

[Q70] 更新统计信息
来源：http://hz.havefunace.top/gtvwudujtu.html

ANALYZE TABLE users;
来源：http://hz.shuidangran.top/gtchixhkve.html

[Q71] 查看建表语句
来源：http://hz.ppjwa.cn/gtreblgzsj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtrcjjrmgb.html

[Q72] 查看索引
来源：http://hz.shanyushiyangkeji.top/gtofpkdoxw.html

SHOW INDEX FROM users;
来源：http://hz.fzhhl.top/gthfnogpaf.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gthtpouwvy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgfzy.top/gtgjgvjeko.html

[Q74] 强制使用索引
来源：http://hz.cucudq.cn/gtxosuvild.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.birdmap.top/gtbxtdljit.html

[Q75] 日期格式化
来源：http://hz.jianghu66.top/gtpkxnvyre.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hywenlv.cn/gtkjtcnpgi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gzhubu.top/gtgtawzutf.html

[Q76] 按天统计
来源：http://hz.chenlongwang.top/gtgnjzsszl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hysaishi.cn/gtcfvzceed.html

[Q77] 时间加减
来源：http://hz.jqgufenzy.top/gtsasdajvo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.0kj1m.cn/gtmwpzgkga.html

[Q78] 当前时间
来源：http://hz.nanxuanxn.top/gtdlyizktd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zdqjudy.top/gttcjhceal.html

[Q79] 字符串拼接
来源：http://hz.sweek.top/gthdvjkhut.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenjidiqi.icu/gtirzzwkle.html

[Q80] 字符串截取
来源：http://hz.cheryme.top/gtyqqhdaue.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.52xcode.cn/gtmnyxfxcr.html

[Q81] 字符串替换
来源：http://hz.smart0.xyz/gtkeiacqao.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tian-w.cn/gtgtujbjcv.html

[Q82] 字符长度与字节长度
来源：http://hz.jinghuilouyu.cn/gtyfswkaez.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydzc1.top/gtclsjkvzn.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtzroxqkbv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.meibo888.top/gtwcozggwj.html

[Q84] 去除首尾空格
来源：http://hz.jlsjyb.cn/gtbfnmydfi.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtisstmacf.html

[Q85] 数值取整
来源：http://hz.jinghuilouyu.cn/gtqhygneqg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jianghu66.top/gtlokoufqy.html

[Q86] 读取 JSON 字段
来源：http://hz.zhongyouzk.top/gtmgjmxnke.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj202588.top/gtbbtxgicc.html

[Q87] JSON 字段做条件
来源：http://hz.tanke756.top/gtjhdcbppu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cheryme.top/gtlyfwwlyx.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydjk.org.cn/gtyyrbxqdg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.9152youxi.cn/gtorbgotbx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ehwqpu.com/gtrdwsjphr.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtwkuqjrsq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtjiixydiv.html

[Q90] 生成序号列
来源：http://hz.jianghu66.top/gtvupcyqgj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtvikogbbs.html

================================================================================
来源：http://hz.andypj.xyz/gttshzdoyg.html

R. Bash 专题
来源：http://hz.dashuyun.cn/gtmfghsixk.html

================================================================================
来源：http://hz.shzxlz.cn/gtssegzfoy.html

[R01] shebang 与严格模式
来源：http://hz.zhiwuduotai.top/gtjacymbxx.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtxxiifbra.html

set -euo pipefail
来源：http://hz.snrcjt.cn/gtnpzrdxmv.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangkeji.top/gtysscbmsf.html

name="Tom"; echo "$name"
来源：http://hz.zhongyouzk.top/gtqnlhgnkc.html

[R03] 只读变量
来源：http://hz.fengsongda.top/gtbjizwvjt.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gtadzssikm.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gtnfadneaz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gzhubu.top/gthlwisldu.html

[R05] 参数默认值
来源：http://hz.yueranfly.top/gtypcqehwf.html

name="${1:-default}"
来源：http://hz.guowangkeji.top/gtrtiknlyc.html

[R06] 判断命令是否存在
来源：http://hz.aibaodan.cn/gtqpvepktt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pengpengdd.cyou/gtvhuefmsa.html

[R07] if 判断文件
来源：http://hz.tianlin.xyz/gtfkuyprot.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.snrcjt.cn/gttpcuxaxb.html

[R08] 数值比较
来源：http://hz.zhongyouzk.top/gthfvuytnr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.mhx1999.top/gtnqmqhqzn.html

[R09] 字符串比较
来源：http://hz.yj20258888.top/gtsyvrxwdy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sysykeji.top/gtxuappdbr.html

[R10] 正则匹配
来源：http://hz.zhixingplan.top/gtilgwcqqa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tianlin.xyz/gtkfrtqduz.html

[R11] case 多分支
来源：http://hz.ydzc1.top/gthxovqdym.html

case "$1" in
来源：http://hz.hysaishi.cn/gtogbwjofi.html

start) echo "启动" ;;
来源：http://hz.ydzc1.top/gtpzarnedj.html

stop)  echo "停止" ;;
来源：http://hz.yonumen.top/gtsjtysbca.html

*)     echo "未知命令" ;;
来源：http://hz.xylfe.cn/gthggjacyn.html

esac
来源：http://hz.haohaochexian.top/gtruaazjgt.html

[R12] for 遍历文件
来源：http://hz.jinyuanbaomall.cn/gtgypiycjs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cashguo.top/gtfjhnjcok.html

[R13] for 计数循环
来源：http://hz.cqqwz.cn/gtulxdmysz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tian-w.cn/gtacgllnns.html

[R14] C 风格 for
来源：http://hz.hfpthk.cn/gtwudtqcmk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtfrryxoyk.html

[R15] while 逐行读文件
来源：http://hz.jinqigufen.top/gtfljtjfiq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtubmviswp.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtqqmxupda.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtuvbdryxp.html

[R17] 数组定义与取值
来源：http://hz.yj20258888.top/gttqbybwbl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhiwuduotai.top/gtqjpsxlaz.html

[R18] 遍历数组
来源：http://hz.aizwys.cn/gtmemrolhr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ehwqpu.com/gtkkdxrmod.html

[R19] 数组长度
来源：http://hz.0kj1m.cn/gtjzacgyod.html

echo "${#arr[@]}"
来源：http://hz.shuidangran.top/gtxgjscwve.html

[R20] 关联数组（字典）
来源：http://hz.svipenyu.cn/gtyoltrrpg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gzhubu.top/gtpvsqecnf.html

[R21] 字符串长度
来源：http://hz.daria6918.cn/gtmwddlduc.html

echo "${#s}"
来源：http://hz.shuidangran.top/gtpltxzqjp.html

[R22] 截取子串
来源：http://hz.meibo888.top/gthyllscus.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gtoeophwrf.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtnbuampbr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhaomingkeji.xyz/gtmvhmtizb.html

[R24] 大小写转换
来源：http://hz.wangshuangyany.cn/gtkkwgyhrg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.andypj.xyz/gtslwrdbms.html

[R25] 去后缀 / 去前缀
来源：http://hz.c1oappe.top/gtorkzwvwn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cashguo.top/gtkxqbmqnl.html

[R26] 命令替换
来源：http://hz.andypj.xyz/gttpvktojn.html

now=$(date +%F); echo "$now"
来源：http://hz.ywan-chungtsiang.top/gtsvwrajlw.html

[R27] 算术展开
来源：http://hz.hysaishi.cn/gtayqjbsop.html

echo $((1 + 2 * 3))
来源：http://hz.yuxming.cn/gtputeuiff.html

[R28] 浮点运算
来源：http://hz.zhengqikj.top/gtjmpnmizx.html

echo "scale=2; 10/3" | bc
来源：http://hz.shangyingyoupin.top/gtnpwirkvc.html

[R29] 定义函数
来源：http://hz.yangfankeji.com/gtrirambso.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.pycfn.com/gtolzrutkm.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtfloymxsy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuetiantiany.cn/gthgkqxgly.html

[R31] 局部变量
来源：http://hz.cdnleiting.top/gtxtjjshkz.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgfzy.top/gtbyhycvdo.html

[R32] 参数个数校验
来源：http://hz.aizwys.cn/gtymbzhmzh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shuidangran.top/gtttmpxzdr.html

[R33] 捕获错误并提示行号
来源：http://hz.bjfxy.top/gtnnrixtid.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhixingplan.top/gtddwynjlo.html

[R34] 退出时清理
来源：http://hz.hnqzz.top/gtzowjctam.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtxdysjugx.html

[R35] 后台执行并等待
来源：http://hz.jlsjyb.cn/gtdqqebyal.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hammf.cn/gtknfknbml.html

[R36] 并发执行多个任务
来源：http://hz.vqdsnc.cn/gthabmxfdf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnxiangtu.top/gtohiawxsq.html

[R37] 把输出赋给变量
来源：http://hz.sufxvd.cn/gtjlkksvbv.html

files=$(ls -1)
来源：http://hz.316326.xyz/gtzdxrgvxv.html

[R38] 管道串联
来源：http://hz.dianchejie.cn/gtzdagzvuq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dianchejie.cn/gtombtfljc.html

[R39] 重定向标准输出与错误
来源：http://hz.yueranfly.top/gtzwjckzgx.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangkeji.top/gtuaofambk.html

[R40] 追加写日志
来源：http://hz.jinqigfzy.top/gttsgysxip.html

echo "log" >> out.log
来源：http://hz.jiagoushi.top/gtpjmcgnug.html

[R41] 丢弃输出
来源：http://hz.c1oappe.top/gtiikzlqsi.html

cmd >/dev/null 2>&1
来源：http://hz.cucudq.cn/gtbupmxngk.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gtgdheggtp.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtnsoimszc.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gtbirvjxdk.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gtgcihpftr.html

[R44] 按修改时间查找
来源：http://hz.jianghu66.top/gtaabnqjiy.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtnwdjqdpq.html

[R45] 批量删除
来源：http://hz.yuanzhike.top/gtbcsogkjh.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtmgfkmvzi.html

[R46] 递归替换文件内容
来源：http://hz.zhoulong.xyz/gtrfwnpffp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.vqdsnc.cn/gtdzmydyal.html

[R47] sed 单行替换
来源：http://hz.yueranfly.top/gtacqlcvpz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenzaomai.com/gtkhytebpo.html

[R48] awk 取指定列
来源：http://hz.dianchejie.cn/gtuuetbtpg.html

awk '{print $1, $3}' a.txt
来源：http://hz.cdnleiting.top/gtkvbijawt.html

[R49] awk 带条件
来源：http://hz.ivvv.top/gttlpiaqxk.html


<!-- 参考信息 -->