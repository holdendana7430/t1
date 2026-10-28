代发 wailian999

);
来源：http://hz.ivvv.top/gtwwamxoeg.html

[Q03] 增加列
来源：http://hz.chenlongwang.top/gtoqnvebqx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.c1oappe.top/gtnqmnnvjz.html

[Q04] 修改列类型
来源：http://hz.iojbl.cn/gtxjuzoeem.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtdrygunzy.html

[Q05] 重命名列
来源：http://hz.hammf.cn/gtopjgweor.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.haohaochexian.top/gtgocrcqwi.html

[Q06] 删除列
来源：http://hz.zhongyouzk.top/gtbkslqyfz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.birdmap.top/gtwwdrqesr.html

[Q07] 删除表
来源：http://hz.cashguo.top/gtuveoskam.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cashguo.top/gtpfjrebyh.html

[Q08] 创建普通索引
来源：http://hz.iojbl.cn/gtodfnckup.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuetiantiany.cn/gtefamyyrg.html

[Q09] 创建唯一索引
来源：http://hz.fzhhl.top/gthcsixvha.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yvedp.cn/gtdyhnvrmk.html

[Q10] 插入单行
来源：http://hz.dashuyun.cn/gtezoddzjs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangshuangyany.cn/gtibnkpzjc.html

[Q11] 一次插入多行
来源：http://hz.chenlongwang.top/gtzfmipvmx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gotoacloud.top/gtqkqbczqc.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gthfefucdp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenjidiqi.icu/gtrhwbimby.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtcttztddl.html

[Q13] 忽略重复插入
来源：http://hz.tianlin.xyz/gtmxxipahs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtieczshka.html

[Q14] 存在则更新（upsert）
来源：http://hz.sysykeji.top/gtrcnrodgs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pycfn.com/gtzuconvwp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tanke756.top/gtcngboihe.html

[Q15] 查询全部
来源：http://hz.aibaodan.cn/gtequpxfnb.html

SELECT * FROM users;
来源：http://hz.zdqjudy.top/gtkofviusv.html

[Q16] 查询指定列
来源：http://hz.cqqwz.cn/gtseoibdkl.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtfyzcvctm.html

[Q17] 条件查询
来源：http://hz.jianghu66.top/gtkmmctaio.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.pengpengdd.cyou/gttryjoqfs.html

[Q18] 模糊匹配
来源：http://hz.hfpthk.cn/gtlyqgiexl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gzhubu.top/gtxmexknsn.html

[Q19] 范围查询
来源：http://hz.yvedp.cn/gtxabfagho.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.snrcjt.cn/gtbuyxbvos.html

[Q20] IN 列表
来源：http://hz.fzhhl.top/gtmoqxrkpx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtdpnapdyf.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtoklcquvf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nwbrower.top/gtwctaxlpj.html

[Q22] 排序
来源：http://hz.sufxvd.cn/gthpkonsov.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guannengcc.top/gtxzzqxjra.html

[Q23] 分页
来源：http://hz.redwolf501.top/gtcacryhtp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtfheqwgym.html

[Q24] 去重
来源：http://hz.sxryk.cn/gtvgnqxssm.html

SELECT DISTINCT city FROM users;
来源：http://hz.jiagoushi.top/gterqjivky.html

[Q25] 只取前 N 条
来源：http://hz.zdqjudy.top/gtdaqcqdjx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ppjwa.cn/gtiurygqrn.html

[Q26] 计数
来源：http://hz.gaohongyu789.top/gtopnfldlq.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhixingplan.top/gtvdcsryvb.html

[Q27] 条件计数
来源：http://hz.wangshuangyany.cn/gtbdsumrdf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangkeji.top/gtnwmcbaab.html

[Q28] 求和与平均
来源：http://hz.xuetiantiany.cn/gtzbtyhqwt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.svipenyu.cn/gtrhndlrir.html

[Q29] 最大最小值
来源：http://hz.vqdsnc.cn/gtwiewjyox.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtzoxrdewg.html

