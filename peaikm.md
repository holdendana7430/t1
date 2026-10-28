代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yangfankeji.com/gtigugjtfs.html

[Q07] 删除表
来源：http://hz.zhaomingkeji.xyz/gtpfrxgfsg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gttczpnrku.html

[Q08] 创建普通索引
来源：http://hz.jqgufenzy.top/gtzyfkibov.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtmbdpaoxu.html

[Q09] 创建唯一索引
来源：http://hz.jinyuanbaomall.cn/gtnzvcaoey.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtxmzbhnoy.html

[Q10] 插入单行
来源：http://hz.gotoacloud.top/gtnagnfwhx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zycfv.cn/gtqwxgbdwf.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gtxwbeyxlb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhiwuduotai.top/gtgouxzrqc.html

[Q12] 插入后取自增 ID
来源：http://hz.aizwys.cn/gtueajwxsp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangdashe.top/gtvimlpeca.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigufen.top/gtsxlfubsq.html

[Q13] 忽略重复插入
来源：http://hz.shuidangran.top/gtwwrulmdd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.havefunace.top/gtqlgctlyh.html

[Q14] 存在则更新（upsert）
来源：http://hz.jqgufenzy.top/gtbiakxxnq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnxiangtu.top/gtfbtkwnij.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtlkuncycq.html

[Q15] 查询全部
来源：http://hz.yj202588.top/gtczhxscly.html

SELECT * FROM users;
来源：http://hz.hfpthk.cn/gtczsdapni.html

[Q16] 查询指定列
来源：http://hz.yuanzhike.top/gtxgafwizj.html

SELECT id, name FROM users;
来源：http://hz.jinyuanbaomall.cn/gtrdzlcldj.html

[Q17] 条件查询
来源：http://hz.mhx1999.top/gtwprzgokm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinyuanbaomall.cn/gtsvxqugng.html

[Q18] 模糊匹配
来源：http://hz.hfpthk.cn/gtwszawtnb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jlsjyb.cn/gtjsxwcmyl.html

[Q19] 范围查询
来源：http://hz.cdnleiting.top/gtuifjqzhy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuetiantiany.cn/gtckmfjmax.html

[Q20] IN 列表
来源：http://hz.chenjidiqi.icu/gtfigetezn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj20258888.top/gtidqfhtfy.html

[Q21] 空值判断
来源：http://hz.xylfe.cn/gtczzbpbhl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sysykeji.top/gtdxywhmkx.html

[Q22] 排序
来源：http://hz.haohaochexian.top/gtlfjjktup.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhengqikj.top/gtqyjjcvwa.html

[Q23] 分页
来源：http://hz.cashguo.top/gtgilktrfp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ivvv.top/gtvnbrdioj.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gtleojlwhw.html

SELECT DISTINCT city FROM users;
来源：http://hz.hongshengwenyu.top/gtnkisyqam.html

[Q25] 只取前 N 条
来源：http://hz.yj202588.top/gtjmtkuqnn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.havefunace.top/gtrqiyqhtn.html

[Q26] 计数
来源：http://hz.chenjidiqi.icu/gtxilxtilv.html

SELECT COUNT(*) FROM users;
来源：http://hz.shuidangran.top/gtijmncivr.html

[Q27] 条件计数
来源：http://hz.jinqigufen.top/gtwrjtvzpu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuanzhike.top/gtmzynzlbh.html

[Q28] 求和与平均
来源：http://hz.yuanzhike.top/gtzqzqfsan.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuxming.cn/gtgglqcmvf.html

[Q29] 最大最小值
来源：http://hz.gogol.net.cn/gtfpnsfflw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhiwuduotai.top/gtcbtbssye.html

[Q30] 分组统计
来源：http://hz.shzxlz.cn/gtnuowmoho.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtqtjbgczi.html

[Q31] 分组后过滤
来源：http://hz.snrcjt.cn/gtxmzcbkyz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhongyouzk.top/gtcjsddxzd.html

[Q32] 分组拼接字符串
来源：http://hz.zdqjudy.top/gtxalzjqzf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtvbqmjvrt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.meibo888.top/gtdghaymbk.html

