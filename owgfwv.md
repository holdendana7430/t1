代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shuidangran.top/gtgopyqxas.html

[Q09] 创建唯一索引
来源：http://hz.birdmap.top/gtccyqaneg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtgosnsmru.html

[Q10] 插入单行
来源：http://hz.jqgfzy.top/gtdmjzlqyi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jyoumei.cn/gthcrutozp.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gtjpeyglxc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtgezxpmjw.html

[Q12] 插入后取自增 ID
来源：http://hz.pycfn.com/gtfvwwvcks.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hywenlv.cn/gtxecktnyp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.svipenyu.cn/gtqercogcc.html

[Q13] 忽略重复插入
来源：http://hz.sysykeji.top/gtzaonsxyp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gtbbcuaacd.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gtgxtykouw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cashguo.top/gtvpqgqgzx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhiwuduotai.top/gtuuyjurty.html

[Q15] 查询全部
来源：http://hz.xinyue.icu/gteyaicdxg.html

SELECT * FROM users;
来源：http://hz.tian-w.cn/gthyhcsmiu.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gtsticrguq.html

SELECT id, name FROM users;
来源：http://hz.aizwys.cn/gtbwlyudvs.html

[Q17] 条件查询
来源：http://hz.yongpay.top/gtczfsvvee.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zdqjudy.top/gtcvxkgkac.html

[Q18] 模糊匹配
来源：http://hz.hfpthk.cn/gtpejzgjwl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.9152youxi.cn/gtwkuvfafk.html

[Q19] 范围查询
来源：http://hz.jqgufenzy.top/gtdujehlad.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj202588.top/gtmmacitox.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gtntadvtob.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.c1oappe.top/gtdnhfenqz.html

[Q21] 空值判断
来源：http://hz.daxiang520.top/gtuqgubwts.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shzxlz.cn/gteblqvaot.html

[Q22] 排序
来源：http://hz.tanke756.top/gtapktqmzs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj202588.top/gtlsqkqazv.html

[Q23] 分页
来源：http://hz.yangfankeji.com/gtewvaekwx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhongyouzk.top/gtqhxamnmr.html

[Q24] 去重
来源：http://hz.xinyue.icu/gtcjkwrlhe.html

SELECT DISTINCT city FROM users;
来源：http://hz.aibaodan.cn/gtykctvgwr.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtwbcahhae.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tanke756.top/gtmoqojbkf.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtaldeztnk.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangtech.top/gtjhgsocbo.html

[Q27] 条件计数
来源：http://hz.sysykeji.top/gttvodfgix.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxinkj.top/gtphlehwvb.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtuqmhbzyt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenlongwang.top/gtcpyihdif.html

[Q29] 最大最小值
来源：http://hz.xingfuxueyuan.xyz/gtpowovyek.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.bjfxy.top/gtsrolcjea.html

[Q30] 分组统计
来源：http://hz.gzhubu.top/gtkpbmvejc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gturbaebeu.html

[Q31] 分组后过滤
来源：http://hz.cashguo.top/gtksrsqexn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ehwqpu.com/gtssqxzhhe.html

[Q32] 分组拼接字符串
来源：http://hz.xziqi.cn/gtujvboucy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtsiajlqkl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.vqdsnc.cn/gtobzgnziu.html

[Q33] 多列分组
来源：http://hz.zhijiandao.cn/gtenhsmdpi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ehwqpu.com/gtuefqdirp.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtwejnkxsk.html

SELECT * FROM (
来源：http://hz.andypj.xyz/gtzssemovm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.pycfn.com/gtsrwjgvok.html

) t WHERE rn = 1;
来源：http://hz.xylfe.cn/gtwkvvdpxq.html

[Q35] 内连接
来源：http://hz.vqdsnc.cn/gtlzdmvzga.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtukdphsbf.html

[Q36] 左连接
来源：http://hz.jinyuanbaomall.cn/gtzvfgcilo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gthqkpgcpy.html

[Q37] 右连接
来源：http://hz.jinqigufen.top/gtrdszcnwx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.316326.xyz/gtzvdmgzmt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sxryk.cn/gtqeuysmak.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.redwolf501.top/gtozwmovgk.html

