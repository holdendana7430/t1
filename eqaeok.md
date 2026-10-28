代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhaomingkeji.xyz/gtgliryjlp.html

[Q11] 一次插入多行
来源：http://hz.zhongyouzk.top/gtyelacnme.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhaomingkeji.xyz/gtmlsrofmr.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258888.top/gtxebfrtwx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtxuiqsmuf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.feifeiyinyue.top/gtbsfvkurr.html

[Q13] 忽略重复插入
来源：http://hz.316326.xyz/gtempdydod.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sxryk.cn/gtrqjzbgft.html

[Q14] 存在则更新（upsert）
来源：http://hz.xuetiantiany.cn/gtxixpxyka.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nwbrower.top/gttixjxvbf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ywan-chungtsiang.top/gtgfobomtx.html

[Q15] 查询全部
来源：http://hz.ybcxt.top/gtirjanvhq.html

SELECT * FROM users;
来源：http://hz.hywenlv.cn/gtbiftpyvn.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gthybqbjpn.html

SELECT id, name FROM users;
来源：http://hz.daxiang520.top/gtlpxswwff.html

[Q17] 条件查询
来源：http://hz.zhixingplan.top/gtrepbylvy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hnxiangtu.top/gtbchgmpjj.html

[Q18] 模糊匹配
来源：http://hz.c1oappe.top/gtygawyzjf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhoulong.xyz/gteftblupy.html

[Q19] 范围查询
来源：http://hz.jinqigfzy.top/gtodciopqn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jianghu66.top/gtmfefinrs.html

[Q20] IN 列表
来源：http://hz.zhengqikj.top/gtcdbskhgn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cucudq.cn/gtuplkxpld.html

[Q21] 空值判断
来源：http://hz.redwolf501.top/gtvsuubfbl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhixingplan.top/gtrnvgidmq.html

[Q22] 排序
来源：http://hz.wangshuangyany.cn/gtityiktqf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinghuilouyu.cn/gtjcpechdw.html

[Q23] 分页
来源：http://hz.gaohongyu789.top/gtculynomj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tanke756.top/gtfakiaztz.html

[Q24] 去重
来源：http://hz.jyoumei.cn/gtmkxyqwam.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigufen.top/gtqznxiigr.html

[Q25] 只取前 N 条
来源：http://hz.hfpthk.cn/gtxxnzqqok.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cdnleiting.top/gtkwvzjawr.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gtdsfyqndg.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenjidiqi.icu/gtfermpkmq.html

[Q27] 条件计数
来源：http://hz.316326.xyz/gtospslvhn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenzaomai.com/gtxhiekucx.html

[Q28] 求和与平均
来源：http://hz.chenlongwang.top/gtgpllscbu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtyljtgpbb.html

[Q29] 最大最小值
来源：http://hz.sufxvd.cn/gtmrxhecdv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gtnxfxpinl.html

[Q30] 分组统计
来源：http://hz.meibo888.top/gtlmqbzrbe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtvhrdpimn.html

[Q31] 分组后过滤
来源：http://hz.jinqigfzy.top/gtwnwkuspr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.feifeiyinyue.top/gtqzumvtba.html

[Q32] 分组拼接字符串
来源：http://hz.yj202588.top/gtzrycrynj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtytpsccjd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.316326.xyz/gtnfnrliwz.html

[Q33] 多列分组
来源：http://hz.zhiwuduotai.top/gtypjgbyfr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zdqjudy.top/gtjzducgcy.html

[Q34] 每组取第一条
来源：http://hz.jianghu66.top/gtdmhbqgzh.html

SELECT * FROM (
来源：http://hz.mhx1999.top/gtlosskghv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtoirvowyq.html

) t WHERE rn = 1;
来源：http://hz.zhongyouzk.top/gttcswaoca.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gttlnbbins.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtvfijmoxj.html

[Q36] 左连接
来源：http://hz.xuanzx.com/gteuzntprg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtdsprtysj.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gtajblcuhy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yangfankeji.com/gtbaaeflic.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.c1oappe.top/gtdgdgoifj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgfzy.top/gtdahuqnfs.html

