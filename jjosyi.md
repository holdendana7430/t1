代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gthsvbpyjr.html

user_id INT NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtoygjrfaj.html

amount DECIMAL(10, 2),
来源：http://hz.ehwqpu.com/gtvdwoeotg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ybcxt.top/gttzelqtlp.html

);
来源：http://hz.haohaochexian.top/gthmcoqyxn.html

[Q03] 增加列
来源：http://hz.snrcjt.cn/gtjgbicmwc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gzhubu.top/gtnvxxwprl.html

[Q04] 修改列类型
来源：http://hz.gogol.net.cn/gtyubmqbkj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtnfngmudw.html

[Q05] 重命名列
来源：http://hz.hnxiangtu.top/gtltaiowjn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinqigfzy.top/gtpopfuaot.html

[Q06] 删除列
来源：http://hz.zhijiandao.cn/gtdqitakfc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.c1oappe.top/gtmhufrokn.html

[Q07] 删除表
来源：http://hz.gaohongyu789.top/gtlmxkafar.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhengqikj.top/gtoabrtgcc.html

[Q08] 创建普通索引
来源：http://hz.yanxiufei.cn/gtsounsxrq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtehrmsrdd.html

[Q09] 创建唯一索引
来源：http://hz.yvedp.cn/gtjlqtarbb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtsjtruawr.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtjodtgnay.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yvedp.cn/gtqqbfztrs.html

[Q11] 一次插入多行
来源：http://hz.aizwys.cn/gttauedrsc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gtaqdubdll.html

[Q12] 插入后取自增 ID
来源：http://hz.shuidangran.top/gtgsatxxyl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhaomingkeji.xyz/gtnvsisqdc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nwbrower.top/gtpwzvpufj.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtmxheinhc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hnqzz.top/gtfrcbdpvq.html

[Q14] 存在则更新（upsert）
来源：http://hz.bjfxy.top/gtqckpqiil.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yuanzhike.top/gtdgyrkzqr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gtgyurmhio.html

[Q15] 查询全部
来源：http://hz.dashuyun.cn/gtarjotzmu.html

SELECT * FROM users;
来源：http://hz.pycfn.com/gtgczxftzs.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gtleahbpad.html

SELECT id, name FROM users;
来源：http://hz.ehwqpu.com/gtztwzorvy.html

[Q17] 条件查询
来源：http://hz.zdqjudy.top/gttghzahak.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuxming.cn/gtfbokqdpg.html

[Q18] 模糊匹配
来源：http://hz.316326.xyz/gtskgfffmp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dianchejie.cn/gtrshhrpmt.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gteybolwxk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.pengpengdd.cyou/gtwpujbeqn.html

[Q20] IN 列表
来源：http://hz.nanxuanxn.top/gtabfortjy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.bjfxy.top/gtrjlavzoz.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gtltikuttp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cucudq.cn/gtaxpdcvrb.html

[Q22] 排序
来源：http://hz.daria6918.cn/gtfbqtdhax.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.birdmap.top/gtvulfkucy.html

[Q23] 分页
来源：http://hz.daxiang520.top/gtjtvuqagr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgfzy.top/gtvhkztmgu.html

[Q24] 去重
来源：http://hz.andypj.xyz/gtopjirkee.html

SELECT DISTINCT city FROM users;
来源：http://hz.shzxlz.cn/gtxgecodrs.html

[Q25] 只取前 N 条
来源：http://hz.tian-w.cn/gtnagyxhnk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xziqi.cn/gtgoicabrf.html

[Q26] 计数
来源：http://hz.tianlin.xyz/gtduqhlcmv.html

SELECT COUNT(*) FROM users;
来源：http://hz.cucudq.cn/gtdhwiuvdw.html

[Q27] 条件计数
来源：http://hz.meibo888.top/gtzpkmrpkp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.bjfxy.top/gtoxvzmpbo.html

[Q28] 求和与平均
来源：http://hz.316326.xyz/gtfmiuvlqe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnxiangtu.top/gtktxeftjr.html

[Q29] 最大最小值
来源：http://hz.xziqi.cn/gtflctaxcm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ywan-chungtsiang.top/gteefcxqpy.html