[Q39] 自连接（查上下级）
来源：http://hz.hongshengwenyu.top/gttvwjzage.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jiagoushi.top/gtnrzdfdba.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtjyuthzwe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.quarkkingdee.top/gtpjxsdylj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zycfv.cn/gtxjgqilaf.html

[Q41] 多表连接
来源：http://hz.daria6918.cn/gtrrtdzawk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guannengcc.top/gtlsxdnmkw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jyoumei.cn/gtsueaezyw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenzaomai.com/gttotqhbnk.html

[Q42] 连接条件附加过滤
来源：http://hz.svipenyu.cn/gtbnokxsgb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.guannengcc.top/gtexjpbjtj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gzhubu.top/gtisvlwbkk.html

[Q43] 标量子查询
来源：http://hz.xuanzx.com/gtzzyuhdtv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jianghu66.top/gtrkcbjyhd.html

[Q44] IN 子查询
来源：http://hz.iojbl.cn/gtiyjifecm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydjk.org.cn/gtcinhiesu.html

[Q45] EXISTS 判断存在
来源：http://hz.chenjidiqi.icu/gtdxgvnobp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtizuouhkt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.andypj.xyz/gtqxbedieq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtjerrxape.html

[Q47] 与平均值比较
来源：http://hz.xziqi.cn/gtjbukivvc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydjk.org.cn/gtmuqwzezp.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtquacqzgj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gaohongyu789.top/gtbweqdavf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shanyushiyangtech.top/gtedceqfqg.html

[Q49] 更新单行
来源：http://hz.xuanzx.com/gtsekpctir.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxinkj.top/gtnmhvvusx.html

[Q50] 批量更新
来源：http://hz.aibaodan.cn/gtdvdskhhd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtxsghbbbs.html

[Q51] 用子查询更新
来源：http://hz.zhoulong.xyz/gtioihcbiy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhoulong.xyz/gtavienbgn.html

[Q52] 删除指定行
来源：http://hz.mhx1999.top/gtgtjdxdjt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cucudq.cn/gtoqmhgomv.html

[Q53] 按条件删除
来源：http://hz.hnxiangtu.top/gteoxcaobn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.birdmap.top/gtulltgldd.html

[Q54] 清空表
来源：http://hz.shangyingyoupin.top/gttszpudqn.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258888.top/gttjccrjzt.html

[Q55] 排名（并列占位）
来源：http://hz.cashguo.top/gtvgqzdfkn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gtnrrbopoc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cheryme.top/gtdkyjekta.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.quarkkingdee.top/gtrlwqwmda.html

[Q57] 行号
来源：http://hz.zhengqikj.top/gtoebdbwxi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnqzz.top/gtxfazijqn.html

[Q58] 累计求和
来源：http://hz.yonumen.top/gtmiewkirh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jyoumei.cn/gtyqadmtpk.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtdlkdtmtx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nwbrower.top/gthtuviywd.html

[Q60] 取上一行 / 下一行
来源：http://hz.guowangkeji.top/gtpkjgrdyj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fzhhl.top/gtlmndsvqe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtotucizyy.html

[Q61] 移动平均
来源：http://hz.bjfxy.top/gtttqrftcm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.0kj1m.cn/gticprgtts.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gtylmgtsrq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtqheerraz.html

[Q63] 开启事务
来源：http://hz.quarkkingdee.top/gtpgwmyidk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gtocqymsrg.html

[Q64] 提交事务
来源：http://hz.sysykeji.top/gtgygzbmde.html

COMMIT;
来源：http://hz.zhoulong.xyz/gtewpvabpc.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtmpshmwnv.html

ROLLBACK;
来源：http://hz.shanyushiyangtech.top/gttvmoeqcd.html

[Q66] 行锁查询
来源：http://hz.gogol.net.cn/gtzqvprcbo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.meibo888.top/gtvpcbnhao.html

[Q67] 设置隔离级别
来源：http://hz.jinghuilouyu.cn/gthkgbigbq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.bjfxy.top/gtidvkfuuu.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtytjfehtf.html

