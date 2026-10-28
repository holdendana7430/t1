代发 wailian999

);
来源：http://hz.jyoumei.cn/gtbbaooujj.html

[Q03] 增加列
来源：http://hz.yangfankeji.com/gtotykhlqj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xziqi.cn/gtuijsjbdc.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtlkupuiod.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shanyushiyangkeji.top/gtrljsgwze.html

[Q05] 重命名列
来源：http://hz.nanxuanxn.top/gtefortlmo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.0kj1m.cn/gtgkdcswra.html

[Q06] 删除列
来源：http://hz.hywenlv.cn/gtmwxwklpp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtczzzyrym.html

[Q07] 删除表
来源：http://hz.kuanghao11.cn/gtrkpcexut.html

DROP TABLE IF EXISTS orders;
来源：http://hz.bjfxy.top/gtfetmivtr.html

[Q08] 创建普通索引
来源：http://hz.ivvv.top/gtzdjjzpne.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtvmgfcsbf.html

[Q09] 创建唯一索引
来源：http://hz.zhongyouzk.top/gtljolromn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtkjonfnad.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtnfvmdasi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hywenlv.cn/gtzcktwvzl.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gtqkbhqpwn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.redwolf501.top/gtqiyzneha.html

[Q12] 插入后取自增 ID
来源：http://hz.smart0.xyz/gtfevozxst.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shuidangran.top/gtnchfidaq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gteqhdtsbs.html

[Q13] 忽略重复插入
来源：http://hz.jinyuanbaomall.cn/gtvobkziop.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gtjnjmlpoe.html

[Q14] 存在则更新（upsert）
来源：http://hz.c1oappe.top/gtaihebwsb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenzaomai.com/gtpjntwjuh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.0kj1m.cn/gtnmnoipsq.html

[Q15] 查询全部
来源：http://hz.jqgufenzy.top/gthlkpucui.html

SELECT * FROM users;
来源：http://hz.guannengcc.top/gtwwlzdejy.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtqsbvqcqi.html

SELECT id, name FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtstxncbtu.html

[Q17] 条件查询
来源：http://hz.cucudq.cn/gtosgqougr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.feifeiyinyue.top/gtiewewtnt.html

[Q18] 模糊匹配
来源：http://hz.wangshuangyany.cn/gtkkhohmgm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.snrcjt.cn/gtnkylolqu.html

[Q19] 范围查询
来源：http://hz.hywenlv.cn/gtrtivcszt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jlsjyb.cn/gtdnynrfjz.html

[Q20] IN 列表
来源：http://hz.yj20258.top/gtcwyvmvza.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.daxiang520.top/gtsubexbva.html

[Q21] 空值判断
来源：http://hz.c1oappe.top/gteplxczhw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangshuangyany.cn/gtfvejwhdz.html

[Q22] 排序
来源：http://hz.jinqigfzy.top/gtuqjrhsgm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.316326.xyz/gthvjrrjfy.html

[Q23] 分页
来源：http://hz.ehwqpu.com/gtzsylhxpu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtloklaggq.html

[Q24] 去重
来源：http://hz.ywan-chungtsiang.top/gtsjnjvyxh.html

SELECT DISTINCT city FROM users;
来源：http://hz.cucudq.cn/gtzzpiurgv.html

[Q25] 只取前 N 条
来源：http://hz.zhixingplan.top/gthhtcppxb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtrofppxjd.html

[Q26] 计数
来源：http://hz.hongshengwenyu.top/gtybfybuls.html

SELECT COUNT(*) FROM users;
来源：http://hz.bjfxy.top/gtvtqmqzwe.html

[Q27] 条件计数
来源：http://hz.c1oappe.top/gtutfsuhzv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tianlin.xyz/gtnpkkbeza.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gtiapwuzmr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtxpxghcdk.html

[Q29] 最大最小值
来源：http://hz.aizwys.cn/gtahkjievs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cheryme.top/gtktzfceao.html

[Q30] 分组统计
来源：http://hz.xingfuxueyuan.xyz/gterqtfefc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtqzfvxhor.html