[Q30] 分组统计
来源：http://hz.hongshengwenyu.top/gtifmobwtt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gttxbmsblj.html

[Q31] 分组后过滤
来源：http://hz.zhongyouzk.top/gtjadlkhqg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.feifeiyinyue.top/gtoxcoiaus.html

[Q32] 分组拼接字符串
来源：http://hz.yonumen.top/gtgokikpia.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gthokvflxk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.316326.xyz/gtestmcwks.html

[Q33] 多列分组
来源：http://hz.tanke756.top/gtnnsaarsr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.0kj1m.cn/gteyystbxm.html

[Q34] 每组取第一条
来源：http://hz.chenjidiqi.icu/gtgnygyggx.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtindvkhfo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tian-w.cn/gtdmmukthj.html

) t WHERE rn = 1;
来源：http://hz.yuxming.cn/gtktuzloqy.html

[Q35] 内连接
来源：http://hz.svipenyu.cn/gtgrshdyka.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gtulyngoxy.html

[Q36] 左连接
来源：http://hz.ywan-chungtsiang.top/gtdsqefdht.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtbmcrgltt.html

[Q37] 右连接
来源：http://hz.meibo888.top/gtrxjgdsjd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.0kj1m.cn/gtakvuxxqf.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gtsqlrovlf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gtimdbyfza.html

[Q39] 自连接（查上下级）
来源：http://hz.hammf.cn/gtmpcrbnnd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenzaomai.com/gtgtgrhddo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangkeji.top/gtibvqkbol.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.pengpengdd.cyou/gtkgkxxqui.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xinyue.icu/gtbvgxlebs.html

[Q41] 多表连接
来源：http://hz.jinqigufen.top/gtfvqtymsp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gteahmogls.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtrxyrqnue.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigufen.top/gtnabogzef.html

[Q42] 连接条件附加过滤
来源：http://hz.yuanzhike.top/gtozwsbilk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.kuanghao11.cn/gtxcudukif.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuanzx.com/gtevzddxac.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtbmyqnnay.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jianghu66.top/gtgkqxcnka.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gtuwjvuxgz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hfpthk.cn/gtxvpbmzkl.html

[Q45] EXISTS 判断存在
来源：http://hz.birdmap.top/gtkdkeshui.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gtcfngikxj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hongshengwenyu.top/gtrgldnwkb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtmwozlaqa.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtpmmzkfee.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhiwuduotai.top/gttfbxbgrp.html

[Q48] CTE 公用表表达式
来源：http://hz.hfpthk.cn/gtffrzzmrd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aibaodan.cn/gtnktyowxh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhiwuduotai.top/gtlwkihefm.html

[Q49] 更新单行
来源：http://hz.jyoumei.cn/gtwhqmudlj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtqnyyurfs.html

[Q50] 批量更新
来源：http://hz.andypj.xyz/gtagpbdwqi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jianghu66.top/gtnwqqtral.html

[Q51] 用子查询更新
来源：http://hz.iojbl.cn/gtmauuxamn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yueranfly.top/gtsyjbengn.html

[Q52] 删除指定行
来源：http://hz.xingfuxueyuan.xyz/gtwfvrarpz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinqigufen.top/gtofyxpnyn.html

[Q53] 按条件删除
来源：http://hz.feifeiyinyue.top/gtzudxyjuk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jyoumei.cn/gtxmjmnbyb.html

[Q54] 清空表
来源：http://hz.tian-w.cn/gtyqewgirp.html

TRUNCATE TABLE logs;
来源：http://hz.cheryme.top/gtsssfubpv.html

[Q55] 排名（并列占位）
来源：http://hz.aizwys.cn/gthrejivql.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zycfv.cn/gtrmpzwmit.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinghuilouyu.cn/gtwlfylohk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.svipenyu.cn/gtfgjugrmk.html

[Q57] 行号
来源：http://hz.mhx1999.top/gthshqcrgi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtlygihkmg.html

[Q58] 累计求和
来源：http://hz.xylfe.cn/gtzxnfkizd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gtyzjjggtm.html