[Q30] 分组统计
来源：http://hz.yueranfly.top/gtyybrrnuj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtuokhrwnd.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtpvagoyqw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.birdmap.top/gtiipkovoi.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtcsdxjkxo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtdaqjwdxi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.andypj.xyz/gtzlulyrgr.html

[Q33] 多列分组
来源：http://hz.pengpengdd.cyou/gtbyccgqlf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yueranfly.top/gtuxosixfa.html

[Q34] 每组取第一条
来源：http://hz.ydzc1.top/gtvjbyuaya.html

SELECT * FROM (
来源：http://hz.316326.xyz/gtncourmda.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cucudq.cn/gtqvdimncc.html

) t WHERE rn = 1;
来源：http://hz.guowangkeji.top/gtersnzbcc.html

[Q35] 内连接
来源：http://hz.jianghu66.top/gtwcpxztee.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigufen.top/gtqdqovaqd.html

[Q36] 左连接
来源：http://hz.hongshengwenyu.top/gttxcwbvpy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gtxixdgzvw.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtqnofxjkd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gzhubu.top/gtilotqsgu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinqigfzy.top/gtiqvzsmey.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shuidangran.top/gtpjfoyqlx.html

[Q39] 自连接（查上下级）
来源：http://hz.ehwqpu.com/gtlcmwmeac.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuanzhike.top/gtoolxnzud.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.bjfxy.top/gticxxcplt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.9152youxi.cn/gtqqbwfxxr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gtcujvwjwa.html

[Q41] 多表连接
来源：http://hz.52xcode.cn/gtizghywrk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cashguo.top/gtzmzpfyqb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgfzy.top/gtidmopsdn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtnchznfqd.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gtmdhtmngm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tian-w.cn/gtzeckwgqf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tianlin.xyz/gtyqkggctd.html

[Q43] 标量子查询
来源：http://hz.zdqjudy.top/gtyoozyfyj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gogol.net.cn/gtasdsolwa.html

[Q44] IN 子查询
来源：http://hz.hfpthk.cn/gtixihnevz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.0kj1m.cn/gtzmohxwtk.html

[Q45] EXISTS 判断存在
来源：http://hz.52xcode.cn/gtwrierexc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.vqdsnc.cn/gtpkyqzsss.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtyyflaicm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtjkdcobfw.html

[Q47] 与平均值比较
来源：http://hz.ydjk.org.cn/gtqjkpowyb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhoulong.xyz/gtsfoikatx.html

[Q48] CTE 公用表表达式
来源：http://hz.zhiwuduotai.top/gthayymlup.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhixingplan.top/gtcktvujeq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sysykeji.top/gtctzsptjw.html

[Q49] 更新单行
来源：http://hz.shuidangran.top/gttwtupikn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtjxwbrpfw.html

[Q50] 批量更新
来源：http://hz.zhengqikj.top/gtasdhzzul.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pengpengdd.cyou/gtfdqaeczi.html

[Q51] 用子查询更新
来源：http://hz.jinqigufen.top/gtjtorhnjz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhiwuduotai.top/gtytkyskbi.html

[Q52] 删除指定行
来源：http://hz.ehwqpu.com/gtuelbijce.html

DELETE FROM users WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtkkcqoicd.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gtiigstosa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.havefunace.top/gtllolmxgp.html

[Q54] 清空表
来源：http://hz.svipenyu.cn/gtkmrvcspp.html

TRUNCATE TABLE logs;
来源：http://hz.ivvv.top/gtjfvokyij.html

[Q55] 排名（并列占位）
来源：http://hz.zhoulong.xyz/gtgsmtexie.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pycfn.com/gtegeaubal.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258888.top/gtnltmnbhp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.iojbl.cn/gtwjlozmxr.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gthvjoefbr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hammf.cn/gtebdqqzkg.html

[Q58] 累计求和
来源：http://hz.yuanzhike.top/gtrhacndov.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenlongwang.top/gthmnrcskp.html

[Q59] 分组内累计
来源：http://hz.fzhhl.top/gtxrumboee.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yangfankeji.com/gtwuvoizvq.html

