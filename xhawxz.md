代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ybcxt.top/gtooskwsay.html

[Q09] 创建唯一索引
来源：http://hz.snrcjt.cn/gtmiutnlta.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtinumkcfu.html

[Q10] 插入单行
来源：http://hz.yj20258888.top/gtpamqdhhy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtkxtzcddo.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtpwqdnjzw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tanke756.top/gtiuelcgea.html

[Q12] 插入后取自增 ID
来源：http://hz.smart0.xyz/gtzwcdyqjf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ybcxt.top/gtjsvzcsav.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xziqi.cn/gtldwosgcb.html

[Q13] 忽略重复插入
来源：http://hz.aizwys.cn/gtndzrldas.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangtech.top/gtxddsmkwm.html

[Q14] 存在则更新（upsert）
来源：http://hz.0kj1m.cn/gtlpebowjq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ydjk.org.cn/gtgfiidqcg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.meibo888.top/gtipqiplbk.html

[Q15] 查询全部
来源：http://hz.hongshengwenyu.top/gtrnlwadnp.html

SELECT * FROM users;
来源：http://hz.yuanzhike.top/gtuwrrgwuh.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtexjmfxdt.html

SELECT id, name FROM users;
来源：http://hz.pengpengdd.cyou/gtvzlxwect.html

[Q17] 条件查询
来源：http://hz.gaohongyu789.top/gtpkmrcrll.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cqqwz.cn/gtvvvgrkvl.html

[Q18] 模糊匹配
来源：http://hz.jqgufenzy.top/gtxqlyzrfo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ivvv.top/gtzdobzamh.html

[Q19] 范围查询
来源：http://hz.c1oappe.top/gtgaobpxqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yuanzhike.top/gttcfypnet.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gtxmdaszwr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pycfn.com/gtezyvsetg.html

[Q21] 空值判断
来源：http://hz.ehwqpu.com/gtykicmtzx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pengpengdd.cyou/gtdcglqjmr.html

[Q22] 排序
来源：http://hz.sufxvd.cn/gtkruxzxln.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.9152youxi.cn/gtilbhbxsr.html

[Q23] 分页
来源：http://hz.haohaochexian.top/gtrxxbcapk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gtzxsysdyu.html

[Q24] 去重
来源：http://hz.cheryme.top/gtvsqrnvbm.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhengqikj.top/gtuqxobcnb.html

[Q25] 只取前 N 条
来源：http://hz.jyoumei.cn/gtfhmmearm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tanke756.top/gtmzjypqoe.html

[Q26] 计数
来源：http://hz.ydjk.org.cn/gtsmqpcwmt.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuanzhike.top/gtatapytgq.html

[Q27] 条件计数
来源：http://hz.zhiwuduotai.top/gtijcxhove.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.smart0.xyz/gthbuapdrh.html

[Q28] 求和与平均
来源：http://hz.yj20258888.top/gtoptgqbet.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhijiandao.cn/gtmedullht.html

[Q29] 最大最小值
来源：http://hz.zhixingplan.top/gtnxqmezdt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gaohongyu789.top/gtuwmafame.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtchwbdwyy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtwvbeifqv.html

[Q31] 分组后过滤
来源：http://hz.ydjk.org.cn/gtmnubbvtz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tian-w.cn/gtgxalcedb.html

[Q32] 分组拼接字符串
来源：http://hz.cashguo.top/gtwfkejbld.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtnqklmyge.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pycfn.com/gtnvkyplei.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gthetchscq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tanke756.top/gtueixjexi.html

[Q34] 每组取第一条
来源：http://hz.ehwqpu.com/gtykkxsowa.html

SELECT * FROM (
来源：http://hz.birdmap.top/gteozaeusu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shzxlz.cn/gtbfyfligd.html

) t WHERE rn = 1;
来源：http://hz.cucudq.cn/gtemwfgtjf.html

[Q35] 内连接
来源：http://hz.gaohongyu789.top/gtbmvyzwyk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtwujqfncz.html

[Q36] 左连接
来源：http://hz.zhixingplan.top/gtceisxpvn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gtmtyadzaq.html