SAVEPOINT sp1;
来源：http://hz.fengsongda.top/gtedpipkxs.html

ROLLBACK TO sp1;
来源：http://hz.mhx1999.top/gtocavjwqu.html

[Q69] 查看执行计划
来源：http://hz.hnqzz.top/gthqvosoot.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinghuilouyu.cn/gtwoundwyf.html

[Q70] 更新统计信息
来源：http://hz.meibo888.top/gttpuuzgfp.html

ANALYZE TABLE users;
来源：http://hz.aibaodan.cn/gtckzoqath.html

[Q71] 查看建表语句
来源：http://hz.shangyingyoupin.top/gthcpffxcb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuetiantiany.cn/gtajaroafl.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gttxandmbp.html

SHOW INDEX FROM users;
来源：http://hz.jinqigufen.top/gtiwblmtts.html

[Q73] 查看表状态
来源：http://hz.ydzc1.top/gtscqdijoe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenzaomai.com/gtrkoqhvcp.html

[Q74] 强制使用索引
来源：http://hz.hywenlv.cn/gtskiqhaxr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtstfcrjif.html

[Q75] 日期格式化
来源：http://hz.zhongyouzk.top/gtwylxmzsq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtmlsbzupr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sweek.top/gtvgvksigf.html

[Q76] 按天统计
来源：http://hz.xuanzx.com/gtatngenpi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yueranfly.top/gtoonqvqij.html

[Q77] 时间加减
来源：http://hz.zdqjudy.top/gtamhhadxx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtnvpwolxg.html

[Q78] 当前时间
来源：http://hz.guowangkeji.top/gtpngymisv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangshuangyany.cn/gtsvlthezv.html

[Q79] 字符串拼接
来源：http://hz.sysykeji.top/gtzuximqqn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xuanzx.com/gtgzkppmij.html

[Q80] 字符串截取
来源：http://hz.jinqigfzy.top/gtmgjcvlnn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guannengcc.top/gtjtlxfgjh.html

[Q81] 字符串替换
来源：http://hz.yanxiufei.cn/gtejqshorq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinghuilouyu.cn/gtctqydxyu.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gttmxpzxnq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sxryk.cn/gtyqzxdyjh.html

[Q83] 大小写转换
来源：http://hz.nanxuanxn.top/gtqelyfkfz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fzhhl.top/gtgjvqmuwc.html

[Q84] 去除首尾空格
来源：http://hz.yj20258.top/gtvbpogaen.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtyzwyedmt.html

[Q85] 数值取整
来源：http://hz.zhaomingkeji.xyz/gtopsuzjlz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgufenzy.top/gtmlgiaglo.html

[Q86] 读取 JSON 字段
来源：http://hz.redwolf501.top/gtpaandfbp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ydzc1.top/gtripxvach.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtibicbkwc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinyuanbaomall.cn/gttudlfrwy.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhongyouzk.top/gtfmcdfsod.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gogol.net.cn/gttzugfgat.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sysykeji.top/gtithnknim.html

[Q89] 判断表是否存在
来源：http://hz.gotoacloud.top/gtheiugmci.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cqqwz.cn/gtiujjjtvm.html

[Q90] 生成序号列
来源：http://hz.sufxvd.cn/gtszoeuoxy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cqqwz.cn/gtwfkeywhb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtorwjvniy.html

R. Bash 专题
来源：http://hz.pengpengdd.cyou/gtekwpwgyt.html

================================================================================
来源：http://hz.jianghu66.top/gtygocdmrz.html

[R01] shebang 与严格模式
来源：http://hz.redwolf501.top/gthlnhhain.html

#!/usr/bin/env bash
来源：http://hz.9152youxi.cn/gtgepzsnzf.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gtpytijoum.html

[R02] 变量赋值与使用
来源：http://hz.vqdsnc.cn/gtrshlpeak.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtlmousoag.html

[R03] 只读变量
来源：http://hz.sufxvd.cn/gtsuetkmsp.html

readonly PI=3.14
来源：http://hz.tian-w.cn/gtmhjqxkna.html

[R04] 位置参数
来源：http://hz.xziqi.cn/gttvvvmbhl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jiagoushi.top/gtllswiehp.html

