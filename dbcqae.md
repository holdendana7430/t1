代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tian-w.cn/gtnsasqiyb.html

[Q05] 重命名列
来源：http://hz.sxryk.cn/gtvpdkqjqc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj202588.top/gtizbjkcnv.html

[Q06] 删除列
来源：http://hz.jianghu66.top/gtvvqnjzwp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ywan-chungtsiang.top/gtnavslcsx.html

[Q07] 删除表
来源：http://hz.ybcxt.top/gtztddbnwb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangdashe.top/gtmmgvolnk.html

[Q08] 创建普通索引
来源：http://hz.zhaomingkeji.xyz/gtlzohiobf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.birdmap.top/gtmbaxxyqi.html

[Q09] 创建唯一索引
来源：http://hz.cdnleiting.top/gtvhnddrdp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuanzhike.top/gtlcmamxsh.html

[Q10] 插入单行
来源：http://hz.yangfankeji.com/gtkeqpuhyj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhengqikj.top/gtpijyimnq.html

[Q11] 一次插入多行
来源：http://hz.nwbrower.top/gtzaenfhsb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jqgufenzy.top/gtxonzzpop.html

[Q12] 插入后取自增 ID
来源：http://hz.andypj.xyz/gtgwlqqsmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangshuangyany.cn/gtulwqnvhd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xingfuxueyuan.xyz/gtavdcuwvm.html

[Q13] 忽略重复插入
来源：http://hz.daxiang520.top/gthbhfeqhg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gttnkarobv.html

[Q14] 存在则更新（upsert）
来源：http://hz.ydzc1.top/gtwnrqdxnf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ivvv.top/gtshoafswt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigufen.top/gtrjuvhyub.html

[Q15] 查询全部
来源：http://hz.kuanghao11.cn/gtqkugadqf.html

SELECT * FROM users;
来源：http://hz.hammf.cn/gttqxfcfqk.html

[Q16] 查询指定列
来源：http://hz.kuanghao11.cn/gtxrylmrmf.html

SELECT id, name FROM users;
来源：http://hz.hysaishi.cn/gthdsxtjdw.html

[Q17] 条件查询
来源：http://hz.pengpengdd.cyou/gtgvphvzas.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gtatpchvjv.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtnufiilqw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xingfuxueyuan.xyz/gtpjbedrpt.html

[Q19] 范围查询
来源：http://hz.mhx1999.top/gtldqwxjds.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sysykeji.top/gtwgvzybtr.html

[Q20] IN 列表
来源：http://hz.dianchejie.cn/gtbiacwmey.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yvedp.cn/gtdaxfhyyf.html

[Q21] 空值判断
来源：http://hz.gzhubu.top/gtykfzylkt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dianchejie.cn/gtedxxttty.html

[Q22] 排序
来源：http://hz.tian-w.cn/gtiggxouvo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gteoduqzeo.html

[Q23] 分页
来源：http://hz.zycfv.cn/gtuhptjdra.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cucudq.cn/gtzvtbscmu.html

[Q24] 去重
来源：http://hz.gaohongyu789.top/gttsamkqrm.html

SELECT DISTINCT city FROM users;
来源：http://hz.hammf.cn/gtawblykmo.html

[Q25] 只取前 N 条
来源：http://hz.hfpthk.cn/gtvlhbxcfd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xylfe.cn/gtkgwhikhe.html

[Q26] 计数
来源：http://hz.ivvv.top/gtnkxmyesu.html

SELECT COUNT(*) FROM users;
来源：http://hz.ehwqpu.com/gtgelmlfat.html

[Q27] 条件计数
来源：http://hz.aizwys.cn/gteomplwei.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nwbrower.top/gtzulyazyu.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangtech.top/gtpagbjqhi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnqzz.top/gtwzycqzrr.html

[Q29] 最大最小值
来源：http://hz.nanxuanxn.top/gtuhtjwnjv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxinkj.top/gthmkjrwiv.html

[Q30] 分组统计
来源：http://hz.jinyuanbaomall.cn/gtriifomcd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtyqivxtif.html

[Q31] 分组后过滤
来源：http://hz.daria6918.cn/gtooigmgal.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xinyue.icu/gtipmdeead.html