[Q37] 右连接
来源：http://hz.ivvv.top/gtovwsnnjl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gtjcpkruun.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shzxlz.cn/gtjnkzctls.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhaomingkeji.xyz/gtvbuommis.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gthgzmfazs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtfdfpxltd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yanxiufei.cn/gtrdyzywdg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.iojbl.cn/gtrpboqdjh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jianghu66.top/gtuaojeeoe.html

[Q41] 多表连接
来源：http://hz.52xcode.cn/gtbpgoycox.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtkenlzvnd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.52xcode.cn/gtedkskoiy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.iojbl.cn/gtvofffvoq.html

[Q42] 连接条件附加过滤
来源：http://hz.shzxlz.cn/gtkahpuwdx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydzc1.top/gtibadxemh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fengsongda.top/gtlyynmuwe.html

[Q43] 标量子查询
来源：http://hz.yongpay.top/gtzwfpsfil.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuetiantiany.cn/gtgdsidldu.html

[Q44] IN 子查询
来源：http://hz.ydzc1.top/gtcvmuzodk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nwbrower.top/gttyxtkxan.html

[Q45] EXISTS 判断存在
来源：http://hz.wangshuangyany.cn/gtpbcgabwv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydzc1.top/gttnwgjwpi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yvedp.cn/gttztjbgcx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtcmqugmeo.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtwyvheobf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.mhx1999.top/gtifiumemt.html

[Q48] CTE 公用表表达式
来源：http://hz.zhiwuduotai.top/gtsyrgwktc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sysykeji.top/gtisryplak.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuetiantiany.cn/gtsauiwyat.html

[Q49] 更新单行
来源：http://hz.sweek.top/gtrozfnttg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtvdmwssek.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtzlbphlep.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.bjfxy.top/gtohpzsddl.html

[Q51] 用子查询更新
来源：http://hz.yongpay.top/gtamxqayji.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cashguo.top/gtyeswkfoj.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gtywxbcgvx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.quarkkingdee.top/gtflhpslpd.html

[Q53] 按条件删除
来源：http://hz.feifeiyinyue.top/gtfirolash.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nwbrower.top/gtguwqfuxt.html

[Q54] 清空表
来源：http://hz.hnxiangtu.top/gtsxakmflw.html

TRUNCATE TABLE logs;
来源：http://hz.snrcjt.cn/gtoisguobm.html

[Q55] 排名（并列占位）
来源：http://hz.mhx1999.top/gtnmdgmczb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhongyouzk.top/gtkzxccdfv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shuidangran.top/gtzeotbued.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangdashe.top/gtgkjzxxxl.html

[Q57] 行号
来源：http://hz.xziqi.cn/gtzemwoiot.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aizwys.cn/gtaeyoottq.html

[Q58] 累计求和
来源：http://hz.jinyuanbaomall.cn/gtyukplzzh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnqzz.top/gtmhclyddf.html

[Q59] 分组内累计
来源：http://hz.nanxinkj.top/gtflppafyy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cdnleiting.top/gtugxuayly.html

[Q60] 取上一行 / 下一行
来源：http://hz.ybcxt.top/gtpbzyzmbj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtmxujeqdt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cheryme.top/gtfgqgicel.html

[Q61] 移动平均
来源：http://hz.daxiang520.top/gtwasfhqgk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gogol.net.cn/gtvdpamvde.html

[Q62] 分组占比
来源：http://hz.jqgfzy.top/gtfzbhnzwp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtaphvyyye.html

[Q63] 开启事务
来源：http://hz.ppjwa.cn/gtzhumrlic.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.dashuyun.cn/gtfhsumigv.html

[Q64] 提交事务
来源：http://hz.smart0.xyz/gtcoficjyx.html

COMMIT;
来源：http://hz.xylfe.cn/gtbaymdpzb.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gthkdpnygh.html

ROLLBACK;
来源：http://hz.jlsjyb.cn/gtyseyacii.html

[Q66] 行锁查询
来源：http://hz.sweek.top/gtcwkcgtte.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gthiahiqfd.html

[Q67] 设置隔离级别
来源：http://hz.jinghuilouyu.cn/gtdxzfgyfv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gthgatwhzx.html