[R05] 参数默认值
来源：http://hz.chenjidiqi.icu/gtizsasrwx.html

name="${1:-default}"
来源：http://hz.nanxinkj.top/gtcxzlvwcp.html

[R06] 判断命令是否存在
来源：http://hz.c1oappe.top/gtzvgfsnar.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.snrcjt.cn/gtkqearbjt.html

[R07] if 判断文件
来源：http://hz.ywan-chungtsiang.top/gtlpkiirqc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shzxlz.cn/gtmbgpplgn.html

[R08] 数值比较
来源：http://hz.andypj.xyz/gtilzuetbz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tanke756.top/gtqersakmk.html

[R09] 字符串比较
来源：http://hz.nwbrower.top/gtujyrdsek.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tianlin.xyz/gtijqipuwy.html

[R10] 正则匹配
来源：http://hz.haohaochexian.top/gtgpnkciub.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenlongwang.top/gtteufuwub.html

[R11] case 多分支
来源：http://hz.jinghuilouyu.cn/gtorgshbto.html

case "$1" in
来源：http://hz.ybcxt.top/gtmtoxjvkc.html

start) echo "启动" ;;
来源：http://hz.jiagoushi.top/gtnwqgvpmr.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtbdxvaxeq.html

*)     echo "未知命令" ;;
来源：http://hz.smart0.xyz/gtqtlzjklw.html

esac
来源：http://hz.gogol.net.cn/gtjejzlzik.html

[R12] for 遍历文件
来源：http://hz.yanxiufei.cn/gtmzpinpro.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydzc1.top/gttapblzmx.html

[R13] for 计数循环
来源：http://hz.svipenyu.cn/gtybsacwrg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gthvfyxgnt.html

[R14] C 风格 for
来源：http://hz.ehwqpu.com/gtpxlbrlvk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ppjwa.cn/gtyocezeei.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtasmafxox.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sufxvd.cn/gtglhnadmv.html

[R16] until 等待条件
来源：http://hz.yuxming.cn/gtvfaqvdbw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gtwbvawscf.html

[R17] 数组定义与取值
来源：http://hz.cashguo.top/gtqbllxvsk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hammf.cn/gtgnxiwxac.html

[R18] 遍历数组
来源：http://hz.jianghu66.top/gtqzsmfvxa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xziqi.cn/gtlcngijmt.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtwxnboqno.html

echo "${#arr[@]}"
来源：http://hz.ydjk.org.cn/gtganjnnun.html

[R20] 关联数组（字典）
来源：http://hz.dianchejie.cn/gtqwwbvdcq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tian-w.cn/gtyqfeqnww.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtkfoastlr.html

echo "${#s}"
来源：http://hz.zdqjudy.top/gtziinuvls.html

[R22] 截取子串
来源：http://hz.xingfuxueyuan.xyz/gtebefmvni.html

echo "${s:0:5}"
来源：http://hz.zdqjudy.top/gtxebjxywt.html

[R23] 字符串替换
来源：http://hz.yuanzhike.top/gtafcdrxvp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.andypj.xyz/gtconjfaag.html

[R24] 大小写转换
来源：http://hz.zhengqikj.top/gtzvmtbylo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fengsongda.top/gtphwjtyca.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtpijpeojq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnxiangtu.top/gtyvzdglyz.html

[R26] 命令替换
来源：http://hz.fzhhl.top/gtqhqsuaor.html

now=$(date +%F); echo "$now"
来源：http://hz.yonumen.top/gtcdeqzxgb.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtpoppdtxm.html

echo $((1 + 2 * 3))
来源：http://hz.jqgufenzy.top/gtexxixeaf.html

[R28] 浮点运算
来源：http://hz.yongpay.top/gttsrbjrsq.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinqigfzy.top/gtcfmrusec.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtsfoabosw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gttbjosfao.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtdrkekdvb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtvwokwtlm.html

[R31] 局部变量
来源：http://hz.jlsjyb.cn/gtxqdadmak.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj202588.top/gtucpvbbsv.html

[R32] 参数个数校验
来源：http://hz.zdqjudy.top/gtrrwdydfm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jianghu66.top/gtoxpwlwal.html