[Q60] 取上一行 / 下一行
来源：http://hz.feifeiyinyue.top/gtqplgaxef.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ehwqpu.com/gtvfrzlkre.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yangfankeji.com/gtkeixpyaa.html

[Q61] 移动平均
来源：http://hz.zhijiandao.cn/gtxszxdrpv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yonumen.top/gtniopseyq.html

[Q62] 分组占比
来源：http://hz.hnxiangtu.top/gtnbbsuvpf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtyvfwomzq.html

[Q63] 开启事务
来源：http://hz.gogol.net.cn/gtjzvqgqph.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gaohongyu789.top/gtnryfffps.html

[Q64] 提交事务
来源：http://hz.aibaodan.cn/gthydxdbds.html

COMMIT;
来源：http://hz.9152youxi.cn/gtgvutjyms.html

[Q65] 回滚事务
来源：http://hz.ppjwa.cn/gtdhgmmgpq.html

ROLLBACK;
来源：http://hz.aibaodan.cn/gtbpiubjer.html

[Q66] 行锁查询
来源：http://hz.nanxinkj.top/gtleqnnbni.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.9152youxi.cn/gtvtonircv.html

[Q67] 设置隔离级别
来源：http://hz.chenlongwang.top/gtjhipykde.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tian-w.cn/gtzeyyvzcp.html

[Q68] 保存点
来源：http://hz.cqqwz.cn/gtmfilhzmv.html

SAVEPOINT sp1;
来源：http://hz.zdqjudy.top/gtikuisfmq.html

ROLLBACK TO sp1;
来源：http://hz.gogol.net.cn/gtqgnbmolb.html

[Q69] 查看执行计划
来源：http://hz.dianchejie.cn/gtxukqfnmi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.iojbl.cn/gtqqonqlig.html

[Q70] 更新统计信息
来源：http://hz.yongpay.top/gtddxwiovi.html

ANALYZE TABLE users;
来源：http://hz.sweek.top/gtavrtbffd.html

[Q71] 查看建表语句
来源：http://hz.ivvv.top/gtyeifdspv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dashuyun.cn/gtqbvrtkem.html

[Q72] 查看索引
来源：http://hz.yanxiufei.cn/gtprmeutun.html

SHOW INDEX FROM users;
来源：http://hz.0kj1m.cn/gthqtgnwzl.html

[Q73] 查看表状态
来源：http://hz.zhiwuduotai.top/gtvykmsqyq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtqqaaltyt.html

[Q74] 强制使用索引
来源：http://hz.quarkkingdee.top/gtxhgcdzvz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtqkdkoblu.html

[Q75] 日期格式化
来源：http://hz.dianchejie.cn/gtozowmdxj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtamafxsno.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.iojbl.cn/gtrhlmllvv.html

[Q76] 按天统计
来源：http://hz.zhixingplan.top/gtpbtcimmk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangtech.top/gtbqzkdgrx.html

[Q77] 时间加减
来源：http://hz.jqgufenzy.top/gtnvvnyhhx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jlsjyb.cn/gtpkqxptub.html

[Q78] 当前时间
来源：http://hz.chenzaomai.com/gtdoctwgmc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gtfiftgewa.html

[Q79] 字符串拼接
来源：http://hz.316326.xyz/gtvtljqjla.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jyoumei.cn/gtktinipep.html

[Q80] 字符串截取
来源：http://hz.yanxiufei.cn/gtfiiwenmy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtibtvpiih.html

[Q81] 字符串替换
来源：http://hz.cdnleiting.top/gtebskoesu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.havefunace.top/gtssrqrjee.html

[Q82] 字符长度与字节长度
来源：http://hz.tanke756.top/gtzqlnfygj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xinyue.icu/gtougjgunx.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtoxsnzyxr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnqzz.top/gtitybjvqt.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtdptydmth.html

SELECT TRIM(name) FROM users;
来源：http://hz.tanke756.top/gtcrlzhiax.html

[Q85] 数值取整
来源：http://hz.havefunace.top/gtlwfdmfeb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gotoacloud.top/gtqkaotiul.html

[Q86] 读取 JSON 字段
来源：http://hz.zhijiandao.cn/gtctrgdjjc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.svipenyu.cn/gtjdfazjhy.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtatcnvizj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhiwuduotai.top/gtiwvfaqzs.html