[Q31] 分组后过滤
来源：http://hz.iojbl.cn/gtmualgwxo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtbhnzcatx.html

[Q32] 分组拼接字符串
来源：http://hz.aibaodan.cn/gtthycxwtk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtmpqnunxb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yonumen.top/gtklefkirk.html

[Q33] 多列分组
来源：http://hz.zhiwuduotai.top/gtkzmgrrxi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gtmcudbjgb.html

[Q34] 每组取第一条
来源：http://hz.hammf.cn/gtutybbtwd.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gtzyfenwds.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhaomingkeji.xyz/gtishhgjve.html

) t WHERE rn = 1;
来源：http://hz.yuxming.cn/gtgppwxprf.html

[Q35] 内连接
来源：http://hz.gotoacloud.top/gtmngvgedf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.aibaodan.cn/gtzdwooqwc.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtuysmdrua.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtqtkbytkw.html

[Q37] 右连接
来源：http://hz.ybcxt.top/gtbeqmstgf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cashguo.top/gtocfxomce.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.smart0.xyz/gtqucorxbt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuanzhike.top/gtinivwvmh.html

[Q39] 自连接（查上下级）
来源：http://hz.pengpengdd.cyou/gtfhvcwyrm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gtiucovbiv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gthebmvrhl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenzaomai.com/gtdwsogljn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxuanxn.top/gtvzdwfarn.html

[Q41] 多表连接
来源：http://hz.yonumen.top/gtzjqlfhnd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtphndxmra.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ywan-chungtsiang.top/gtxxhyvinp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cashguo.top/gtfygimruu.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gtgofvjavj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenzaomai.com/gtuwpiomkc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgufenzy.top/gtyhahgkzy.html

[Q43] 标量子查询
来源：http://hz.jinqigufen.top/gtzoxnzfpo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258888.top/gtcvlcckmu.html

[Q44] IN 子查询
来源：http://hz.ydjk.org.cn/gtofrxcsku.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hnxiangtu.top/gtjaelauel.html

[Q45] EXISTS 判断存在
来源：http://hz.hammf.cn/gtrwnswxqy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtogjsqyep.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gtvtfbbtys.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fzhhl.top/gtcvgjscee.html

[Q47] 与平均值比较
来源：http://hz.dashuyun.cn/gteijyqvxo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yongpay.top/gtpomciwcd.html

[Q48] CTE 公用表表达式
来源：http://hz.jlsjyb.cn/gthnxqgtky.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daxiang520.top/gtswinkzad.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtguntegbg.html

[Q49] 更新单行
来源：http://hz.sufxvd.cn/gtrlshdchw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenzaomai.com/gtjswmirbx.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtyfhajzcw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtpvoreqyd.html

[Q51] 用子查询更新
来源：http://hz.snrcjt.cn/gtutnnhfjf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuxming.cn/gteevpkbbb.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtjodwqpzk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.birdmap.top/gtlenzrszz.html

[Q53] 按条件删除
来源：http://hz.nanxuanxn.top/gtlavloqbn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydjk.org.cn/gthpmueomo.html

[Q54] 清空表
来源：http://hz.ivvv.top/gtintctdwz.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigfzy.top/gtxpkwhnkg.html

[Q55] 排名（并列占位）
来源：http://hz.dianchejie.cn/gtlnweizoe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhengqikj.top/gttwvegzfh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pycfn.com/gtgassizpu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtnpwipnfs.html

[Q57] 行号
来源：http://hz.nwbrower.top/gtghqvokwu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yvedp.cn/gtgvepinyt.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtjaucltlp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gzhubu.top/gtuxhotsnx.html

[Q59] 分组内累计
来源：http://hz.fzhhl.top/gtmewoocnc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxinkj.top/gtfhfvvtfb.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gtpfwedvrf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.c1oappe.top/gtdkbjpznq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hysaishi.cn/gtakiskbqq.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtghzphxcd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj20258.top/gtknyajxiw.html

[Q62] 分组占比
来源：http://hz.ydjk.org.cn/gtjenvckly.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtdbeshsff.html

