代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtbxqgfpro.html

[Q07] 删除表
来源：http://hz.dianchejie.cn/gtsvvtrzin.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xziqi.cn/gtozahuncu.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtutdbocpu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sufxvd.cn/gttzatmqdf.html

[Q09] 创建唯一索引
来源：http://hz.ivvv.top/gtbhprstow.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gtwrcucygo.html

[Q10] 插入单行
来源：http://hz.nanxinkj.top/gtgnyagryl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sysykeji.top/gtixrsxmuq.html

[Q11] 一次插入多行
来源：http://hz.gogol.net.cn/gtefdvmhyk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gthvbzkfik.html

[Q12] 插入后取自增 ID
来源：http://hz.jiagoushi.top/gtlrzxgolz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.bjfxy.top/gtukveuuam.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtfijelpom.html

[Q13] 忽略重复插入
来源：http://hz.jinyuanbaomall.cn/gtyxpqqore.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtkxqqnivc.html

[Q14] 存在则更新（upsert）
来源：http://hz.quarkkingdee.top/gtdshgiktc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jianghu66.top/gtqeleuybv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhengqikj.top/gtfjuddvui.html

[Q15] 查询全部
来源：http://hz.nwbrower.top/gtthjvuljs.html

SELECT * FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtzonrohdv.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gttsbnumzz.html

SELECT id, name FROM users;
来源：http://hz.jinyuanbaomall.cn/gtnblfeduf.html

[Q17] 条件查询
来源：http://hz.pengpengdd.cyou/gtypclwgeb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj20258.top/gtsyaxyvuk.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtzzimnfpw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guowangkeji.top/gtglfpuees.html

[Q19] 范围查询
来源：http://hz.dashuyun.cn/gthuakoeyo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gteryqptfp.html

[Q20] IN 列表
来源：http://hz.daxiang520.top/gtosfgtcyw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.c1oappe.top/gtblhtgjim.html

[Q21] 空值判断
来源：http://hz.nanxuanxn.top/gtrdiqmnih.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gogol.net.cn/gtcyxptafq.html

[Q22] 排序
来源：http://hz.xuanzx.com/gtiiwkzkvv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sxryk.cn/gtooyxrkef.html

[Q23] 分页
来源：http://hz.xylfe.cn/gtvegatozp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dashuyun.cn/gtzdpawfkk.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gtinpjgpdj.html

SELECT DISTINCT city FROM users;
来源：http://hz.nwbrower.top/gticadlbcw.html

[Q25] 只取前 N 条
来源：http://hz.jlsjyb.cn/gtlrwgefph.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.iojbl.cn/gtztyguafk.html

[Q26] 计数
来源：http://hz.tianlin.xyz/gtqjqabigf.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj202588.top/gtlupjnrkd.html

[Q27] 条件计数
来源：http://hz.hongshengwenyu.top/gtymxwkqvw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.redwolf501.top/gtmazoitjw.html

[Q28] 求和与平均
来源：http://hz.hongshengwenyu.top/gtndqlpfbx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tianlin.xyz/gtcvsljkft.html

[Q29] 最大最小值
来源：http://hz.hysaishi.cn/gtnoebcuzw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtyitcvraq.html

[Q30] 分组统计
来源：http://hz.svipenyu.cn/gtzwexbavp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtkeeupeac.html

[Q31] 分组后过滤
来源：http://hz.iojbl.cn/gtodaxqlel.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hongshengwenyu.top/gtsfgyqvzd.html

[Q32] 分组拼接字符串
来源：http://hz.jyoumei.cn/gtzxqxxyju.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtacygchks.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tian-w.cn/gtqpcdxstn.html

[Q33] 多列分组
来源：http://hz.hammf.cn/gtlgruoeed.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtstprirqf.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtdbchrrpa.html

SELECT * FROM (
来源：http://hz.yonumen.top/gttbpbmrfv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sweek.top/gtcwhxghms.html

) t WHERE rn = 1;
来源：http://hz.jinghuilouyu.cn/gtjhoiatev.html

[Q35] 内连接
来源：http://hz.ybcxt.top/gtoizpnuuo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtbfwsqsfs.html