[Q39] 自连接（查上下级）
来源：http://hz.cashguo.top/gtaobfydei.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yvedp.cn/gtdyzmywor.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangshuangyany.cn/gtscqvcncy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenzaomai.com/gtptfqaycn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydjk.org.cn/gtrunxdfcz.html

[Q41] 多表连接
来源：http://hz.sufxvd.cn/gtlhvjxxaq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yueranfly.top/gtsedgdsnr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xinyue.icu/gtudwkfzeh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj20258.top/gtieigdvhn.html

[Q42] 连接条件附加过滤
来源：http://hz.iojbl.cn/gtfiewmyxu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtafludfyi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.mhx1999.top/gtckbjckmk.html

[Q43] 标量子查询
来源：http://hz.gotoacloud.top/gtqbukxohy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.316326.xyz/gtfdnsvgry.html

[Q44] IN 子查询
来源：http://hz.dianchejie.cn/gtlyxckaje.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daxiang520.top/gtbspbwwnn.html

[Q45] EXISTS 判断存在
来源：http://hz.yuanzhike.top/gtzwaojewt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtflrqiiqt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtzhdwqbdb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtsrecqfdx.html

[Q47] 与平均值比较
来源：http://hz.daxiang520.top/gtqklzrkua.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.meibo888.top/gtehbtqxrp.html

[Q48] CTE 公用表表达式
来源：http://hz.zhoulong.xyz/gthebcjpnc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.kuanghao11.cn/gtqbgdhsew.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zdqjudy.top/gtsxrtyzhb.html

[Q49] 更新单行
来源：http://hz.daxiang520.top/gtithothjw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtkplnvgjz.html

[Q50] 批量更新
来源：http://hz.cqqwz.cn/gtiybppwko.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cqqwz.cn/gtupmqdmie.html

[Q51] 用子查询更新
来源：http://hz.feifeiyinyue.top/gtwhvnddqd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinyuanbaomall.cn/gtiupdhagh.html

[Q52] 删除指定行
来源：http://hz.jqgfzy.top/gtevyckzfd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtaijuxfex.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gtxwcdaexu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.316326.xyz/gtsakqtkap.html

[Q54] 清空表
来源：http://hz.cashguo.top/gtznmcukju.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtexihccox.html

[Q55] 排名（并列占位）
来源：http://hz.iojbl.cn/gthcqlbmxi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dashuyun.cn/gtrqvlgtun.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yonumen.top/gtwvrqlber.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.haohaochexian.top/gtnvwsczdd.html

[Q57] 行号
来源：http://hz.yonumen.top/gtxntkvqpv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.havefunace.top/gtmdidubbl.html

[Q58] 累计求和
来源：http://hz.jqgufenzy.top/gtvybtmjwz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pengpengdd.cyou/gtzmuvpapi.html

[Q59] 分组内累计
来源：http://hz.cdnleiting.top/gteomftver.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xziqi.cn/gtqtayosyg.html

[Q60] 取上一行 / 下一行
来源：http://hz.cqqwz.cn/gthonfkqpf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.kuanghao11.cn/gtxzvckulw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhixingplan.top/gtsjrhstjc.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtxhnvdqkw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daxiang520.top/gtphdxpxwe.html

[Q62] 分组占比
来源：http://hz.yj20258.top/gtavjzxgjm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtuanidnyt.html

[Q63] 开启事务
来源：http://hz.nanxuanxn.top/gtcmgvpczc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xingfuxueyuan.xyz/gthwxyywmd.html

[Q64] 提交事务
来源：http://hz.sufxvd.cn/gtzoiilbmf.html

COMMIT;
来源：http://hz.yongpay.top/gtpobdnfkd.html

[Q65] 回滚事务
来源：http://hz.shanyushiyangtech.top/gtxevfapkk.html

ROLLBACK;
来源：http://hz.jinqigfzy.top/gtbulcgoch.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtggnocggu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuetiantiany.cn/gtdeiycmjy.html

[Q67] 设置隔离级别
来源：http://hz.xingfuxueyuan.xyz/gtwmivrgfw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pengpengdd.cyou/gtspjaxigj.html

[Q68] 保存点
来源：http://hz.fzhhl.top/gtpudxfcpz.html