[Q63] 开启事务
来源：http://hz.haohaochexian.top/gthzeiaeaw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.0kj1m.cn/gtqolbxjax.html

[Q64] 提交事务
来源：http://hz.yanxiufei.cn/gtwtuhephv.html

COMMIT;
来源：http://hz.zhongyouzk.top/gtyrvyadkx.html

[Q65] 回滚事务
来源：http://hz.zhiwuduotai.top/gtztlltphr.html

ROLLBACK;
来源：http://hz.mhx1999.top/gteorvafcc.html

[Q66] 行锁查询
来源：http://hz.zhoulong.xyz/gtuptxlnkl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuanzhike.top/gtskxhpycn.html

[Q67] 设置隔离级别
来源：http://hz.jyoumei.cn/gtcpazzvhg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gtxfklifes.html

[Q68] 保存点
来源：http://hz.yanxiufei.cn/gtkjgqanyv.html

SAVEPOINT sp1;
来源：http://hz.zhengqikj.top/gthcvaxckp.html

ROLLBACK TO sp1;
来源：http://hz.nanxuanxn.top/gtpcoguoxl.html

[Q69] 查看执行计划
来源：http://hz.tian-w.cn/gtpgwemdoj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xingfuxueyuan.xyz/gtisgltntd.html

[Q70] 更新统计信息
来源：http://hz.sweek.top/gtpinubfmh.html

ANALYZE TABLE users;
来源：http://hz.ivvv.top/gtojpstllf.html

[Q71] 查看建表语句
来源：http://hz.tanke756.top/gtawrisylq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gtjrhdswfv.html

[Q72] 查看索引
来源：http://hz.9152youxi.cn/gtdcuaqjwi.html

SHOW INDEX FROM users;
来源：http://hz.zhixingplan.top/gtesezckdm.html

[Q73] 查看表状态
来源：http://hz.c1oappe.top/gtxrhkduqy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangtech.top/gtgcttgebw.html

[Q74] 强制使用索引
来源：http://hz.ivvv.top/gtccxjkagw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ehwqpu.com/gtdkucnwry.html

[Q75] 日期格式化
来源：http://hz.gogol.net.cn/gthuirspjp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nanxinkj.top/gtssxvzxrb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.52xcode.cn/gtuqcpzrok.html

[Q76] 按天统计
来源：http://hz.yuxming.cn/gtcwhzraai.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yanxiufei.cn/gtqgyvkzhp.html

[Q77] 时间加减
来源：http://hz.tian-w.cn/gtqnbhkaqv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtavjykdsd.html

[Q78] 当前时间
来源：http://hz.hnqzz.top/gtvemsjnpp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gotoacloud.top/gtholfmjda.html

[Q79] 字符串拼接
来源：http://hz.nanxuanxn.top/gtkkwhskos.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.52xcode.cn/gtyquofhym.html

[Q80] 字符串截取
来源：http://hz.9152youxi.cn/gtuuxfvenm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtlguxjrzm.html

[Q81] 字符串替换
来源：http://hz.ivvv.top/gttlzyiqag.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.svipenyu.cn/gtkxtbqheh.html

[Q82] 字符长度与字节长度
来源：http://hz.cdnleiting.top/gtdxgrnbxx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ivvv.top/gtdjldjipc.html

[Q83] 大小写转换
来源：http://hz.svipenyu.cn/gtelrvbjai.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xinyue.icu/gtbhezvwzj.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtntvpjzes.html