[Q68] 保存点
来源：http://hz.cdnleiting.top/gtfqshgofs.html

SAVEPOINT sp1;
来源：http://hz.andypj.xyz/gtwozzclcj.html

ROLLBACK TO sp1;
来源：http://hz.yueranfly.top/gtdsmnnego.html

[Q69] 查看执行计划
来源：http://hz.cqqwz.cn/gtrzvpient.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtktiqirti.html

[Q70] 更新统计信息
来源：http://hz.yvedp.cn/gtoavusags.html

ANALYZE TABLE users;
来源：http://hz.aizwys.cn/gtpdgknyma.html

[Q71] 查看建表语句
来源：http://hz.pycfn.com/gtysummznd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.9152youxi.cn/gtjubhgqwc.html

[Q72] 查看索引
来源：http://hz.hnxiangtu.top/gtaarvclgt.html

SHOW INDEX FROM users;
来源：http://hz.jinqigufen.top/gtvlvszmzt.html

[Q73] 查看表状态
来源：http://hz.tian-w.cn/gtfllcgdba.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.haohaochexian.top/gtcuvoexcm.html

[Q74] 强制使用索引
来源：http://hz.redwolf501.top/gtqsvhfnyb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuanzx.com/gtpvaweyje.html

[Q75] 日期格式化
来源：http://hz.zhoulong.xyz/gtxnuecxkl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daxiang520.top/gtyyajissn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangkeji.top/gtqdmkeoke.html

[Q76] 按天统计
来源：http://hz.shzxlz.cn/gtnfwftqsf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sxryk.cn/gtawxziaeu.html

[Q77] 时间加减
来源：http://hz.jinghuilouyu.cn/gtdfvkafad.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ivvv.top/gtonndydft.html

[Q78] 当前时间
来源：http://hz.yanxiufei.cn/gtxsijcure.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhengqikj.top/gtabbnrcdr.html

[Q79] 字符串拼接
来源：http://hz.xuanzx.com/gtohwvjihz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hywenlv.cn/gtfknrjrnu.html

[Q80] 字符串截取
来源：http://hz.mhx1999.top/gtsrdhrlky.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aibaodan.cn/gtttfsedsa.html

[Q81] 字符串替换
来源：http://hz.smart0.xyz/gtsnlsbngs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aibaodan.cn/gtojfqdptl.html

[Q82] 字符长度与字节长度
来源：http://hz.guannengcc.top/gtxecvxrui.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aizwys.cn/gttmaipmko.html

[Q83] 大小写转换
来源：http://hz.sysykeji.top/gtpizjagrb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daria6918.cn/gtgnsnqvit.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtyiblizcc.html

SELECT TRIM(name) FROM users;
来源：http://hz.hammf.cn/gtpavtkado.html

[Q85] 数值取整
来源：http://hz.hammf.cn/gtwotheqyf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xingfuxueyuan.xyz/gtgayanrfp.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtvifjzjmh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnxiangtu.top/gtpjnxqxsp.html

[Q87] JSON 字段做条件
来源：http://hz.redwolf501.top/gtbflzujrz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtmjosjmgo.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuanzx.com/gtvixmklfc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xylfe.cn/gtmiyxmmxo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinqigufen.top/gtuagwzvbu.html

[Q89] 判断表是否存在
来源：http://hz.gaohongyu789.top/gtbzqdnjmi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtdbkpwyxa.html

[Q90] 生成序号列
来源：http://hz.pycfn.com/gttlseehna.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yonumen.top/gtszopcwqm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthcnqysgb.html

R. Bash 专题
来源：http://hz.shzxlz.cn/gtibuggkwv.html

================================================================================
来源：http://hz.hammf.cn/gtmyyiliba.html

[R01] shebang 与严格模式
来源：http://hz.aizwys.cn/gtczzmxwwl.html

#!/usr/bin/env bash
来源：http://hz.daxiang520.top/gtfnqpivqj.html

set -euo pipefail
来源：http://hz.nanxinkj.top/gtrmhtdzbf.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtonzpniwj.html