[Q88] 行转列（条件聚合）
来源：http://hz.dianchejie.cn/gtujmzxhyl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.aizwys.cn/gtflsxpwmg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aizwys.cn/gtyfdrxlgi.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtednrnhxf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gtgbrebkvl.html

[Q90] 生成序号列
来源：http://hz.52xcode.cn/gtalukvwjg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtybftqvrc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjrvoknhu.html

R. Bash 专题
来源：http://hz.wangshuangyany.cn/gtpylvwdoh.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtprpwywqa.html

[R01] shebang 与严格模式
来源：http://hz.zhiwuduotai.top/gtmscrjqij.html

#!/usr/bin/env bash
来源：http://hz.chenzaomai.com/gtsniegkam.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtkjunlafs.html

[R02] 变量赋值与使用
来源：http://hz.pycfn.com/gtfrdriavq.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtvkshlrcd.html

[R03] 只读变量
来源：http://hz.chenjidiqi.icu/gtyjgllsyq.html

readonly PI=3.14
来源：http://hz.sxryk.cn/gtmhqhtrsm.html

[R04] 位置参数
来源：http://hz.wangshuangyany.cn/gtghnazizg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fengsongda.top/gthszzfobx.html

[R05] 参数默认值
来源：http://hz.gotoacloud.top/gtqproanmd.html

name="${1:-default}"
来源：http://hz.bjfxy.top/gtnpbyrubw.html

[R06] 判断命令是否存在
来源：http://hz.mhx1999.top/gtqvorbtsu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxuanxn.top/gtglvprdaz.html

[R07] if 判断文件
来源：http://hz.dianchejie.cn/gtacwefhhl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jqgufenzy.top/gtjcxlttmd.html

[R08] 数值比较
来源：http://hz.chenjidiqi.icu/gtxrffrsyr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yongpay.top/gttsiwdrgu.html

[R09] 字符串比较
来源：http://hz.zhiwuduotai.top/gtoqekfxvh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cqqwz.cn/gtpqjtdred.html

[R10] 正则匹配
来源：http://hz.xingfuxueyuan.xyz/gtxtxnlcri.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.0kj1m.cn/gtarbuzedx.html

[R11] case 多分支
来源：http://hz.ehwqpu.com/gtjconqlfc.html

case "$1" in
来源：http://hz.aibaodan.cn/gtiwswcewv.html

start) echo "启动" ;;
来源：http://hz.fzhhl.top/gtimdrdufg.html

stop)  echo "停止" ;;
来源：http://hz.aizwys.cn/gtfhwndirk.html

*)     echo "未知命令" ;;
来源：http://hz.redwolf501.top/gtjhwwhpab.html

esac
来源：http://hz.yangfankeji.com/gtmcxxyamd.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtkpmvgdou.html

for f in *.txt; do echo "$f"; done
来源：http://hz.snrcjt.cn/gtrvyozone.html

[R13] for 计数循环
来源：http://hz.zhongyouzk.top/gtibpfixfy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtratqbnzc.html

[R14] C 风格 for
来源：http://hz.zdqjudy.top/gtkaqlixxk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtolnuuaxm.html

[R15] while 逐行读文件
来源：http://hz.yongpay.top/gtmysnqtfa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtbqvirkrv.html

[R16] until 等待条件
来源：http://hz.yuanzhike.top/gtqgwjgwjl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.iojbl.cn/gtuzyoednk.html

[R17] 数组定义与取值
来源：http://hz.xinyue.icu/gtjwjmbvgn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangdashe.top/gtwbmhjrro.html

[R18] 遍历数组
来源：http://hz.feifeiyinyue.top/gtqplvgtqm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtaosbtiru.html

[R19] 数组长度
来源：http://hz.dianchejie.cn/gtqwvwxqsb.html

echo "${#arr[@]}"
来源：http://hz.nwbrower.top/gtjpzqbtta.html

[R20] 关联数组（字典）
来源：http://hz.jiagoushi.top/gtrpdkijci.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shzxlz.cn/gtzbrqasnj.html

[R21] 字符串长度
来源：http://hz.yj20258888.top/gtnssmyrxx.html