[Q36] 左连接
来源：http://hz.jyoumei.cn/gtnfldrqhn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtqpsilvaj.html

[Q37] 右连接
来源：http://hz.316326.xyz/gtpxbfpssm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgfzy.top/gtnqeupwod.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhoulong.xyz/gtgpjtfhmd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cdnleiting.top/gtonilgndn.html

[Q39] 自连接（查上下级）
来源：http://hz.9152youxi.cn/gtjkpwcscz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shuidangran.top/gtnqebkcca.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cdnleiting.top/gtuxfhrhtz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hywenlv.cn/gtavvuowao.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.9152youxi.cn/gtrhkeuwlo.html

[Q41] 多表连接
来源：http://hz.yj20258.top/gtpwdboezy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zdqjudy.top/gtrnubowzm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shuidangran.top/gtvaahoyvr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxuanxn.top/gtebgtsfab.html

[Q42] 连接条件附加过滤
来源：http://hz.xylfe.cn/gtgwdqbpvr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hammf.cn/gtosqbvaom.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shzxlz.cn/gtkougczgt.html

[Q43] 标量子查询
来源：http://hz.nanxinkj.top/gtoegvuuri.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.316326.xyz/gtudfdyckw.html

[Q44] IN 子查询
来源：http://hz.yvedp.cn/gtqormzkyg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxinkj.top/gtqumyhltx.html

[Q45] EXISTS 判断存在
来源：http://hz.ydzc1.top/gtvyizyckl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtccvegfjw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sweek.top/gtqusmbhoz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtxfvgngix.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtnuewbrkn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydjk.org.cn/gtzgzdjnnt.html

[Q48] CTE 公用表表达式
来源：http://hz.xziqi.cn/gtoueewgxa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.redwolf501.top/gtkejjqkyf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenjidiqi.icu/gtqobeegzl.html

[Q49] 更新单行
来源：http://hz.yj20258.top/gtkrmahaph.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cashguo.top/gtcuqsgkmw.html

[Q50] 批量更新
来源：http://hz.yj20258888.top/gtmumgbpat.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hysaishi.cn/gtrxicymcp.html

[Q51] 用子查询更新
来源：http://hz.ppjwa.cn/gtrxmdozcv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gotoacloud.top/gtiuatxvqd.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtyzctqrff.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtomutllwj.html

[Q53] 按条件删除
来源：http://hz.hongshengwenyu.top/gtuybwiakl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shzxlz.cn/gtvvvilpev.html

[Q54] 清空表
来源：http://hz.zhiwuduotai.top/gtgkdbsdxo.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtoewknhkw.html

[Q55] 排名（并列占位）
来源：http://hz.ybcxt.top/gtgpqshfkj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.kuanghao11.cn/gtsalxcdvf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydjk.org.cn/gtdqcssfzh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.havefunace.top/gtppwufbbv.html

[Q57] 行号
来源：http://hz.cdnleiting.top/gtnslvowxl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.c1oappe.top/gtuusbvubs.html

[Q58] 累计求和
来源：http://hz.vqdsnc.cn/gtbrfcasyo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangdashe.top/gtbynpcxuv.html

[Q59] 分组内累计
来源：http://hz.jinyuanbaomall.cn/gtkolajgmx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangdashe.top/gtkicpiuwx.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenzaomai.com/gtgrqhwdlf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhixingplan.top/gtctinjiig.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cheryme.top/gtjywkbdmg.html

[Q61] 移动平均
来源：http://hz.daxiang520.top/gtwuccdngr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yongpay.top/gtlnxavgxl.html

[Q62] 分组占比
来源：http://hz.xziqi.cn/gtccwzzwaj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtkvuzdjki.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtlimfxlof.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cucudq.cn/gtcgngzsjf.html

[Q64] 提交事务
来源：http://hz.0kj1m.cn/gtiigrzgrp.html

COMMIT;
来源：http://hz.gotoacloud.top/gtytnryxfh.html

[Q65] 回滚事务
来源：http://hz.tian-w.cn/gtkpkcomii.html

ROLLBACK;
来源：http://hz.nanxinkj.top/gttjsuuurk.html

[Q66] 行锁查询
来源：http://hz.dashuyun.cn/gtzynwcwol.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jlsjyb.cn/gtydzopose.html