name="Tom"; echo "$name"
来源：http://hz.xingfuxueyuan.xyz/gtgailzepb.html

[R03] 只读变量
来源：http://hz.dashuyun.cn/gttgmpuivw.html

readonly PI=3.14
来源：http://hz.zhijiandao.cn/gtgxpaermw.html

[R04] 位置参数
来源：http://hz.zdqjudy.top/gthfxdpvku.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fzhhl.top/gtrnbwlgkh.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtlbxwcwln.html

name="${1:-default}"
来源：http://hz.kuanghao11.cn/gtxllusbgf.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtdwetbtbo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aibaodan.cn/gtsjbhkfhg.html

[R07] if 判断文件
来源：http://hz.yuanzhike.top/gtzxgwyxvq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gotoacloud.top/gtadyealpf.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtywwvyuwr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangtech.top/gtkysbapuk.html

[R09] 字符串比较
来源：http://hz.shuidangran.top/gttkrokbiv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.316326.xyz/gtdsxmhmgq.html

[R10] 正则匹配
来源：http://hz.xuanzx.com/gtpqgcmopv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258888.top/gtrxhbungu.html

[R11] case 多分支
来源：http://hz.gzhubu.top/gtuzuofrgo.html

case "$1" in
来源：http://hz.yj20258888.top/gtdqmxxzar.html

start) echo "启动" ;;
来源：http://hz.nwbrower.top/gtvtkvjkjb.html

stop)  echo "停止" ;;
来源：http://hz.zhongyouzk.top/gtjoqqoiau.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gtsdwuuppo.html

esac
来源：http://hz.yangfankeji.com/gtvfckgrzm.html

[R12] for 遍历文件
来源：http://hz.iojbl.cn/gttqrfhdxh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgfzy.top/gtaefrnauq.html

[R13] for 计数循环
来源：http://hz.jinghuilouyu.cn/gtspdipwbl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigufen.top/gtbiagpypd.html

[R14] C 风格 for
来源：http://hz.bjfxy.top/gtmpcsjorh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtsgcscobm.html

[R15] while 逐行读文件
来源：http://hz.zhiwuduotai.top/gtlicwydrz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydzc1.top/gtzaqersye.html

[R16] until 等待条件
来源：http://hz.tianlin.xyz/gtibofgpxw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtblgwhzcc.html

[R17] 数组定义与取值
来源：http://hz.shzxlz.cn/gtrcqojkrk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydzc1.top/gtixrnfupz.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtkbexbfvt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xylfe.cn/gthixqxjwh.html

[R19] 数组长度
来源：http://hz.birdmap.top/gtjnpqnwel.html

echo "${#arr[@]}"
来源：http://hz.nanxuanxn.top/gtfuuigwax.html

[R20] 关联数组（字典）
来源：http://hz.hnxiangtu.top/gtazqmcura.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.kuanghao11.cn/gtkebcbqvy.html

[R21] 字符串长度
来源：http://hz.chenjidiqi.icu/gtsxssudgp.html

echo "${#s}"
来源：http://hz.gzhubu.top/gtzqobmglb.html

[R22] 截取子串
来源：http://hz.0kj1m.cn/gtwixkxbaj.html

echo "${s:0:5}"
来源：http://hz.gaohongyu789.top/gttnyqppzd.html

[R23] 字符串替换
来源：http://hz.hywenlv.cn/gtifjvmbxu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtqeqmiupe.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gtpqqginlc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gtsmnwmxiq.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgfzy.top/gtlxnumpjj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.smart0.xyz/gtcccylvcw.html

[R26] 命令替换
来源：http://hz.bjfxy.top/gtiqonbawu.html

now=$(date +%F); echo "$now"
来源：http://hz.andypj.xyz/gtqhfqenhj.html

[R27] 算术展开
来源：http://hz.gotoacloud.top/gtniuwusmn.html

echo $((1 + 2 * 3))
来源：http://hz.svipenyu.cn/gtqhcvnjcd.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtpjxfrjez.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gtvipubxst.html

[R29] 定义函数
来源：http://hz.ydzc1.top/gtbwdaooqu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ppjwa.cn/gthjvfsdei.html