SELECT TRIM(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtnxaaelzj.html

[Q85] 数值取整
来源：http://hz.52xcode.cn/gtrjnvqnja.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenjidiqi.icu/gtuhovaohh.html

[Q86] 读取 JSON 字段
来源：http://hz.jqgufenzy.top/gttpbnnbio.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sysykeji.top/gtkxxpvnho.html

[Q87] JSON 字段做条件
来源：http://hz.yanxiufei.cn/gtxakaqjim.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gtflbtgtki.html

[Q88] 行转列（条件聚合）
来源：http://hz.0kj1m.cn/gtysutwbtb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yuanzhike.top/gtrvjrgeyf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtgviwnkib.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gtmfmeadbk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtkamamgkp.html

[Q90] 生成序号列
来源：http://hz.aizwys.cn/gtnnibejqj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gttdcwgwpy.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtnhnqbaox.html

R. Bash 专题
来源：http://hz.fengsongda.top/gtwzpgydip.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwkzkojri.html

[R01] shebang 与严格模式
来源：http://hz.316326.xyz/gtidoguqpw.html

#!/usr/bin/env bash
来源：http://hz.xziqi.cn/gtmdgmcvrs.html

set -euo pipefail
来源：http://hz.ppjwa.cn/gtrrryenig.html

[R02] 变量赋值与使用
来源：http://hz.yj20258.top/gtsbtabtfy.html

name="Tom"; echo "$name"
来源：http://hz.gogol.net.cn/gtacnbkrsl.html

[R03] 只读变量
来源：http://hz.zhongyouzk.top/gtxnrivdku.html

readonly PI=3.14
来源：http://hz.xziqi.cn/gtfzxdkclr.html

[R04] 位置参数
来源：http://hz.xingfuxueyuan.xyz/gtcgxajcgk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.feifeiyinyue.top/gthagjjiuk.html

[R05] 参数默认值
来源：http://hz.shangyingyoupin.top/gtmhskyugc.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtfnxgonqs.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtylkbotjb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yanxiufei.cn/gtxausaqum.html

[R07] if 判断文件
来源：http://hz.gogol.net.cn/gtmffokgjz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnqzz.top/gtravmuchs.html

[R08] 数值比较
来源：http://hz.yj202588.top/gtnqdazmmg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.birdmap.top/gtzexmfdfd.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtlrawckve.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigufen.top/gtoyscfsop.html

[R10] 正则匹配
来源：http://hz.yonumen.top/gtdwrzbjlz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.iojbl.cn/gtbeanzvgm.html

[R11] case 多分支
来源：http://hz.wangdashe.top/gtfrtbusfs.html

case "$1" in
来源：http://hz.hnxiangtu.top/gtjtescfer.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gtrjtqeqxo.html

stop)  echo "停止" ;;
来源：http://hz.aizwys.cn/gtzhjihpcl.html

*)     echo "未知命令" ;;
来源：http://hz.316326.xyz/gtvvqkjarl.html

esac
来源：http://hz.hammf.cn/gtivqymykh.html

[R12] for 遍历文件
来源：http://hz.guowangkeji.top/gtmdgxaeff.html

for f in *.txt; do echo "$f"; done
来源：http://hz.iojbl.cn/gtugjjuong.html

[R13] for 计数循环
来源：http://hz.xziqi.cn/gtcrvuiuiq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.snrcjt.cn/gtpygvlcxu.html

[R14] C 风格 for
来源：http://hz.aizwys.cn/gtnomltryc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnqzz.top/gtsjzaedcl.html

[R15] while 逐行读文件
来源：http://hz.haohaochexian.top/gtjgrhctmf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuanzhike.top/gtgvunpzqk.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gtxipyehoz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.birdmap.top/gtibzqrqro.html

[R17] 数组定义与取值
来源：http://hz.ydzc1.top/gtatmdaxps.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zdqjudy.top/gtelazmohe.html

[R18] 遍历数组
来源：http://hz.sweek.top/gtvokgcebi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gtiequuhsl.html

[R19] 数组长度
来源：http://hz.zycfv.cn/gtatmgzelq.html

echo "${#arr[@]}"
来源：http://hz.nanxuanxn.top/gtmvrlzmou.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtbzhziyge.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yongpay.top/gtjxbahbgf.html

[R21] 字符串长度
来源：http://hz.ybcxt.top/gtcjhpmlyw.html

echo "${#s}"
来源：http://hz.yueranfly.top/gtflieahec.html

[R22] 截取子串
来源：http://hz.yj20258888.top/gtcjyenuky.html