[Q67] 设置隔离级别
来源：http://hz.wangshuangyany.cn/gtbpcnjgcg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hfpthk.cn/gtkzggpqlc.html

[Q68] 保存点
来源：http://hz.chenjidiqi.icu/gtzwnwlqeg.html

SAVEPOINT sp1;
来源：http://hz.cashguo.top/gtfcygjyxc.html

ROLLBACK TO sp1;
来源：http://hz.wangshuangyany.cn/gtfzqisxrx.html

[Q69] 查看执行计划
来源：http://hz.sweek.top/gtwpoytokt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgfzy.top/gtaotzikxu.html

[Q70] 更新统计信息
来源：http://hz.zhaomingkeji.xyz/gtukjlkfxb.html

ANALYZE TABLE users;
来源：http://hz.shuidangran.top/gtwbshbtxg.html

[Q71] 查看建表语句
来源：http://hz.iojbl.cn/gttguqtpkl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.svipenyu.cn/gtbxbhrnou.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gtjckdfrpb.html

SHOW INDEX FROM users;
来源：http://hz.nanxuanxn.top/gtajfoywxx.html

[Q73] 查看表状态
来源：http://hz.quarkkingdee.top/gtmzakuezw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guannengcc.top/gtxifumbxe.html

[Q74] 强制使用索引
来源：http://hz.gotoacloud.top/gtmsteupfn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenjidiqi.icu/gtbtezvefl.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtsdlhxmsz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtxvydtjpm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydjk.org.cn/gttubgpuba.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gtscujppmf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtjdvsutrw.html

[Q77] 时间加减
来源：http://hz.nanxinkj.top/gtafsrwdea.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gotoacloud.top/gtqlbvjeao.html

[Q78] 当前时间
来源：http://hz.cashguo.top/gtdniypiob.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guowangkeji.top/gtejowdphi.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtrzzqnice.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ybcxt.top/gtvcfqhgxl.html

[Q80] 字符串截取
来源：http://hz.yuanzhike.top/gtuxyrnnds.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xylfe.cn/gtvsoqtclj.html

[Q81] 字符串替换
来源：http://hz.chenzaomai.com/gtuhrkbfts.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.9152youxi.cn/gthhauremq.html

[Q82] 字符长度与字节长度
来源：http://hz.zycfv.cn/gtzrtvfeeq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.havefunace.top/gtqpgjtcal.html

[Q83] 大小写转换
来源：http://hz.hongshengwenyu.top/gtmbqplorj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cashguo.top/gtlhnahpvd.html

[Q84] 去除首尾空格
来源：http://hz.shzxlz.cn/gtphwyytmx.html

SELECT TRIM(name) FROM users;
来源：http://hz.hammf.cn/gtgwinkfjx.html

[Q85] 数值取整
来源：http://hz.shanyushiyangtech.top/gteqeyexuw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sysykeji.top/gtscumhiug.html

[Q86] 读取 JSON 字段
来源：http://hz.ivvv.top/gttqgqmftt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.pycfn.com/gtqckotmjm.html

[Q87] JSON 字段做条件
来源：http://hz.zhengqikj.top/gtmcypmumk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.haohaochexian.top/gtxcahdjud.html

[Q88] 行转列（条件聚合）
来源：http://hz.svipenyu.cn/gtgdvxkpdu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zycfv.cn/gtdjujdmpf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhoulong.xyz/gtqjotisnw.html

[Q89] 判断表是否存在
来源：http://hz.zycfv.cn/gtigrfrimu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dianchejie.cn/gtjmsnzbbj.html

[Q90] 生成序号列
来源：http://hz.ydjk.org.cn/gtublisyok.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hammf.cn/gtplkvchlx.html

================================================================================
来源：http://hz.hnqzz.top/gtwjnspvmo.html

R. Bash 专题
来源：http://hz.ehwqpu.com/gthyqsljgt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtadnjzpsy.html

[R01] shebang 与严格模式
来源：http://hz.sufxvd.cn/gtumpjkpaf.html

#!/usr/bin/env bash
来源：http://hz.shangyingyoupin.top/gtuchicnki.html

set -euo pipefail
来源：http://hz.cashguo.top/gtvtqdlulw.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtxmsnysis.html