[Q32] 分组拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtyeunpyol.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtahpadyzb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnqzz.top/gtxhunhlvv.html

[Q33] 多列分组
来源：http://hz.sysykeji.top/gteximkzns.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gtaqekkyyy.html

[Q34] 每组取第一条
来源：http://hz.redwolf501.top/gteoiobxpv.html

SELECT * FROM (
来源：http://hz.gaohongyu789.top/gtlwvbrhli.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.svipenyu.cn/gtvwitwpuk.html

) t WHERE rn = 1;
来源：http://hz.vqdsnc.cn/gthqdmiura.html

[Q35] 内连接
来源：http://hz.shanyushiyangkeji.top/gtlwzpbpvw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtdynddiks.html

[Q36] 左连接
来源：http://hz.jqgufenzy.top/gtvnlprvtu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtxmmaeuvz.html

[Q37] 右连接
来源：http://hz.sufxvd.cn/gtydmbqtxd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtrtnrtite.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.dashuyun.cn/gtpgziiuxp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cdnleiting.top/gtjjfujdmx.html

[Q39] 自连接（查上下级）
来源：http://hz.pengpengdd.cyou/gtsttseped.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.52xcode.cn/gtbmybzmpd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.meibo888.top/gtufusstap.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtyrxyzseq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.bjfxy.top/gtvfzdewsh.html

[Q41] 多表连接
来源：http://hz.cashguo.top/gtjhldowmp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuanzx.com/gtllmbpanq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnqzz.top/gtbobhgfmm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jlsjyb.cn/gtiyzogphi.html

[Q42] 连接条件附加过滤
来源：http://hz.xziqi.cn/gtadpqqhce.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenzaomai.com/gtjcvnweub.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.feifeiyinyue.top/gthwiiiczo.html

[Q43] 标量子查询
来源：http://hz.vqdsnc.cn/gthkilkioo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.guowangkeji.top/gtinfqxfis.html

[Q44] IN 子查询
来源：http://hz.zhaomingkeji.xyz/gtnreiujds.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhixingplan.top/gtyjpinpff.html

[Q45] EXISTS 判断存在
来源：http://hz.zhixingplan.top/gtewwanocx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtledukjho.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hfpthk.cn/gtssatprdh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtlkzfhnra.html

[Q47] 与平均值比较
来源：http://hz.ehwqpu.com/gtaxrbudvy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhijiandao.cn/gtoklquadp.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtyxayvyix.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gtjewzhzcb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhijiandao.cn/gthcmqkdpz.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gtmwyrffpq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigufen.top/gtypwnpzhp.html

[Q50] 批量更新
来源：http://hz.0kj1m.cn/gtvczjmyxe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ywan-chungtsiang.top/gtbgxacpzb.html

[Q51] 用子查询更新
来源：http://hz.smart0.xyz/gtitkytysn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangdashe.top/gtgxkafahb.html

[Q52] 删除指定行
来源：http://hz.yj202588.top/gtskfbovss.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gaohongyu789.top/gthantqpbf.html

[Q53] 按条件删除
来源：http://hz.xuanzx.com/gtvivbmbyt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ehwqpu.com/gtamstlazg.html

[Q54] 清空表
来源：http://hz.jianghu66.top/gtwoncxbyg.html

TRUNCATE TABLE logs;
来源：http://hz.mhx1999.top/gttbfzvqcb.html

[Q55] 排名（并列占位）
来源：http://hz.yj202588.top/gtqcutbrxd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cheryme.top/gthpcbzgrd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258888.top/gtfflcgvlw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ybcxt.top/gticlmetqe.html

[Q57] 行号
来源：http://hz.9152youxi.cn/gtrgxicefs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhixingplan.top/gtlzwsrrxg.html

[Q58] 累计求和
来源：http://hz.tian-w.cn/gtihcbeviv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gttcnenjdc.html

[Q59] 分组内累计
来源：http://hz.nwbrower.top/gtkilbdzsk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sysykeji.top/gtshwwwask.html

[Q60] 取上一行 / 下一行
来源：http://hz.cqqwz.cn/gtxiusoejl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtttngwdyv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fzhhl.top/gtpjzunpgn.html

[Q61] 移动平均
来源：http://hz.yongpay.top/gtfalftukw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gtiqepoitv.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gthikyvofu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtuvnjrveo.html