echo "${#s}"
来源：http://hz.yj202588.top/gtxqzadczn.html

[R22] 截取子串
来源：http://hz.gotoacloud.top/gtmihaqfou.html

echo "${s:0:5}"
来源：http://hz.ivvv.top/gtmdrnlseh.html

[R23] 字符串替换
来源：http://hz.feifeiyinyue.top/gtwphatahg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangtech.top/gtmfbocsyk.html

[R24] 大小写转换
来源：http://hz.dashuyun.cn/gtgddntmgn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fengsongda.top/gtxgirvibf.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigfzy.top/gtvdxvjpby.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gtjyndhqhw.html

[R26] 命令替换
来源：http://hz.shanyushiyangkeji.top/gtyoejqjuq.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigufen.top/gtfreyrqla.html

[R27] 算术展开
来源：http://hz.hammf.cn/gtbxgfwogv.html

echo $((1 + 2 * 3))
来源：http://hz.xuetiantiany.cn/gtktvzerub.html

[R28] 浮点运算
来源：http://hz.jlsjyb.cn/gthgricasm.html

echo "scale=2; 10/3" | bc
来源：http://hz.shangyingyoupin.top/gtuelzxorw.html

[R29] 定义函数
来源：http://hz.snrcjt.cn/gtpkaxhkjy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.0kj1m.cn/gtberpgrfu.html

[R30] 函数返回状态码
来源：http://hz.xziqi.cn/gtnbgfucwz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtrbaxmotu.html

[R31] 局部变量
来源：http://hz.shangyingyoupin.top/gtmetmxccr.html

f() { local x=1; echo "$x"; }
来源：http://hz.52xcode.cn/gtytjzdlag.html

[R32] 参数个数校验
来源：http://hz.snrcjt.cn/gtrbtrxpqz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.vqdsnc.cn/gtcqwyzckm.html

[R33] 捕获错误并提示行号
来源：http://hz.gaohongyu789.top/gtswtkdwle.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtodpbkjwx.html

[R34] 退出时清理
来源：http://hz.yangfankeji.com/gtirclqfjw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gthfatutue.html

[R35] 后台执行并等待
来源：http://hz.sufxvd.cn/gtqzqxcsrh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guowangkeji.top/gtkdqyhdac.html

[R36] 并发执行多个任务
来源：http://hz.ydjk.org.cn/gtrjpjvatm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnqzz.top/gtaifmosez.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangkeji.top/gtavynlgfw.html

files=$(ls -1)
来源：http://hz.smart0.xyz/gtwudahlml.html

[R38] 管道串联
来源：http://hz.daria6918.cn/gtdigddaxt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxinkj.top/gtklwgtkre.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangtech.top/gtdnnacvyo.html

cmd > out.log 2>&1
来源：http://hz.ywan-chungtsiang.top/gtkgwruyab.html

[R40] 追加写日志
来源：http://hz.ivvv.top/gtzrvdpafa.html

echo "log" >> out.log
来源：http://hz.cdnleiting.top/gtgwufdcna.html

[R41] 丢弃输出
来源：http://hz.gotoacloud.top/gtquzdbxcc.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258888.top/gthfyuobil.html

[R42] 输入重定向
来源：http://hz.bjfxy.top/gtdknayzay.html

wc -l < a.txt
来源：http://hz.jiagoushi.top/gtgxqquozp.html

[R43] 按名字查找文件
来源：http://hz.guowangkeji.top/gtrjtqzwed.html

find . -name "*.log" -type f
来源：http://hz.jinqigufen.top/gtoxzpzvhd.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtthleipgt.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtlxwlkavg.html

[R45] 批量删除
来源：http://hz.316326.xyz/gthxpwmysm.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258.top/gtorbrxoly.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gtnybhklpa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhoulong.xyz/gtkjmzgnur.html

[R47] sed 单行替换
来源：http://hz.cqqwz.cn/gtndyivioo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtgzdvzbgr.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtbhseubve.html

awk '{print $1, $3}' a.txt
来源：http://hz.sweek.top/gtnvxcdwhf.html

[R49] awk 带条件
来源：http://hz.yanxiufei.cn/gtrzxgzqtz.html


<!-- 参考信息 -->