[Q59] 分组内累计
来源：http://hz.zycfv.cn/gthoxfkgaw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cheryme.top/gtiqqlyggg.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtlblmlxtr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.iojbl.cn/gtgtpoxhes.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuanzhike.top/gtmoouoqzd.html

[Q61] 移动平均
来源：http://hz.yuanzhike.top/gtrhoxgvxe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shangyingyoupin.top/gthithhxlr.html

[Q62] 分组占比
来源：http://hz.sweek.top/gtxiiodawm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtxdotqwed.html

[Q63] 开启事务
来源：http://hz.yvedp.cn/gtahorcars.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtswmlbyst.html

[Q64] 提交事务
来源：http://hz.zdqjudy.top/gtzrfyjnzw.html

COMMIT;
来源：http://hz.yj202588.top/gtfmprkeju.html

[Q65] 回滚事务
来源：http://hz.zhixingplan.top/gtygqmwbsr.html

ROLLBACK;
来源：http://hz.kuanghao11.cn/gtxkvkbmln.html

[Q66] 行锁查询
来源：http://hz.chenlongwang.top/gtsksbzouw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.guowangkeji.top/gttklqkqij.html

[Q67] 设置隔离级别
来源：http://hz.havefunace.top/gtvscnwurr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gtjzpnpeii.html

[Q68] 保存点
来源：http://hz.zhongyouzk.top/gthcznbdad.html

SAVEPOINT sp1;
来源：http://hz.quarkkingdee.top/gtkyifkdma.html

ROLLBACK TO sp1;
来源：http://hz.tian-w.cn/gtfprmbpyk.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtpeunyreg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xuetiantiany.cn/gtvhhegsvo.html

[Q70] 更新统计信息
来源：http://hz.jyoumei.cn/gtvvezegio.html

ANALYZE TABLE users;
来源：http://hz.svipenyu.cn/gtttagwtzi.html

[Q71] 查看建表语句
来源：http://hz.hywenlv.cn/gtpilehfxh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtmuzakfii.html

[Q72] 查看索引
来源：http://hz.zycfv.cn/gtfijckyys.html

SHOW INDEX FROM users;
来源：http://hz.tian-w.cn/gtmiecczlm.html

[Q73] 查看表状态
来源：http://hz.mhx1999.top/gtqxudkcau.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nwbrower.top/gtkuqqopnf.html

[Q74] 强制使用索引
来源：http://hz.shangyingyoupin.top/gtlwjmvuez.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ivvv.top/gtgampaluh.html

[Q75] 日期格式化
来源：http://hz.quarkkingdee.top/gtaprwntia.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gaohongyu789.top/gtyqjbdenz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangshuangyany.cn/gtrpvwcodq.html

[Q76] 按天统计
来源：http://hz.iojbl.cn/gtctdljsei.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cucudq.cn/gtjhtwdgap.html

[Q77] 时间加减
来源：http://hz.xinyue.icu/gttgkaewup.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgufenzy.top/gtucbwyokd.html

[Q78] 当前时间
来源：http://hz.cqqwz.cn/gtovxqzlhw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.daria6918.cn/gttujjsldj.html

[Q79] 字符串拼接
来源：http://hz.hysaishi.cn/gtrpmxhinm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daxiang520.top/gtbemafxry.html

[Q80] 字符串截取
来源：http://hz.yueranfly.top/gtzxjnjomu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xylfe.cn/gtgrybfews.html

[Q81] 字符串替换
来源：http://hz.tanke756.top/gtabittdkk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtfdgvukcr.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtwvexvasm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jiagoushi.top/gtvynivibn.html

[Q83] 大小写转换
来源：http://hz.meibo888.top/gtavcloqjq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gttpipwtky.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtbflpdgxg.html