[Q63] 开启事务
来源：http://hz.yj20258.top/gtayswytsu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tanke756.top/gtlmwipjba.html

[Q64] 提交事务
来源：http://hz.kuanghao11.cn/gtlqzhyzqk.html

COMMIT;
来源：http://hz.sufxvd.cn/gtupyrluwz.html

[Q65] 回滚事务
来源：http://hz.xziqi.cn/gtnfuerefd.html

ROLLBACK;
来源：http://hz.fengsongda.top/gtvxrikbfs.html

[Q66] 行锁查询
来源：http://hz.gaohongyu789.top/gttgpwcoif.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gteyeiotrh.html

[Q67] 设置隔离级别
来源：http://hz.jinqigfzy.top/gtjudhxuxv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.316326.xyz/gtwnhfzesp.html

[Q68] 保存点
来源：http://hz.yuanzhike.top/gtsdqathce.html

SAVEPOINT sp1;
来源：http://hz.hammf.cn/gthmmomezt.html

ROLLBACK TO sp1;
来源：http://hz.zhaomingkeji.xyz/gthtjpcqql.html

[Q69] 查看执行计划
来源：http://hz.sxryk.cn/gtgvlkjvzv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cucudq.cn/gtfktpcpmw.html

[Q70] 更新统计信息
来源：http://hz.aibaodan.cn/gtflhvizob.html

ANALYZE TABLE users;
来源：http://hz.tianlin.xyz/gtnkwiuqaw.html

[Q71] 查看建表语句
来源：http://hz.shuidangran.top/gtsbzlioif.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.52xcode.cn/gtodbgieap.html

[Q72] 查看索引
来源：http://hz.xuetiantiany.cn/gtsyhybsks.html

SHOW INDEX FROM users;
来源：http://hz.guannengcc.top/gtvqsibnta.html

[Q73] 查看表状态
来源：http://hz.yvedp.cn/gtnrjebvox.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.c1oappe.top/gtdlzpvsll.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gtoskttvab.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhengqikj.top/gthsidvvea.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtditmnvvb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pycfn.com/gtpeesqtrr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtydntpdhk.html

[Q76] 按天统计
来源：http://hz.sysykeji.top/gtujcthite.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.316326.xyz/gtrmrlryyk.html

[Q77] 时间加减
来源：http://hz.zdqjudy.top/gtebtmhmhl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.52xcode.cn/gtexqdgeac.html

[Q78] 当前时间
来源：http://hz.birdmap.top/gtufewxafh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aizwys.cn/gtygqlldjd.html

[Q79] 字符串拼接
来源：http://hz.smart0.xyz/gtaegmjsuu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xylfe.cn/gtkahaeoox.html

[Q80] 字符串截取
来源：http://hz.andypj.xyz/gtfsmjptfj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhengqikj.top/gtngcxlqgj.html

[Q81] 字符串替换
来源：http://hz.mhx1999.top/gtnwnjlxgv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhongyouzk.top/gtbjvunyyq.html

[Q82] 字符长度与字节长度
来源：http://hz.xinyue.icu/gtpjjoghoa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtljpeylbm.html

[Q83] 大小写转换
来源：http://hz.yuanzhike.top/gtzemikjca.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guannengcc.top/gtdcfzblub.html

[Q84] 去除首尾空格
来源：http://hz.yj20258888.top/gtxpwkbgwm.html

SELECT TRIM(name) FROM users;
来源：http://hz.meibo888.top/gtnpwslucl.html

[Q85] 数值取整
来源：http://hz.c1oappe.top/gtbstqwhpx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xziqi.cn/gtbzcjzgmn.html

[Q86] 读取 JSON 字段
来源：http://hz.gotoacloud.top/gtqtosaovz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhoulong.xyz/gtlfzcuqma.html

[Q87] JSON 字段做条件
来源：http://hz.cdnleiting.top/gthytknkhh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gtxxjnqhsf.html

[Q88] 行转列（条件聚合）
来源：http://hz.dianchejie.cn/gtlmlnkfrt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtokmfzpxr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ehwqpu.com/gtymkbnhly.html

[Q89] 判断表是否存在
来源：http://hz.redwolf501.top/gtdaqiuofv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtdugemdlz.html