SAVEPOINT sp1;
来源：http://hz.ppjwa.cn/gtwswhjqfb.html

ROLLBACK TO sp1;
来源：http://hz.cucudq.cn/gtucrwgnjk.html

[Q69] 查看执行计划
来源：http://hz.bjfxy.top/gtyfujvknw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtyagderbf.html

[Q70] 更新统计信息
来源：http://hz.svipenyu.cn/gtvrbfvtnl.html

ANALYZE TABLE users;
来源：http://hz.pycfn.com/gtiwhfmhjx.html

[Q71] 查看建表语句
来源：http://hz.redwolf501.top/gtdzlfrglz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangshuangyany.cn/gtoqdmdkns.html

[Q72] 查看索引
来源：http://hz.yj20258.top/gtcbbvhaoo.html

SHOW INDEX FROM users;
来源：http://hz.feifeiyinyue.top/gtpwbwjkxv.html

[Q73] 查看表状态
来源：http://hz.ybcxt.top/gtqlwyiajd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jianghu66.top/gtastbwbpj.html

[Q74] 强制使用索引
来源：http://hz.pengpengdd.cyou/gtnrjyvigx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ppjwa.cn/gtsxkvhffz.html

[Q75] 日期格式化
来源：http://hz.meibo888.top/gtfocdbqqz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gotoacloud.top/gtkgxxqglx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.fengsongda.top/gtmdwkmrzk.html

[Q76] 按天统计
来源：http://hz.yj20258888.top/gtzeicwiex.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258888.top/gtibfbfgam.html

[Q77] 时间加减
来源：http://hz.nanxinkj.top/gtdzxwvmmd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtzjprxkfj.html

[Q78] 当前时间
来源：http://hz.yvedp.cn/gtqqrqlmlo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sxryk.cn/gtwxkbnoni.html

[Q79] 字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gtefebccen.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.feifeiyinyue.top/gtwqalthli.html

[Q80] 字符串截取
来源：http://hz.ybcxt.top/gtsbqistna.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jiagoushi.top/gtkldvcgpk.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtqgqbqlts.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daria6918.cn/gtnapbczjh.html

[Q82] 字符长度与字节长度
来源：http://hz.zhengqikj.top/gthufazpgj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gttfmglltk.html

[Q83] 大小写转换
来源：http://hz.9152youxi.cn/gtdrmhmala.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.snrcjt.cn/gthdjzommj.html

[Q84] 去除首尾空格
来源：http://hz.ybcxt.top/gtclxizbyf.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gttfjmsrfc.html

[Q85] 数值取整
来源：http://hz.yj20258888.top/gtvmrvqfcz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydjk.org.cn/gtlbjzpsif.html

[Q86] 读取 JSON 字段
来源：http://hz.snrcjt.cn/gtbibbuqjk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yueranfly.top/gtzfjzzkde.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigufen.top/gtraoiuqyq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ybcxt.top/gtwekgolkn.html

[Q88] 行转列（条件聚合）
来源：http://hz.tanke756.top/gtgnozmxrh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xziqi.cn/gtrxgedxyi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.9152youxi.cn/gtxcgfydgg.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gtxtyfcpgc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gtxsbnobdi.html

[Q90] 生成序号列
来源：http://hz.sufxvd.cn/gtyxgjcyxm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigfzy.top/gtribznzds.html

================================================================================
来源：http://hz.xuanzx.com/gtcfrmjhvw.html

R. Bash 专题
来源：http://hz.nwbrower.top/gtjhjtabmm.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtoqpoxzna.html

[R01] shebang 与严格模式
来源：http://hz.hnxiangtu.top/gtpbfbcfbe.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtjsuibwkd.html

set -euo pipefail
来源：http://hz.jinghuilouyu.cn/gtpdcxfuqw.html

[R02] 变量赋值与使用
来源：http://hz.nanxuanxn.top/gtesbzmnzy.html

name="Tom"; echo "$name"
来源：http://hz.jlsjyb.cn/gtsgrqgrwl.html

[R03] 只读变量
来源：http://hz.guowangkeji.top/gtigajrjae.html

readonly PI=3.14
来源：http://hz.yongpay.top/gtsrmjxvca.html