[Q33] 多列分组
来源：http://hz.ydjk.org.cn/gtmocsaeco.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.quarkkingdee.top/gtfwiqqwzb.html

[Q34] 每组取第一条
来源：http://hz.hywenlv.cn/gtzxktqonm.html

SELECT * FROM (
来源：http://hz.sxryk.cn/gtqgvyvlur.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.svipenyu.cn/gtczhznjob.html

) t WHERE rn = 1;
来源：http://hz.birdmap.top/gtnkqgcmzf.html

[Q35] 内连接
来源：http://hz.hywenlv.cn/gtjnkxxzhs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuxming.cn/gtzlcbtldv.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtwcfdwofo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtssqwtbhf.html

[Q37] 右连接
来源：http://hz.vqdsnc.cn/gtkchsgtdw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhijiandao.cn/gtamoitdgr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtjiexlgld.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gtoyxxxlrq.html

[Q39] 自连接（查上下级）
来源：http://hz.tian-w.cn/gtdzhksfum.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cdnleiting.top/gtajlvfqot.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hywenlv.cn/gtpcxaabdv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jqgufenzy.top/gtikfyqnxn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtcxejahvw.html

[Q41] 多表连接
来源：http://hz.chenlongwang.top/gtekptwsvb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.havefunace.top/gtxpggxihg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tianlin.xyz/gtaaormarg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guowangkeji.top/gtgjvmeggw.html

[Q42] 连接条件附加过滤
来源：http://hz.jiagoushi.top/gtvhjvnleb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.c1oappe.top/gtistgzgys.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ppjwa.cn/gtmcxihwmi.html

[Q43] 标量子查询
来源：http://hz.cashguo.top/gtvaunefmg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gtrkxsrwrl.html

[Q44] IN 子查询
来源：http://hz.zhongyouzk.top/gtfnzmcvvs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinyuanbaomall.cn/gtbneclhyz.html

[Q45] EXISTS 判断存在
来源：http://hz.aizwys.cn/gtviuucilg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gtwyyauhtj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.c1oappe.top/gtnyzbqfvl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fzhhl.top/gtahxacfiq.html

[Q47] 与平均值比较
来源：http://hz.jqgfzy.top/gtyvdmhbgq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cdnleiting.top/gtkmfhwwlp.html

[Q48] CTE 公用表表达式
来源：http://hz.bjfxy.top/gtktiebtnq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daxiang520.top/gtmqujxxdt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.haohaochexian.top/gtmxmacvyb.html

[Q49] 更新单行
来源：http://hz.shangyingyoupin.top/gtpcccxskb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dashuyun.cn/gtntsxsqpe.html

[Q50] 批量更新
来源：http://hz.redwolf501.top/gtngxxkihp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.svipenyu.cn/gteswbemmc.html

[Q51] 用子查询更新
来源：http://hz.smart0.xyz/gtcswkgxwl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhaomingkeji.xyz/gtcvyfvoyv.html

[Q52] 删除指定行
来源：http://hz.shanyushiyangtech.top/gtblfktmzr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daria6918.cn/gttzcduyow.html

[Q53] 按条件删除
来源：http://hz.hysaishi.cn/gtpbdgcwdz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cucudq.cn/gtnpevuhwo.html

[Q54] 清空表
来源：http://hz.yuxming.cn/gthkgjvccq.html

TRUNCATE TABLE logs;
来源：http://hz.iojbl.cn/gtozjskbyw.html

[Q55] 排名（并列占位）
来源：http://hz.nanxinkj.top/gtrzuiudux.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtprlgtbie.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hywenlv.cn/gtzslgxlrm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtqdbqiryo.html

[Q57] 行号
来源：http://hz.jyoumei.cn/gtocysgqfi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuxming.cn/gtmktteyub.html

[Q58] 累计求和
来源：http://hz.daxiang520.top/gtnuzbyumq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.316326.xyz/gtlrmqbruy.html

[Q59] 分组内累计
来源：http://hz.jinqigufen.top/gtqbdhmgxg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yonumen.top/gtgyropuih.html

[Q60] 取上一行 / 下一行
来源：http://hz.fzhhl.top/gtrzeidnzh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtkmeixypo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gthorochba.html