[Q90] 生成序号列
来源：http://hz.gogol.net.cn/gtrgzqkgjf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.bjfxy.top/gtydvhdsvi.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqtaucruu.html

R. Bash 专题
来源：http://hz.xuetiantiany.cn/gtiyadhzkw.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsscriccc.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtmpdxokjj.html

#!/usr/bin/env bash
来源：http://hz.yj20258.top/gtpsdbynsi.html

set -euo pipefail
来源：http://hz.chenjidiqi.icu/gttxyqnpwz.html

[R02] 变量赋值与使用
来源：http://hz.chenzaomai.com/gtncoalmoo.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gtjkmyaccj.html

[R03] 只读变量
来源：http://hz.chenlongwang.top/gtwuplsqit.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtjtavifaw.html

[R04] 位置参数
来源：http://hz.jinyuanbaomall.cn/gtlwhsrsba.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtqklrmluj.html

[R05] 参数默认值
来源：http://hz.jianghu66.top/gtgeyiufqo.html

name="${1:-default}"
来源：http://hz.jyoumei.cn/gtxfftikcx.html

[R06] 判断命令是否存在
来源：http://hz.xylfe.cn/gtcrexhttd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aibaodan.cn/gtcjfvzitr.html

[R07] if 判断文件
来源：http://hz.ybcxt.top/gtonmftsns.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.snrcjt.cn/gtmxfqawsf.html

[R08] 数值比较
来源：http://hz.birdmap.top/gtkothtiwk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.quarkkingdee.top/gtjpusijdt.html

[R09] 字符串比较
来源：http://hz.hysaishi.cn/gtegicljay.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.snrcjt.cn/gtziofxxfp.html

[R10] 正则匹配
来源：http://hz.vqdsnc.cn/gtvitbsjrq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xinyue.icu/gtjbvauxec.html

[R11] case 多分支
来源：http://hz.andypj.xyz/gtdpvqtcqv.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtgtulxzxy.html

start) echo "启动" ;;
来源：http://hz.yangfankeji.com/gtdheqblov.html

stop)  echo "停止" ;;
来源：http://hz.ydjk.org.cn/gtqkvzizes.html

*)     echo "未知命令" ;;
来源：http://hz.9152youxi.cn/gtfwamwtnc.html

esac
来源：http://hz.vqdsnc.cn/gtpymsiwil.html

[R12] for 遍历文件
来源：http://hz.hysaishi.cn/gtbutoprvl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgfzy.top/gtbyjvoizt.html

[R13] for 计数循环
来源：http://hz.shanyushiyangtech.top/gttqntxnbc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yangfankeji.com/gtxlmdqrjs.html

[R14] C 风格 for
来源：http://hz.quarkkingdee.top/gtpdgugdeg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cucudq.cn/gtkvpgyuua.html

[R15] while 逐行读文件
来源：http://hz.yangfankeji.com/gthlmrhlfs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.pengpengdd.cyou/gtivoezuow.html

[R16] until 等待条件
来源：http://hz.yuxming.cn/gtydkrbzog.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gttkqeqqfb.html

[R17] 数组定义与取值
来源：http://hz.hysaishi.cn/gtgwlcggas.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuanzx.com/gtxlynksos.html

[R18] 遍历数组
来源：http://hz.mhx1999.top/gtzjqeopsn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigufen.top/gtwxjhzwfj.html

[R19] 数组长度
来源：http://hz.fzhhl.top/gtmbgkjcok.html

echo "${#arr[@]}"
来源：http://hz.ivvv.top/gtyarjowzz.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangtech.top/gtekhygijy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxuanxn.top/gtdkrvhpts.html

[R21] 字符串长度
来源：http://hz.cqqwz.cn/gtqlydajir.html

echo "${#s}"
来源：http://hz.tianlin.xyz/gtshuzpcxs.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtcicxcgkm.html

echo "${s:0:5}"
来源：http://hz.yueranfly.top/gtdksnjnxi.html

[R23] 字符串替换
来源：http://hz.shanyushiyangtech.top/gtrufblyby.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zdqjudy.top/gtyaapdith.html

[R24] 大小写转换
来源：http://hz.kuanghao11.cn/gtgtjbfstd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtmqxyzzbr.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuetiantiany.cn/gtmnppthce.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jiagoushi.top/gtbxzkmwsv.html