echo "${s:0:5}"
来源：http://hz.yj202588.top/gtwzxmzdzl.html

[R23] 字符串替换
来源：http://hz.zhixingplan.top/gtjphwduoe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinghuilouyu.cn/gtftaiscjn.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtwhtrgywg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tian-w.cn/gtrgklxsym.html

[R25] 去后缀 / 去前缀
来源：http://hz.cashguo.top/gtilyeaytp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guannengcc.top/gtajqgkegl.html

[R26] 命令替换
来源：http://hz.yj202588.top/gtjunlpxgt.html

now=$(date +%F); echo "$now"
来源：http://hz.aibaodan.cn/gtzwujbhhp.html

[R27] 算术展开
来源：http://hz.sweek.top/gtjnbbvyux.html

echo $((1 + 2 * 3))
来源：http://hz.tianlin.xyz/gtusulnoce.html

[R28] 浮点运算
来源：http://hz.smart0.xyz/gtmqhscfzn.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtxnidevwt.html

[R29] 定义函数
来源：http://hz.andypj.xyz/gtgszuecoh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yongpay.top/gtyoyrgbjz.html

[R30] 函数返回状态码
来源：http://hz.gotoacloud.top/gtvcluawkm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gtfphvhdgy.html

[R31] 局部变量
来源：http://hz.yuxming.cn/gtsmrzjupt.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydzc1.top/gtcvsbptup.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtuvcavcot.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtgvgbpeyn.html

[R33] 捕获错误并提示行号
来源：http://hz.cdnleiting.top/gtfsutnaqf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.andypj.xyz/gtpucnaowx.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtsynxcglc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtcjizfbcl.html

[R35] 后台执行并等待
来源：http://hz.yongpay.top/gtcerjjnfv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gtxzesguyq.html

[R36] 并发执行多个任务
来源：http://hz.kuanghao11.cn/gtcfvjvgzj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgufenzy.top/gtwafozxbc.html

[R37] 把输出赋给变量
来源：http://hz.xinyue.icu/gtidyyejun.html

files=$(ls -1)
来源：http://hz.haohaochexian.top/gtmimylhtt.html

[R38] 管道串联
来源：http://hz.xziqi.cn/gttnlbpsgx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zycfv.cn/gtpuozzrvf.html

[R39] 重定向标准输出与错误
来源：http://hz.xinyue.icu/gtmiaafkog.html

cmd > out.log 2>&1
来源：http://hz.aizwys.cn/gtgsrnoqnx.html

[R40] 追加写日志
来源：http://hz.nwbrower.top/gtxpbgwbub.html

echo "log" >> out.log
来源：http://hz.zhixingplan.top/gttkwokpok.html

[R41] 丢弃输出
来源：http://hz.mhx1999.top/gtdyidmjks.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtmhcnzvdz.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtlzhwexdk.html

wc -l < a.txt
来源：http://hz.yonumen.top/gttrtewcgk.html

[R43] 按名字查找文件
来源：http://hz.yongpay.top/gtfqeagdth.html

find . -name "*.log" -type f
来源：http://hz.hfpthk.cn/gthpbmkztx.html

[R44] 按修改时间查找
来源：http://hz.xylfe.cn/gtfspipxwi.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gthrigrblt.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gtzbyysnex.html

find . -name "*.tmp" -delete
来源：http://hz.sysykeji.top/gtnnyzippz.html

[R46] 递归替换文件内容
来源：http://hz.aizwys.cn/gthsfwkntz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gttydafzvz.html

[R47] sed 单行替换
来源：http://hz.yonumen.top/gtjdetmmmh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtncyvqlfh.html

[R48] awk 取指定列
来源：http://hz.zhixingplan.top/gtgwsvexcr.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtpotzwbni.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtlsduogfg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fengsongda.top/gtdecwfjem.html

[R50] awk 求和
来源：http://hz.jqgfzy.top/gtbgjztnbq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nanxinkj.top/gtrgpksubn.html

[R51] 排序去重取前几
来源：http://hz.cashguo.top/gtpcyjpdwf.html


<!-- 参考信息 -->