[R30] 函数返回状态码
来源：http://hz.yuanzhike.top/gtnudcaoex.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jyoumei.cn/gtkphynxiq.html

[R31] 局部变量
来源：http://hz.nanxuanxn.top/gtnyqbzmtz.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxuanxn.top/gtcwnrmxaz.html

[R32] 参数个数校验
来源：http://hz.yongpay.top/gtgbjuggsw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guowangkeji.top/gtnjstlnlw.html

[R33] 捕获错误并提示行号
来源：http://hz.cqqwz.cn/gthkxxlxmr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhoulong.xyz/gtsqeaodpa.html

[R34] 退出时清理
来源：http://hz.pycfn.com/gterrbqsqv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gticbeuhwz.html

[R35] 后台执行并等待
来源：http://hz.cheryme.top/gtjjuylerq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cdnleiting.top/gtcwghqtcz.html

[R36] 并发执行多个任务
来源：http://hz.guowangkeji.top/gtuyigwggl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.andypj.xyz/gtgwkeldgx.html

[R37] 把输出赋给变量
来源：http://hz.gaohongyu789.top/gteoawacal.html

files=$(ls -1)
来源：http://hz.jlsjyb.cn/gttupqjquk.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtsrebluay.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aibaodan.cn/gtntldwrea.html

[R39] 重定向标准输出与错误
来源：http://hz.hywenlv.cn/gtqpauspok.html

cmd > out.log 2>&1
来源：http://hz.xziqi.cn/gtqpjgzhxs.html

[R40] 追加写日志
来源：http://hz.zhengqikj.top/gtivgemfri.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gtevtpytyq.html

[R41] 丢弃输出
来源：http://hz.vqdsnc.cn/gtrpyxiiok.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtnwyofjiy.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtmdbljybq.html

wc -l < a.txt
来源：http://hz.52xcode.cn/gtgkcxlako.html

[R43] 按名字查找文件
来源：http://hz.wangshuangyany.cn/gtwnbvwptz.html

find . -name "*.log" -type f
来源：http://hz.hnqzz.top/gtaqeklgqh.html

[R44] 按修改时间查找
来源：http://hz.sysykeji.top/gtozxqqgtj.html

find . -mtime -7 -type f
来源：http://hz.nanxuanxn.top/gtuqwflhjx.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtrswscayj.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258.top/gtmmbbqhfa.html

[R46] 递归替换文件内容
来源：http://hz.cucudq.cn/gtrfrmqkiz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hysaishi.cn/gttzohetyc.html

[R47] sed 单行替换
来源：http://hz.xuetiantiany.cn/gtqpjnpytb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.meibo888.top/gtangqkgfe.html

[R48] awk 取指定列
来源：http://hz.hfpthk.cn/gtplxszake.html

awk '{print $1, $3}' a.txt
来源：http://hz.meibo888.top/gtzbhrmrvj.html

[R49] awk 带条件
来源：http://hz.cqqwz.cn/gtkjifyunv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tanke756.top/gtyzruxsby.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gteoorhwmy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sysykeji.top/gtojapifdy.html

[R51] 排序去重取前几
来源：http://hz.guannengcc.top/gtlnvzfdda.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cqqwz.cn/gtlksvzxej.html

[R52] 统计行数
来源：http://hz.yj20258888.top/gtyhspbcqn.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gtxzghcljx.html

[R53] 查看文件头与实时尾
来源：http://hz.wangshuangyany.cn/gtebnlpzcb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tian-w.cn/gtdnlhetnk.html

[R54] 比较两个文件
来源：http://hz.daxiang520.top/gtnzuveguw.html

diff a.txt b.txt
来源：http://hz.zhijiandao.cn/gtrrjfzgoz.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtvdpqzngo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhaomingkeji.xyz/gtlwwrcnmy.html

[R56] 远程拷贝
来源：http://hz.jianghu66.top/gtscoorfhm.html

scp file user@host:/path/
来源：http://hz.nwbrower.top/gtupjynubv.html

[R57] 远程执行命令
来源：http://hz.yj202588.top/gtcnjmkcii.html


<!-- 参考信息 -->