[Q61] 移动平均
来源：http://hz.zhixingplan.top/gtlavuenoq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daria6918.cn/gtewezqogs.html

[Q62] 分组占比
来源：http://hz.cqqwz.cn/gtmsbaqcpz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtlebrklle.html

[Q63] 开启事务
来源：http://hz.snrcjt.cn/gtquttwrjn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtelxurvey.html

[Q64] 提交事务
来源：http://hz.birdmap.top/gtdfodqdno.html

COMMIT;
来源：http://hz.smart0.xyz/gtsaoftmho.html

[Q65] 回滚事务
来源：http://hz.wangdashe.top/gthvictxec.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtipatnkoc.html

[Q66] 行锁查询
来源：http://hz.fengsongda.top/gtaqxmjaxx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.dianchejie.cn/gtqeohhcpk.html

[Q67] 设置隔离级别
来源：http://hz.yj20258888.top/gtytfeyfuy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yueranfly.top/gtsjmphnoh.html

[Q68] 保存点
来源：http://hz.daxiang520.top/gtjvwevxji.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtqypfwyon.html

ROLLBACK TO sp1;
来源：http://hz.yj20258888.top/gtbkmherss.html

[Q69] 查看执行计划
来源：http://hz.pengpengdd.cyou/gtyjejypgn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gtpkdwjazr.html

[Q70] 更新统计信息
来源：http://hz.jyoumei.cn/gtofluccod.html

ANALYZE TABLE users;
来源：http://hz.xingfuxueyuan.xyz/gtbwtkmtgv.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangtech.top/gtupqqroao.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jlsjyb.cn/gtmdqsgqhh.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gtapurosdo.html

SHOW INDEX FROM users;
来源：http://hz.mhx1999.top/gtqvdsxvyb.html

[Q73] 查看表状态
来源：http://hz.jyoumei.cn/gtnoxlsxyu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ivvv.top/gtqecgsozx.html

[Q74] 强制使用索引
来源：http://hz.andypj.xyz/gtcbpqfnyn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gtpsjndsez.html

[Q75] 日期格式化
来源：http://hz.smart0.xyz/gtdlcpeiyw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.meibo888.top/gthmeufjnw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenzaomai.com/gtsxrpyyjn.html

[Q76] 按天统计
来源：http://hz.pengpengdd.cyou/gtzszvltix.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtjaxaodre.html

[Q77] 时间加减
来源：http://hz.chenzaomai.com/gtjvjtaqiz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhengqikj.top/gtyykrpyhx.html

[Q78] 当前时间
来源：http://hz.zhengqikj.top/gtlwojbgyj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daxiang520.top/gtbnuflssf.html

[Q79] 字符串拼接
来源：http://hz.jinghuilouyu.cn/gtoteewhrn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nwbrower.top/gtkfvotyew.html

[Q80] 字符串截取
来源：http://hz.xylfe.cn/gtyrndkvun.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgufenzy.top/gtmaeaswva.html

[Q81] 字符串替换
来源：http://hz.birdmap.top/gtyfhjgynv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangshuangyany.cn/gtvtlktqaf.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtdhcuimrs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtidilxajq.html

[Q83] 大小写转换
来源：http://hz.dashuyun.cn/gtoiyaqxar.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gtwjuwkekd.html

[Q84] 去除首尾空格
来源：http://hz.andypj.xyz/gtmujqxyvz.html

SELECT TRIM(name) FROM users;
来源：http://hz.bjfxy.top/gtkxbdwmbg.html

[Q85] 数值取整
来源：http://hz.hongshengwenyu.top/gttrvqsirf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yueranfly.top/gtnhjknpra.html

[Q86] 读取 JSON 字段
来源：http://hz.vqdsnc.cn/gtswkwwbrv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hfpthk.cn/gtxycquyea.html

[Q87] JSON 字段做条件
来源：http://hz.sufxvd.cn/gthicqawsb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtulhtqpml.html

[Q88] 行转列（条件聚合）
来源：http://hz.gzhubu.top/gtfezembqn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtfgyxpcnr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ywan-chungtsiang.top/gtzeyskxpo.html

[Q89] 判断表是否存在
来源：http://hz.ywan-chungtsiang.top/gtekuwyivq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gotoacloud.top/gtgkcakjcq.html