name="Tom"; echo "$name"
来源：http://hz.cdnleiting.top/gtwhirmoaw.html

[R03] 只读变量
来源：http://hz.zycfv.cn/gtesgaiirm.html

readonly PI=3.14
来源：http://hz.52xcode.cn/gtzwomtboc.html

[R04] 位置参数
来源：http://hz.zhongyouzk.top/gtayrryscy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tianlin.xyz/gtowmtvqni.html

[R05] 参数默认值
来源：http://hz.nanxuanxn.top/gtegrzvsoa.html

name="${1:-default}"
来源：http://hz.redwolf501.top/gtwgmzgnzu.html

[R06] 判断命令是否存在
来源：http://hz.wangshuangyany.cn/gtrgdnpwyx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cheryme.top/gtptpmzuek.html

[R07] if 判断文件
来源：http://hz.ehwqpu.com/gtlyebswgy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hywenlv.cn/gtthoofbmc.html

[R08] 数值比较
来源：http://hz.jlsjyb.cn/gtocxqpavj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yanxiufei.cn/gthssgvkua.html

[R09] 字符串比较
来源：http://hz.yonumen.top/gtlhvtuigj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhiwuduotai.top/gtvjptznsp.html

[R10] 正则匹配
来源：http://hz.shzxlz.cn/gtaprdukis.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yonumen.top/gtepupyiqs.html

[R11] case 多分支
来源：http://hz.shuidangran.top/gttnrktzrw.html

case "$1" in
来源：http://hz.bjfxy.top/gtnbodtfxc.html

start) echo "启动" ;;
来源：http://hz.tanke756.top/gtuwbjbbvz.html

stop)  echo "停止" ;;
来源：http://hz.hnqzz.top/gtcnluoucy.html

*)     echo "未知命令" ;;
来源：http://hz.hywenlv.cn/gtlqxfzohp.html

esac
来源：http://hz.ybcxt.top/gtcfjcopcu.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gtryntsfbf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guannengcc.top/gtcifarqsr.html

[R13] for 计数循环
来源：http://hz.fengsongda.top/gtwfjefdul.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yangfankeji.com/gtfombjryk.html

[R14] C 风格 for
来源：http://hz.yuxming.cn/gtbtwndxos.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydzc1.top/gtayuefycc.html

[R15] while 逐行读文件
来源：http://hz.chenzaomai.com/gtchlktqvf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenzaomai.com/gtokxwzqfy.html

[R16] until 等待条件
来源：http://hz.hnxiangtu.top/gtewnhmihp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gttfgoyjfr.html

[R17] 数组定义与取值
来源：http://hz.nanxinkj.top/gtjsqubuua.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jlsjyb.cn/gthvoburuo.html

[R18] 遍历数组
来源：http://hz.iojbl.cn/gtsswsksyr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gtbyhgpvom.html

[R19] 数组长度
来源：http://hz.chenzaomai.com/gtqflzaoks.html

echo "${#arr[@]}"
来源：http://hz.daxiang520.top/gtrskbfgpl.html

[R20] 关联数组（字典）
来源：http://hz.hfpthk.cn/gtlsbsrtgw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cdnleiting.top/gtivojpele.html

[R21] 字符串长度
来源：http://hz.bjfxy.top/gtazljlblp.html

echo "${#s}"
来源：http://hz.yj20258.top/gtmifffuru.html

[R22] 截取子串
来源：http://hz.cucudq.cn/gtcnfggmck.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gtlanjidzb.html

[R23] 字符串替换
来源：http://hz.feifeiyinyue.top/gtosutdnuk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cashguo.top/gtwqnjwpbw.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gtgsuuyvlt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.vqdsnc.cn/gtzimfftmw.html

[R25] 去后缀 / 去前缀
来源：http://hz.sufxvd.cn/gtzlrtvrxx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuetiantiany.cn/gtdyjykqlp.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtpihnqiwe.html

now=$(date +%F); echo "$now"
来源：http://hz.xylfe.cn/gtnlnvojrz.html

[R27] 算术展开
来源：http://hz.gogol.net.cn/gtmeyyuiyy.html