SELECT TRIM(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtwixzdehr.html

[Q85] 数值取整
来源：http://hz.daria6918.cn/gtxoimfbxb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258888.top/gtmhqjlvdo.html

[Q86] 读取 JSON 字段
来源：http://hz.xylfe.cn/gtiuaojbzw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.mhx1999.top/gtnlmbedds.html

[Q87] JSON 字段做条件
来源：http://hz.chenlongwang.top/gtewzrsxsb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gtpmkvohdp.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtisizrgog.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtqfjosqfm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.c1oappe.top/gtzsyuphiy.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gtayuzcgog.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sufxvd.cn/gtvjcqsuyl.html

[Q90] 生成序号列
来源：http://hz.cheryme.top/gtnezkxdzd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtiskaocho.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvwiabzmw.html

R. Bash 专题
来源：http://hz.9152youxi.cn/gtdoumhhya.html

================================================================================
来源：http://hz.chenlongwang.top/gtqvdyublu.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtbeuyncem.html

#!/usr/bin/env bash
来源：http://hz.shzxlz.cn/gttiilntik.html

set -euo pipefail
来源：http://hz.0kj1m.cn/gtzbzfoqat.html

[R02] 变量赋值与使用
来源：http://hz.nwbrower.top/gtfyiddiah.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gtjiwnggdl.html

[R03] 只读变量
来源：http://hz.shzxlz.cn/gtqptdzmad.html

readonly PI=3.14
来源：http://hz.yonumen.top/gtgmovnlro.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gtfigtlkew.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangshuangyany.cn/gtnehkbnjc.html

[R05] 参数默认值
来源：http://hz.dashuyun.cn/gtbhqrxpuj.html

name="${1:-default}"
来源：http://hz.tanke756.top/gtkxlnunos.html

[R06] 判断命令是否存在
来源：http://hz.nwbrower.top/gtlhfygzlo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhongyouzk.top/gtlkkwurag.html

[R07] if 判断文件
来源：http://hz.wangshuangyany.cn/gtmuozlrfo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.mhx1999.top/gthkgcmmps.html

[R08] 数值比较
来源：http://hz.andypj.xyz/gtugptzkgd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuanzx.com/gtxvpnywcg.html

[R09] 字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtbwcoblca.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenlongwang.top/gtqhxllive.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtxsaglrpe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtytxbdhoh.html

[R11] case 多分支
来源：http://hz.jyoumei.cn/gtayqjrilq.html

case "$1" in
来源：http://hz.havefunace.top/gthhoxjplp.html

start) echo "启动" ;;
来源：http://hz.zycfv.cn/gtyrywlwbx.html

stop)  echo "停止" ;;
来源：http://hz.xinyue.icu/gtklthcdhe.html

*)     echo "未知命令" ;;
来源：http://hz.zycfv.cn/gtlglemqha.html

esac
来源：http://hz.gotoacloud.top/gthzpxpluj.html

[R12] for 遍历文件
来源：http://hz.zdqjudy.top/gtnhjqhhcr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinghuilouyu.cn/gtgwqynjwv.html

[R13] for 计数循环
来源：http://hz.bjfxy.top/gtcdtgvclr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gtwztkjryg.html

[R14] C 风格 for
来源：http://hz.xuetiantiany.cn/gtdosgquyd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhengqikj.top/gtisfjaoqu.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtixgzkoni.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gthrzkznpn.html

[R16] until 等待条件
来源：http://hz.yuanzhike.top/gtxjsdmpwz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.9152youxi.cn/gtrxxvngfm.html

[R17] 数组定义与取值
来源：http://hz.yongpay.top/gtimwliwnm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gttyehwwzk.html

[R18] 遍历数组
来源：http://hz.zhaomingkeji.xyz/gthwtracbg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.52xcode.cn/gtuqxjobvb.html

[R19] 数组长度
来源：http://hz.yueranfly.top/gtfqgcsiqv.html

echo "${#arr[@]}"
来源：http://hz.fzhhl.top/gtfibbqprp.html

[R20] 关联数组（字典）
来源：http://hz.ivvv.top/gtzklmmfzp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gtxwlctyfz.html

[R21] 字符串长度
来源：http://hz.ywan-chungtsiang.top/gtuztacvsy.html

echo "${#s}"
来源：http://hz.nanxuanxn.top/gtchbobjda.html