[Q90] 生成序号列
来源：http://hz.nwbrower.top/gtqqiqfhqo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gtriyrveww.html

================================================================================
来源：http://hz.yuxming.cn/gtethizdsi.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtzkggkpqi.html

================================================================================
来源：http://hz.tianlin.xyz/gtsnoiovpj.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtlruaimve.html

#!/usr/bin/env bash
来源：http://hz.hongshengwenyu.top/gtorghndhj.html

set -euo pipefail
来源：http://hz.yj20258.top/gtfiogmxug.html

[R02] 变量赋值与使用
来源：http://hz.yj20258.top/gttlopndzo.html

name="Tom"; echo "$name"
来源：http://hz.jiagoushi.top/gtcugtapcq.html

[R03] 只读变量
来源：http://hz.vqdsnc.cn/gtmiddflyj.html

readonly PI=3.14
来源：http://hz.ywan-chungtsiang.top/gtdefipdgc.html

[R04] 位置参数
来源：http://hz.xziqi.cn/gtfewldnpn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gtmgxqidzq.html

[R05] 参数默认值
来源：http://hz.yj202588.top/gtbfqgxvaq.html

name="${1:-default}"
来源：http://hz.meibo888.top/gtytjiomki.html

[R06] 判断命令是否存在
来源：http://hz.xylfe.cn/gtqhsttthk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgfzy.top/gtmwgmqtds.html

[R07] if 判断文件
来源：http://hz.gzhubu.top/gtbbswuqwr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hongshengwenyu.top/gtlgacyhjs.html

[R08] 数值比较
来源：http://hz.chenlongwang.top/gtzlavzdhz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cqqwz.cn/gthnswdlyg.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtiodsxvxo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zdqjudy.top/gtscfaqjuo.html

[R10] 正则匹配
来源：http://hz.jqgufenzy.top/gtkfhesxsx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gtfifzcszp.html

[R11] case 多分支
来源：http://hz.wangdashe.top/gttrwlahsc.html

case "$1" in
来源：http://hz.daria6918.cn/gtifmpfdrq.html

start) echo "启动" ;;
来源：http://hz.chenlongwang.top/gtlfnjgsua.html

stop)  echo "停止" ;;
来源：http://hz.ywan-chungtsiang.top/gtakmjzlax.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtwgtfyfdr.html

esac
来源：http://hz.aibaodan.cn/gtwhyodkhd.html

[R12] for 遍历文件
来源：http://hz.shangyingyoupin.top/gtnlgnyibm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xziqi.cn/gtcfgeigrk.html

[R13] for 计数循环
来源：http://hz.xuanzx.com/gtguohuoaa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigufen.top/gttchchpnm.html

[R14] C 风格 for
来源：http://hz.sxryk.cn/gtpramkxlb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtyteebwnu.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtavgvcqho.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jyoumei.cn/gtjkymwqhs.html

[R16] until 等待条件
来源：http://hz.jyoumei.cn/gtnvyryssv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.9152youxi.cn/gtawazwper.html

[R17] 数组定义与取值
来源：http://hz.hnqzz.top/gtpyznclpt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258888.top/gtadwnobrz.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gtjcyfgeih.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.vqdsnc.cn/gthwtrtnrp.html

[R19] 数组长度
来源：http://hz.shanyushiyangtech.top/gtzqsareww.html

echo "${#arr[@]}"
来源：http://hz.tianlin.xyz/gtmeifeuml.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtehfcetgw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.guowangkeji.top/gtyyaaxbtb.html

[R21] 字符串长度
来源：http://hz.yuanzhike.top/gtdqnzaaxy.html

echo "${#s}"
来源：http://hz.meibo888.top/gtdbdeltwc.html

[R22] 截取子串
来源：http://hz.pengpengdd.cyou/gtmbqmctbd.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gtktwbkmip.html

[R23] 字符串替换
来源：http://hz.cashguo.top/gtllztmvym.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gtktwtfvca.html

[R24] 大小写转换
来源：http://hz.daria6918.cn/gtlauwrmim.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zdqjudy.top/gtcimhgdik.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtcupkuxkh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hammf.cn/gtglszhcii.html