[R04] 位置参数
来源：http://hz.xinyue.icu/gtdtwglrju.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.vqdsnc.cn/gtonkikbjb.html

[R05] 参数默认值
来源：http://hz.quarkkingdee.top/gtvuzfmwnm.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gttpljcevk.html

[R06] 判断命令是否存在
来源：http://hz.jlsjyb.cn/gtejvqgsdv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.quarkkingdee.top/gtdlridhhf.html

[R07] if 判断文件
来源：http://hz.yj202588.top/gtqoqejunl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yuanzhike.top/gtrirzrowx.html

[R08] 数值比较
来源：http://hz.jinqigfzy.top/gtzyofnqrp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtqvpoyncy.html

[R09] 字符串比较
来源：http://hz.chenjidiqi.icu/gtxiqiehnj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gtkwaokpbz.html

[R10] 正则匹配
来源：http://hz.gotoacloud.top/gtcporpmmy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hammf.cn/gtuttkiwyq.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gtfcawfodu.html

case "$1" in
来源：http://hz.jqgfzy.top/gtiovfyyow.html

start) echo "启动" ;;
来源：http://hz.jqgufenzy.top/gtnnucwkux.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtityffojq.html

*)     echo "未知命令" ;;
来源：http://hz.kuanghao11.cn/gtzthhseut.html

esac
来源：http://hz.zhijiandao.cn/gtgztkkjns.html

[R12] for 遍历文件
来源：http://hz.ydjk.org.cn/gtaujrtydy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgufenzy.top/gtitigvdmt.html

[R13] for 计数循环
来源：http://hz.xinyue.icu/gtrsfpesny.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtfibphvah.html

[R14] C 风格 for
来源：http://hz.daria6918.cn/gtlstxpqdn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ivvv.top/gtxuvsgdik.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gttluutmxd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zycfv.cn/gtkttmocrt.html

[R16] until 等待条件
来源：http://hz.iojbl.cn/gtvogmdlhj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtupqksbfb.html

[R17] 数组定义与取值
来源：http://hz.feifeiyinyue.top/gtgufpizlk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gttyzystnl.html

[R18] 遍历数组
来源：http://hz.gaohongyu789.top/gtptlbugos.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtghetwbtn.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gturyiuyha.html

echo "${#arr[@]}"
来源：http://hz.hnxiangtu.top/gtsiddmxft.html

[R20] 关联数组（字典）
来源：http://hz.ydjk.org.cn/gtthsogsrz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aibaodan.cn/gtyhsifhfs.html

[R21] 字符串长度
来源：http://hz.bjfxy.top/gtcevqtujz.html

echo "${#s}"
来源：http://hz.jiagoushi.top/gtvwncxlex.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gtbwfcplmg.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtryagkccs.html

[R23] 字符串替换
来源：http://hz.gaohongyu789.top/gtcjcczxyq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zdqjudy.top/gtsdypopba.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gtgmpykzwf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yongpay.top/gtgvznetcz.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gthhyadllh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gotoacloud.top/gtpjtszzim.html

[R26] 命令替换
来源：http://hz.zhijiandao.cn/gtszwkobgo.html

now=$(date +%F); echo "$now"
来源：http://hz.mhx1999.top/gtnnpqxsxl.html

[R27] 算术展开
来源：http://hz.ybcxt.top/gtpoemhugp.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtzikmuqdf.html

[R28] 浮点运算
来源：http://hz.hnqzz.top/gtszwqqhhu.html

echo "scale=2; 10/3" | bc
来源：http://hz.jyoumei.cn/gtnzxerltg.html

[R29] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtywgxokah.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gzhubu.top/gtpvibsrdh.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gtbihxexsx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.0kj1m.cn/gthvvgjusz.html

[R31] 局部变量
来源：http://hz.jqgfzy.top/gtsaavpwuo.html

f() { local x=1; echo "$x"; }
来源：http://hz.shuidangran.top/gtzchadjbk.html

[R32] 参数个数校验
来源：http://hz.yanxiufei.cn/gtznliynfr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cdnleiting.top/gtnlqfvaqv.html