[R22] 截取子串
来源：http://hz.hongshengwenyu.top/gtaewkwcnn.html

echo "${s:0:5}"
来源：http://hz.iojbl.cn/gtsqfkzbxr.html

[R23] 字符串替换
来源：http://hz.sweek.top/gtatwefjnn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gtthlcneok.html

[R24] 大小写转换
来源：http://hz.shuidangran.top/gttubrqfic.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sysykeji.top/gtkqsbrsmc.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gttlidboru.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtdyxkmcua.html

[R26] 命令替换
来源：http://hz.shanyushiyangtech.top/gtwomamumc.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gtbsjfelkj.html

[R27] 算术展开
来源：http://hz.smart0.xyz/gtfazqmpuh.html

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtethynqrv.html

[R28] 浮点运算
来源：http://hz.guowangkeji.top/gtszgeppky.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gtocckzual.html

[R29] 定义函数
来源：http://hz.redwolf501.top/gtqwpkfiin.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtahuatqxe.html

[R30] 函数返回状态码
来源：http://hz.0kj1m.cn/gtrumnluen.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cdnleiting.top/gtkxjxbcir.html

[R31] 局部变量
来源：http://hz.pycfn.com/gtporvlmpd.html

f() { local x=1; echo "$x"; }
来源：http://hz.andypj.xyz/gtfppdhcrh.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtupafuxjb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tanke756.top/gtsvhzculb.html

[R33] 捕获错误并提示行号
来源：http://hz.hfpthk.cn/gtfsrxmabn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtlaqdxcbx.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gthxxmilto.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtaxepgipk.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gtjfdogltp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.andypj.xyz/gticycybzb.html

[R36] 并发执行多个任务
来源：http://hz.nanxinkj.top/gtvkfeqtfj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.52xcode.cn/gtbmkjwhpj.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtvmohtygb.html

files=$(ls -1)
来源：http://hz.52xcode.cn/gtrzmixnnr.html

[R38] 管道串联
来源：http://hz.tianlin.xyz/gtzhdjilzx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cheryme.top/gtmwughpjc.html

[R39] 重定向标准输出与错误
来源：http://hz.jyoumei.cn/gtryddnyps.html

cmd > out.log 2>&1
来源：http://hz.cdnleiting.top/gtlgtpelkl.html

[R40] 追加写日志
来源：http://hz.shuidangran.top/gtqpfihrqv.html

echo "log" >> out.log
来源：http://hz.feifeiyinyue.top/gtuzawywed.html

[R41] 丢弃输出
来源：http://hz.xuanzx.com/gtlydtmedo.html

cmd >/dev/null 2>&1
来源：http://hz.jqgfzy.top/gtjoltujnf.html

[R42] 输入重定向
来源：http://hz.yj20258.top/gtdyjepxkh.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gtkddtmoap.html

[R43] 按名字查找文件
来源：http://hz.jiagoushi.top/gtwwdrxamr.html

find . -name "*.log" -type f
来源：http://hz.dianchejie.cn/gtiokbxqfn.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gtqoiqntzl.html

find . -mtime -7 -type f
来源：http://hz.cheryme.top/gtseaolmjz.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtiaoviehm.html

find . -name "*.tmp" -delete
来源：http://hz.xylfe.cn/gthyfvcsom.html

[R46] 递归替换文件内容
来源：http://hz.haohaochexian.top/gtestcwmsl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnqzz.top/gtebalopsy.html

[R47] sed 单行替换
来源：http://hz.jianghu66.top/gtrvkmnrbt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nwbrower.top/gtagowpigr.html

[R48] awk 取指定列
来源：http://hz.nanxuanxn.top/gthxtlpvux.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgfzy.top/gtirohkbsw.html

[R49] awk 带条件
来源：http://hz.andypj.xyz/gtmchgjgpf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgfzy.top/gtqjatvolb.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gtzxcqtomf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenjidiqi.icu/gtehvnzvas.html

[R51] 排序去重取前几
来源：http://hz.zhongyouzk.top/gtwuizqbky.html


<!-- 参考信息 -->