[R33] 捕获错误并提示行号
来源：http://hz.ivvv.top/gtolgzjeyz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dianchejie.cn/gtnauzveqx.html

[R34] 退出时清理
来源：http://hz.9152youxi.cn/gtiqkurhkp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtiowlvjmt.html

[R35] 后台执行并等待
来源：http://hz.yj20258.top/gtmscihjgr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtvespgtlw.html

[R36] 并发执行多个任务
来源：http://hz.tian-w.cn/gtuuwvjudo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xingfuxueyuan.xyz/gtazifgxli.html

[R37] 把输出赋给变量
来源：http://hz.dashuyun.cn/gtrwmekkml.html

files=$(ls -1)
来源：http://hz.cheryme.top/gtrivefqom.html

[R38] 管道串联
来源：http://hz.mhx1999.top/gtsnlfbyek.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhaomingkeji.xyz/gtwtxspuvr.html

[R39] 重定向标准输出与错误
来源：http://hz.wangdashe.top/gtwipvrisj.html

cmd > out.log 2>&1
来源：http://hz.c1oappe.top/gthwjiwfng.html

[R40] 追加写日志
来源：http://hz.ydjk.org.cn/gtpcjxfsfu.html

echo "log" >> out.log
来源：http://hz.yj20258.top/gtgfhnfrwj.html

[R41] 丢弃输出
来源：http://hz.quarkkingdee.top/gtxecnjile.html

cmd >/dev/null 2>&1
来源：http://hz.smart0.xyz/gtinamomsx.html

[R42] 输入重定向
来源：http://hz.xuetiantiany.cn/gtkwqlbhwm.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtwnflqbbx.html

[R43] 按名字查找文件
来源：http://hz.snrcjt.cn/gtmlbwmtpc.html

find . -name "*.log" -type f
来源：http://hz.jinqigufen.top/gtnibzfkbz.html

[R44] 按修改时间查找
来源：http://hz.smart0.xyz/gtgfobeilq.html

find . -mtime -7 -type f
来源：http://hz.chenzaomai.com/gthnvzstuv.html

[R45] 批量删除
来源：http://hz.xinyue.icu/gtooovukst.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigfzy.top/gtxfnuxizc.html

[R46] 递归替换文件内容
来源：http://hz.9152youxi.cn/gtxkbvapcz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guannengcc.top/gtfuljowsj.html

[R47] sed 单行替换
来源：http://hz.ybcxt.top/gtyzmupute.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gtnbboehye.html

[R48] awk 取指定列
来源：http://hz.yonumen.top/gtdunvdefq.html

awk '{print $1, $3}' a.txt
来源：http://hz.jlsjyb.cn/gtkadxhzff.html

[R49] awk 带条件
来源：http://hz.zhongyouzk.top/gtyflglorh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhiwuduotai.top/gtabqbwgra.html

[R50] awk 求和
来源：http://hz.yuanzhike.top/gtqfcbmkxb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.vqdsnc.cn/gtieekhoez.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gtlypmxbov.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.andypj.xyz/gtgyyliyzr.html

[R52] 统计行数
来源：http://hz.fzhhl.top/gtqebjmlie.html

wc -l a.txt
来源：http://hz.yueranfly.top/gturvbpgnh.html

[R53] 查看文件头与实时尾
来源：http://hz.iojbl.cn/gtoybuskya.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.guowangkeji.top/gtpqaylwoh.html

[R54] 比较两个文件
来源：http://hz.guowangkeji.top/gtrgbikpxx.html

diff a.txt b.txt
来源：http://hz.hysaishi.cn/gtzilnxwtq.html

[R55] 压缩与解压
来源：http://hz.xuanzx.com/gtoixapdjb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zycfv.cn/gtpwrlflrn.html

[R56] 远程拷贝
来源：http://hz.havefunace.top/gthdjxxgto.html

scp file user@host:/path/
来源：http://hz.yonumen.top/gtwcazbfzx.html

[R57] 远程执行命令
来源：http://hz.meibo888.top/gtzloicfrq.html


<!-- 参考信息 -->