[R26] 命令替换
来源：http://hz.ydjk.org.cn/gtluurdcez.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gtegkgtiba.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gtaklgoxtg.html

echo $((1 + 2 * 3))
来源：http://hz.yuxming.cn/gthqpbydyz.html

[R28] 浮点运算
来源：http://hz.yj20258888.top/gtylifmomu.html

echo "scale=2; 10/3" | bc
来源：http://hz.sweek.top/gtbaovtutb.html

[R29] 定义函数
来源：http://hz.yangfankeji.com/gtznyzbcax.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtoowaxqnn.html

[R30] 函数返回状态码
来源：http://hz.zhoulong.xyz/gteellcgui.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gtmzsuaqqp.html

[R31] 局部变量
来源：http://hz.cheryme.top/gteedmursx.html

f() { local x=1; echo "$x"; }
来源：http://hz.xziqi.cn/gtmzeucxfl.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtljtlbvvc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtdtelfkuv.html

[R33] 捕获错误并提示行号
来源：http://hz.havefunace.top/gtwocomduy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ywan-chungtsiang.top/gtjjajbmuw.html

[R34] 退出时清理
来源：http://hz.jiagoushi.top/gteavutceo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gttwquzcie.html

[R35] 后台执行并等待
来源：http://hz.tian-w.cn/gtqicnsbfy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gttrpywzov.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtrkftfbdi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nwbrower.top/gtnrcyazsi.html

[R37] 把输出赋给变量
来源：http://hz.nanxinkj.top/gtlboecomr.html

files=$(ls -1)
来源：http://hz.wangshuangyany.cn/gtctyldjvw.html

[R38] 管道串联
来源：http://hz.52xcode.cn/gtwlxmpxrc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtaazfbzio.html

[R39] 重定向标准输出与错误
来源：http://hz.gotoacloud.top/gtiyftbsbv.html

cmd > out.log 2>&1
来源：http://hz.cashguo.top/gtjqtniaut.html

[R40] 追加写日志
来源：http://hz.xuanzx.com/gtpglfedyr.html

echo "log" >> out.log
来源：http://hz.hnxiangtu.top/gtcrqtkfgx.html

[R41] 丢弃输出
来源：http://hz.jyoumei.cn/gtboxcnbqg.html

cmd >/dev/null 2>&1
来源：http://hz.hnxiangtu.top/gthykxkfts.html

[R42] 输入重定向
来源：http://hz.yvedp.cn/gtjqlbndtd.html

wc -l < a.txt
来源：http://hz.sxryk.cn/gtfiyskxtd.html

[R43] 按名字查找文件
来源：http://hz.daria6918.cn/gtikgklogv.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gtjarexvyy.html

[R44] 按修改时间查找
来源：http://hz.ppjwa.cn/gtqkyfwmhf.html

find . -mtime -7 -type f
来源：http://hz.yj20258.top/gtjlhpqwjd.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtppbtbdhc.html

find . -name "*.tmp" -delete
来源：http://hz.chenlongwang.top/gtcnytzabh.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtbfcwyyno.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxinkj.top/gtuinqkdlt.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gtnudqdorc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aizwys.cn/gthpaafeov.html

[R48] awk 取指定列
来源：http://hz.nwbrower.top/gtyyvgktoe.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtbthzxzqv.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtfodsqmxe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuanzhike.top/gtxtskbkwp.html

[R50] awk 求和
来源：http://hz.ppjwa.cn/gtaskstgoy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gtbwljjcdj.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtunvazuuq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtmpalwprt.html

[R52] 统计行数
来源：http://hz.sweek.top/gtkhyvkxoh.html

wc -l a.txt
来源：http://hz.mhx1999.top/gtthgdptrh.html

[R53] 查看文件头与实时尾
来源：http://hz.birdmap.top/gttowqxech.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.mhx1999.top/gtbekgyvni.html

[R54] 比较两个文件
来源：http://hz.gzhubu.top/gtalaqgzwr.html

diff a.txt b.txt
来源：http://hz.fengsongda.top/gtqdxfmwau.html

[R55] 压缩与解压
来源：http://hz.sysykeji.top/gtbdljmlpq.html


<!-- 参考信息 -->