[R33] 捕获错误并提示行号
来源：http://hz.xylfe.cn/gtttsjqnhe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhiwuduotai.top/gtoqrbuypy.html

[R34] 退出时清理
来源：http://hz.316326.xyz/gtrrmybahe.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtyhotzbtr.html

[R35] 后台执行并等待
来源：http://hz.sxryk.cn/gtrksvgpuu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj202588.top/gtmncbzeal.html

[R36] 并发执行多个任务
来源：http://hz.jianghu66.top/gthwufadeh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhixingplan.top/gtzqscqdls.html

[R37] 把输出赋给变量
来源：http://hz.yueranfly.top/gtspsnilhx.html

files=$(ls -1)
来源：http://hz.dashuyun.cn/gtpldtkxex.html

[R38] 管道串联
来源：http://hz.yonumen.top/gtnufkkzcj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinqigfzy.top/gtmixsfibx.html

[R39] 重定向标准输出与错误
来源：http://hz.cqqwz.cn/gterbykbzu.html

cmd > out.log 2>&1
来源：http://hz.quarkkingdee.top/gtqmwbelpl.html

[R40] 追加写日志
来源：http://hz.jinyuanbaomall.cn/gtosmfgjml.html

echo "log" >> out.log
来源：http://hz.vqdsnc.cn/gteovnabfx.html

[R41] 丢弃输出
来源：http://hz.tanke756.top/gtvmzdfgkg.html

cmd >/dev/null 2>&1
来源：http://hz.gaohongyu789.top/gtpseejibq.html

[R42] 输入重定向
来源：http://hz.hfpthk.cn/gtvtgashbm.html

wc -l < a.txt
来源：http://hz.0kj1m.cn/gtnrzcpqjz.html

[R43] 按名字查找文件
来源：http://hz.yangfankeji.com/gtuzqasffw.html

find . -name "*.log" -type f
来源：http://hz.hywenlv.cn/gtgowrymly.html

[R44] 按修改时间查找
来源：http://hz.hysaishi.cn/gtzedduofe.html

find . -mtime -7 -type f
来源：http://hz.mhx1999.top/gtphoghwbu.html

[R45] 批量删除
来源：http://hz.tanke756.top/gtedfdgnes.html

find . -name "*.tmp" -delete
来源：http://hz.9152youxi.cn/gtdjrjljuq.html

[R46] 递归替换文件内容
来源：http://hz.hysaishi.cn/gthqicgbnv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.0kj1m.cn/gtxibidkdm.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtmvsykicz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jlsjyb.cn/gtbzljvzjd.html

[R48] awk 取指定列
来源：http://hz.meibo888.top/gthdqxsmly.html

awk '{print $1, $3}' a.txt
来源：http://hz.cashguo.top/gtuxrlpzzf.html

[R49] awk 带条件
来源：http://hz.shanyushiyangkeji.top/gtemzemphu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gthbnistll.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtsgyypkla.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhengqikj.top/gtzjarorbm.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gtvwilegob.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ivvv.top/gtcmlmwunh.html

[R52] 统计行数
来源：http://hz.zhiwuduotai.top/gthcwhnbzh.html

wc -l a.txt
来源：http://hz.daria6918.cn/gtxtdoucnr.html

[R53] 查看文件头与实时尾
来源：http://hz.vqdsnc.cn/gtsmatcjya.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gaohongyu789.top/gtayvwojmz.html

[R54] 比较两个文件
来源：http://hz.chenjidiqi.icu/gtqhuefchb.html

diff a.txt b.txt
来源：http://hz.tanke756.top/gthjssxlin.html

[R55] 压缩与解压
来源：http://hz.tianlin.xyz/gtcpgukknu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenlongwang.top/gtynaagcvs.html

[R56] 远程拷贝
来源：http://hz.tianlin.xyz/gtsntgkkgj.html

scp file user@host:/path/
来源：http://hz.tanke756.top/gtmgtseosa.html

[R57] 远程执行命令
来源：http://hz.meibo888.top/gtwseelyxj.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtrvfjnzpg.html

[R58] 下载文件
来源：http://hz.tian-w.cn/gtwiuilagd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.andypj.xyz/gthbmketeg.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtglshlhmb.html


<!-- 参考信息 -->