echo $((1 + 2 * 3))
来源：http://hz.xinyue.icu/gtupgpljkx.html

[R28] 浮点运算
来源：http://hz.yuxming.cn/gtyvdrwrmx.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangkeji.top/gttoznxbci.html

[R29] 定义函数
来源：http://hz.cqqwz.cn/gtgvlyfxqk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yueranfly.top/gtdqwdqmpk.html

[R30] 函数返回状态码
来源：http://hz.yangfankeji.com/gtjkfyghqy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.bjfxy.top/gtrneugnje.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gtkewfspij.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangtech.top/gtjwmadjyn.html

[R32] 参数个数校验
来源：http://hz.wangdashe.top/gttkzwcmbz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtchfxmtjw.html

[R33] 捕获错误并提示行号
来源：http://hz.jiagoushi.top/gtqwivocqv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenzaomai.com/gtyxgfooyb.html

[R34] 退出时清理
来源：http://hz.fengsongda.top/gtlkjpuxug.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtszxvcdst.html

[R35] 后台执行并等待
来源：http://hz.jinyuanbaomall.cn/gtqvinfihh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gteenmijcd.html

[R36] 并发执行多个任务
来源：http://hz.jyoumei.cn/gtmvbjsbtt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhixingplan.top/gtiinkdlmg.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtdviobzws.html

files=$(ls -1)
来源：http://hz.haohaochexian.top/gtxjqgkgue.html

[R38] 管道串联
来源：http://hz.xinyue.icu/gtklsefkpj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gzhubu.top/gtbfstasax.html

[R39] 重定向标准输出与错误
来源：http://hz.yj202588.top/gtebvrqmqr.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtrzytcvjt.html

[R40] 追加写日志
来源：http://hz.pycfn.com/gtrzssdshc.html

echo "log" >> out.log
来源：http://hz.shzxlz.cn/gtmlhiqrry.html

[R41] 丢弃输出
来源：http://hz.yj202588.top/gtcgbnnamf.html

cmd >/dev/null 2>&1
来源：http://hz.zhiwuduotai.top/gtcbppmgyz.html

[R42] 输入重定向
来源：http://hz.jinghuilouyu.cn/gtsnrqkvax.html

wc -l < a.txt
来源：http://hz.gotoacloud.top/gthhhwkzwe.html

[R43] 按名字查找文件
来源：http://hz.zhixingplan.top/gthuyfwhwo.html

find . -name "*.log" -type f
来源：http://hz.gzhubu.top/gtcokppxbf.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gtzzdbllkc.html

find . -mtime -7 -type f
来源：http://hz.hnxiangtu.top/gtawoxjybc.html

[R45] 批量删除
来源：http://hz.shangyingyoupin.top/gtjvbdzhvc.html

find . -name "*.tmp" -delete
来源：http://hz.ywan-chungtsiang.top/gtmdvlsrfh.html

[R46] 递归替换文件内容
来源：http://hz.guowangkeji.top/gterpuompe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangdashe.top/gtvrxffmud.html

[R47] sed 单行替换
来源：http://hz.xuetiantiany.cn/gtyybetuba.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtavhbylhx.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangtech.top/gtfrotmpcy.html

awk '{print $1, $3}' a.txt
来源：http://hz.kuanghao11.cn/gtdvlnboun.html

[R49] awk 带条件
来源：http://hz.gogol.net.cn/gtqokeepnv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.havefunace.top/gtihoffwjp.html

[R50] awk 求和
来源：http://hz.yj20258888.top/gtrrbyzvjb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.9152youxi.cn/gtsqoqipqg.html

[R51] 排序去重取前几
来源：http://hz.nanxuanxn.top/gtzcsvlynr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydzc1.top/gtdomepnfa.html

[R52] 统计行数
来源：http://hz.sweek.top/gtuizrovxi.html

wc -l a.txt
来源：http://hz.cheryme.top/gtnezqwqtk.html

[R53] 查看文件头与实时尾
来源：http://hz.daxiang520.top/gtnhhrohzq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtrsqojyry.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtkkdnrbvf.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gtrvhzdaqn.html

[R55] 压缩与解压
来源：http://hz.52xcode.cn/gtoyjrrssq.html


<!-- 参考信息 -->