[R26] 命令替换
来源：http://hz.cheryme.top/gtgxtuiaba.html

now=$(date +%F); echo "$now"
来源：http://hz.ywan-chungtsiang.top/gttamqjoau.html

[R27] 算术展开
来源：http://hz.kuanghao11.cn/gtbmyhgdpe.html

echo $((1 + 2 * 3))
来源：http://hz.hywenlv.cn/gtzeqizeqt.html

[R28] 浮点运算
来源：http://hz.yj20258888.top/gtarwrgpli.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtvvgdyrgs.html

[R29] 定义函数
来源：http://hz.nanxinkj.top/gtiaewuarn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.haohaochexian.top/gtdndsbqwj.html

[R30] 函数返回状态码
来源：http://hz.jyoumei.cn/gtyouudfwu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tian-w.cn/gtkmrqagkd.html

[R31] 局部变量
来源：http://hz.tian-w.cn/gtukjtsqtz.html

f() { local x=1; echo "$x"; }
来源：http://hz.yueranfly.top/gtjpjewxjb.html

[R32] 参数个数校验
来源：http://hz.pengpengdd.cyou/gtuonpszbk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258888.top/gtytfsdpnu.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangtech.top/gthzqoabsy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gotoacloud.top/gtnrzddmtn.html

[R34] 退出时清理
来源：http://hz.hfpthk.cn/gtdbwfudgx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtfpljcgue.html

[R35] 后台执行并等待
来源：http://hz.vqdsnc.cn/gtwpishikm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhongyouzk.top/gtvgsatfpl.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtfmagotjs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenlongwang.top/gtjhxtayjf.html

[R37] 把输出赋给变量
来源：http://hz.hfpthk.cn/gtusaddryb.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gtppoigvob.html

[R38] 管道串联
来源：http://hz.hfpthk.cn/gthltyypiv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shangyingyoupin.top/gtxnrosbhg.html

[R39] 重定向标准输出与错误
来源：http://hz.gaohongyu789.top/gtpabngvrp.html

cmd > out.log 2>&1
来源：http://hz.c1oappe.top/gtzgqpgnwu.html

[R40] 追加写日志
来源：http://hz.0kj1m.cn/gtuisougby.html

echo "log" >> out.log
来源：http://hz.wangdashe.top/gtouctsvtt.html

[R41] 丢弃输出
来源：http://hz.gogol.net.cn/gtfvuuuvxn.html

cmd >/dev/null 2>&1
来源：http://hz.sysykeji.top/gtecxmwojx.html

[R42] 输入重定向
来源：http://hz.fzhhl.top/gtfogrdfwp.html

wc -l < a.txt
来源：http://hz.chenjidiqi.icu/gtntofpoma.html

[R43] 按名字查找文件
来源：http://hz.xuanzx.com/gtkdxqszir.html

find . -name "*.log" -type f
来源：http://hz.pengpengdd.cyou/gtvpqeuwqd.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gtjdztlkwn.html

find . -mtime -7 -type f
来源：http://hz.chenlongwang.top/gtxiczflei.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtxsyecmfc.html

find . -name "*.tmp" -delete
来源：http://hz.aibaodan.cn/gtuitmgkdh.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtasqyuels.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxuanxn.top/gtweuargyp.html

[R47] sed 单行替换
来源：http://hz.tanke756.top/gtflubdiqh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hysaishi.cn/gtqycnslpg.html

[R48] awk 取指定列
来源：http://hz.zdqjudy.top/gtembzlzhi.html

awk '{print $1, $3}' a.txt
来源：http://hz.kuanghao11.cn/gtpresgapj.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtsdzabxkg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guannengcc.top/gtsgcbnqlx.html

[R50] awk 求和
来源：http://hz.yanxiufei.cn/gtvuhuqgxz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenlongwang.top/gtcfbukkyd.html

[R51] 排序去重取前几
来源：http://hz.xuetiantiany.cn/gtkjbyydsv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtzyqiikzz.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gtdmwpeggl.html

wc -l a.txt
来源：http://hz.jinqigfzy.top/gtqmcblmst.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtwixoykgg.html


<!-- 参考信息 -->