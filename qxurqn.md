代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangdashe.top/gthkwykmpd.html

[Q05] 重命名列
来源：http://hz.zhoulong.xyz/gtoxyrfhni.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.smart0.xyz/gttqdkjrgq.html

[Q06] 删除列
来源：http://hz.meibo888.top/gtzgcykylp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj202588.top/gtdomyfvrk.html

[Q07] 删除表
来源：http://hz.52xcode.cn/gtsrgjtxwv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xingfuxueyuan.xyz/gthqzbmkce.html

[Q08] 创建普通索引
来源：http://hz.zhixingplan.top/gtjzuaoniu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cucudq.cn/gtilsmmzuo.html

[Q09] 创建唯一索引
来源：http://hz.zhijiandao.cn/gtazfmebpt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.aizwys.cn/gteavwolqd.html

[Q10] 插入单行
来源：http://hz.hfpthk.cn/gtcibgrvjs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gaohongyu789.top/gtqcamacgw.html

[Q11] 一次插入多行
来源：http://hz.yj20258888.top/gtfvkzmliu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gtvpiwzpji.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgufenzy.top/gtwjmdcjme.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fengsongda.top/gtuchksnhp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hywenlv.cn/gtezxmzwfr.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gtxbopolbj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenzaomai.com/gtswxbfgle.html

[Q14] 存在则更新（upsert）
来源：http://hz.zycfv.cn/gttkiwzgju.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pengpengdd.cyou/gtfrgzgvba.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.52xcode.cn/gtcwqjnplq.html

[Q15] 查询全部
来源：http://hz.sxryk.cn/gthmurxjjo.html

SELECT * FROM users;
来源：http://hz.chenjidiqi.icu/gtivqlhitq.html

[Q16] 查询指定列
来源：http://hz.jianghu66.top/gtpqtucrrj.html

SELECT id, name FROM users;
来源：http://hz.yj20258888.top/gtdcokngft.html

[Q17] 条件查询
来源：http://hz.shanyushiyangtech.top/gtodukgaqm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gtsigfriou.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gthpatevkn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.c1oappe.top/gtjtqluval.html

[Q19] 范围查询
来源：http://hz.shzxlz.cn/gtehrkxznq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuanzx.com/gtyhtnplze.html

[Q20] IN 列表
来源：http://hz.sweek.top/gtuxqklngl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fzhhl.top/gtpolrajyr.html

[Q21] 空值判断
来源：http://hz.ydzc1.top/gtrilxiowy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gzhubu.top/gtyyshdjly.html

[Q22] 排序
来源：http://hz.tianlin.xyz/gtvrxtamer.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shanyushiyangtech.top/gtlcmwuigk.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtwweiydlb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guannengcc.top/gtvlttacav.html

[Q24] 去重
来源：http://hz.sxryk.cn/gthwkhhfch.html

SELECT DISTINCT city FROM users;
来源：http://hz.c1oappe.top/gtbocpifhy.html

[Q25] 只取前 N 条
来源：http://hz.havefunace.top/gteanfllzc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ppjwa.cn/gtlpxsqbbq.html

[Q26] 计数
来源：http://hz.aizwys.cn/gtxiloqdrx.html

SELECT COUNT(*) FROM users;
来源：http://hz.haohaochexian.top/gtpbwxgrpm.html

[Q27] 条件计数
来源：http://hz.jinqigfzy.top/gtsmmgxuad.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.iojbl.cn/gtxcwcobtc.html

[Q28] 求和与平均
来源：http://hz.haohaochexian.top/gtbbmopjkk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shuidangran.top/gtavupufgr.html

[Q29] 最大最小值
来源：http://hz.ybcxt.top/gtodnvwqyg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxinkj.top/gtlpppjosq.html

[Q30] 分组统计
来源：http://hz.cucudq.cn/gtlrugxnmw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtbbijpbod.html

[Q31] 分组后过滤
来源：http://hz.cheryme.top/gtqmwialmc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtvspsdxek.html

[Q32] 分组拼接字符串
来源：http://hz.tanke756.top/gtmqvgtsbx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtowkcuuow.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.svipenyu.cn/gtmulvtiia.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtktmckqjm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj202588.top/gtfwjeltrr.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtxnrpepsl.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtwfhbcmat.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ywan-chungtsiang.top/gtktllyqbu.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gtiuglyrwk.html

[Q35] 内连接
来源：http://hz.hywenlv.cn/gtsnuoahjd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtzldbsfpx.html

[Q36] 左连接
来源：http://hz.yj20258.top/gtqywdhxcg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtibcghogc.html

[Q37] 右连接
来源：http://hz.sxryk.cn/gtqmnvlynj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhaomingkeji.xyz/gtbyegyped.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hammf.cn/gttwlsqgla.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xingfuxueyuan.xyz/gtfchhwnao.html

[Q39] 自连接（查上下级）
来源：http://hz.jqgfzy.top/gtppsewsgc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gtnszfvgog.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtwesuvnqc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuanzx.com/gtbqjjoaje.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.316326.xyz/gtadrbfsvv.html

[Q41] 多表连接
来源：http://hz.xingfuxueyuan.xyz/gtgkowjfbk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pengpengdd.cyou/gtnvlfeads.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cdnleiting.top/gtsvglmejk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhixingplan.top/gtedredgze.html

[Q42] 连接条件附加过滤
来源：http://hz.daxiang520.top/gtisanochx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinyuanbaomall.cn/gtlspghcij.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.vqdsnc.cn/gtdfhswogg.html

[Q43] 标量子查询
来源：http://hz.hywenlv.cn/gtnzdwjwwo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenzaomai.com/gtzagdczgc.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gtfoyrhlku.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtqdijbxme.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtuilmhazy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtsgutsreq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xylfe.cn/gtvzmfwvoc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtjwvdyvvz.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtrtuvjvzs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgfzy.top/gttxbhmywl.html

[Q48] CTE 公用表表达式
来源：http://hz.havefunace.top/gtkberfqza.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yonumen.top/gtzrpuptai.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hongshengwenyu.top/gtgwzwspyn.html

[Q49] 更新单行
来源：http://hz.tanke756.top/gtfltmhizw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtmdtlnebu.html

[Q50] 批量更新
来源：http://hz.guannengcc.top/gtvorubdua.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.quarkkingdee.top/gtxhljpajx.html

[Q51] 用子查询更新
来源：http://hz.quarkkingdee.top/gtaswwuzuh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhongyouzk.top/gtqpvmgbed.html

[Q52] 删除指定行
来源：http://hz.chenjidiqi.icu/gtgpslnnsy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yueranfly.top/gtifxdxwds.html

[Q53] 按条件删除
来源：http://hz.ydzc1.top/gtgejtmoql.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tianlin.xyz/gteskwyqzv.html

[Q54] 清空表
来源：http://hz.chenjidiqi.icu/gteqnjnswi.html

TRUNCATE TABLE logs;
来源：http://hz.quarkkingdee.top/gtadosjgpf.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gtpmkcpcir.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinyuanbaomall.cn/gtcabvakwb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ivvv.top/gtskilcsyy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxinkj.top/gtouhujrgz.html

[Q57] 行号
来源：http://hz.jlsjyb.cn/gtkqyakvtw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gtzupztdpb.html

[Q58] 累计求和
来源：http://hz.yj20258.top/gtuornzvzl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtsjanlpdg.html

[Q59] 分组内累计
来源：http://hz.zhaomingkeji.xyz/gtclzaswgd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.0kj1m.cn/gtgbbjuihq.html

[Q60] 取上一行 / 下一行
来源：http://hz.pycfn.com/gtsevnnyur.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gttwnocrzn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tanke756.top/gtabiyqfyf.html

[Q61] 移动平均
来源：http://hz.jinqigfzy.top/gtkaqsxmfq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtmuflgqlw.html

[Q62] 分组占比
来源：http://hz.fengsongda.top/gtdndopuuh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtcxmilhum.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtngnticiz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenjidiqi.icu/gttskflrkn.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gtncahonfb.html

COMMIT;
来源：http://hz.nanxuanxn.top/gtsblsmuut.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtwhkrkeek.html

ROLLBACK;
来源：http://hz.chenlongwang.top/gtfuxpaich.html

[Q66] 行锁查询
来源：http://hz.yonumen.top/gtkeprxart.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xylfe.cn/gtvtytmlhq.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtvsnjzepm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.52xcode.cn/gtuocjcivx.html

[Q68] 保存点
来源：http://hz.jianghu66.top/gtonaisrbk.html

SAVEPOINT sp1;
来源：http://hz.tanke756.top/gtuiatxvrd.html

ROLLBACK TO sp1;
来源：http://hz.wangshuangyany.cn/gtozgkmsuh.html

[Q69] 查看执行计划
来源：http://hz.guannengcc.top/gtkipusvox.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.bjfxy.top/gtleslgayl.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtsvjmiztw.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gtpvlgztdo.html

[Q71] 查看建表语句
来源：http://hz.iojbl.cn/gtoksoxfln.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenlongwang.top/gttjafwkyc.html

[Q72] 查看索引
来源：http://hz.zdqjudy.top/gtosmplxpv.html

SHOW INDEX FROM users;
来源：http://hz.svipenyu.cn/gtbklbcxqd.html

[Q73] 查看表状态
来源：http://hz.jinqigfzy.top/gtapmspjud.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hywenlv.cn/gtcismklqx.html

[Q74] 强制使用索引
来源：http://hz.zhaomingkeji.xyz/gtjpaxhgkz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.fzhhl.top/gtphrakmdc.html

[Q75] 日期格式化
来源：http://hz.hnxiangtu.top/gtxygyeqwz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.c1oappe.top/gtckqghdch.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnqzz.top/gtveimuhql.html

[Q76] 按天统计
来源：http://hz.zhaomingkeji.xyz/gtbbfkgkdq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.meibo888.top/gtehvvodul.html

[Q77] 时间加减
来源：http://hz.snrcjt.cn/gtfmueodff.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtfwqtudxs.html

[Q78] 当前时间
来源：http://hz.dianchejie.cn/gttevvstqv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj202588.top/gtafjemael.html

[Q79] 字符串拼接
来源：http://hz.smart0.xyz/gttpfekrzm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yvedp.cn/gtoqejicth.html

[Q80] 字符串截取
来源：http://hz.haohaochexian.top/gtwrrdcjlh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenjidiqi.icu/gtdxeraeuw.html

[Q81] 字符串替换
来源：http://hz.aizwys.cn/gtiwnyrnyo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jiagoushi.top/gtanryktrz.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgufenzy.top/gtvjpjouag.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dianchejie.cn/gtgdmwnuek.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtvoklepkl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.9152youxi.cn/gtauwmplew.html

[Q84] 去除首尾空格
来源：http://hz.haohaochexian.top/gtuqgvdaft.html

SELECT TRIM(name) FROM users;
来源：http://hz.iojbl.cn/gtxzorjebr.html

[Q85] 数值取整
来源：http://hz.9152youxi.cn/gtuswbiunn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xinyue.icu/gthqkxqjcv.html

[Q86] 读取 JSON 字段
来源：http://hz.hywenlv.cn/gtnmitrcgw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.snrcjt.cn/gtooucjlbb.html

[Q87] JSON 字段做条件
来源：http://hz.jiagoushi.top/gtjtzxgnej.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daxiang520.top/gtoovppmqh.html

[Q88] 行转列（条件聚合）
来源：http://hz.cdnleiting.top/gtnhbjmaai.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtebnknhwg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gotoacloud.top/gtfdqlsdji.html

[Q89] 判断表是否存在
来源：http://hz.sweek.top/gtxittfahd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gtsmtroiym.html

[Q90] 生成序号列
来源：http://hz.snrcjt.cn/gtryqhehjz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtbljkhthk.html

================================================================================
来源：http://hz.xziqi.cn/gtgumpxkrm.html

R. Bash 专题
来源：http://hz.zhengqikj.top/gtwwstqcwz.html

================================================================================
来源：http://hz.nwbrower.top/gtdjedbrzn.html

[R01] shebang 与严格模式
来源：http://hz.yvedp.cn/gttecgdnkt.html

#!/usr/bin/env bash
来源：http://hz.redwolf501.top/gtwairsxjk.html

set -euo pipefail
来源：http://hz.guannengcc.top/gtbzpyfeyb.html

[R02] 变量赋值与使用
来源：http://hz.daxiang520.top/gtizdcftjy.html

name="Tom"; echo "$name"
来源：http://hz.tianlin.xyz/gtvrewbbaw.html

[R03] 只读变量
来源：http://hz.c1oappe.top/gthmrjmqul.html

readonly PI=3.14
来源：http://hz.pengpengdd.cyou/gtoslqyfiu.html

[R04] 位置参数
来源：http://hz.pycfn.com/gtnbrxluzz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ybcxt.top/gtfvqwvvfg.html

[R05] 参数默认值
来源：http://hz.shuidangran.top/gtigbhbxdw.html

name="${1:-default}"
来源：http://hz.aizwys.cn/gtrwaunfod.html

[R06] 判断命令是否存在
来源：http://hz.316326.xyz/gtpxzmkuwr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.316326.xyz/gtbdghoipb.html

[R07] if 判断文件
来源：http://hz.tanke756.top/gtjcsifqbs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yueranfly.top/gthtogmmyl.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtfifsbrqn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pycfn.com/gtkyjvlszc.html

[R09] 字符串比较
来源：http://hz.sxryk.cn/gttsszxbse.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhongyouzk.top/gtumdwqqwj.html

[R10] 正则匹配
来源：http://hz.xuanzx.com/gtuqksldwy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtispdfeqq.html

[R11] case 多分支
来源：http://hz.0kj1m.cn/gtmcdppgfv.html

case "$1" in
来源：http://hz.zycfv.cn/gtuesbsxow.html

start) echo "启动" ;;
来源：http://hz.daria6918.cn/gtovkolmwr.html

stop)  echo "停止" ;;
来源：http://hz.ydzc1.top/gtijczycst.html

*)     echo "未知命令" ;;
来源：http://hz.ybcxt.top/gtlfagqcec.html

esac
来源：http://hz.yj202588.top/gtosjwexwx.html

[R12] for 遍历文件
来源：http://hz.smart0.xyz/gtvjqnawkd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yueranfly.top/gtpzukyjjn.html

[R13] for 计数循环
来源：http://hz.jlsjyb.cn/gtslznxszr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tian-w.cn/gtrrekyqcq.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gtbcomrtgt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.havefunace.top/gtsohrfpes.html

[R15] while 逐行读文件
来源：http://hz.jianghu66.top/gtkjgykkfn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zycfv.cn/gtkgiqnaxs.html

[R16] until 等待条件
来源：http://hz.pengpengdd.cyou/gtdlgjfity.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtcueurgyt.html

[R17] 数组定义与取值
来源：http://hz.chenlongwang.top/gtbtrkxqod.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgfzy.top/gtwqdmpcur.html

[R18] 遍历数组
来源：http://hz.shzxlz.cn/gtppvpispf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dianchejie.cn/gtwjgnvodi.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtjobhbrln.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtqkwsugox.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangkeji.top/gtvmjhpwft.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gtrwuvunjt.html

[R21] 字符串长度
来源：http://hz.fzhhl.top/gtdbgtqbsa.html

echo "${#s}"
来源：http://hz.mhx1999.top/gtqqieobqn.html

[R22] 截取子串
来源：http://hz.iojbl.cn/gtrbkvjgjq.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtuystpgrz.html

[R23] 字符串替换
来源：http://hz.jiagoushi.top/gtijuxxndu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ppjwa.cn/gtlvyvvtep.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtxwxvibdb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangtech.top/gtckfeezvp.html

[R25] 去后缀 / 去前缀
来源：http://hz.yonumen.top/gtdrbnaxzg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yvedp.cn/gtjyectamd.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtzljgtwbk.html

now=$(date +%F); echo "$now"
来源：http://hz.yonumen.top/gtsalxpfwj.html

[R27] 算术展开
来源：http://hz.daria6918.cn/gthxeoyewt.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258.top/gtheoravvz.html

[R28] 浮点运算
来源：http://hz.shangyingyoupin.top/gtrdifevcu.html

echo "scale=2; 10/3" | bc
来源：http://hz.sxryk.cn/gtcxfbxohe.html

[R29] 定义函数
来源：http://hz.guowangkeji.top/gtzlhrcifv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gtnbhyxfjf.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtatnjvcos.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.dashuyun.cn/gtzsprgxut.html

[R31] 局部变量
来源：http://hz.cashguo.top/gtxfwbiqky.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhiwuduotai.top/gthnjxbzyx.html

[R32] 参数个数校验
来源：http://hz.shzxlz.cn/gtsiuuxhsi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shuidangran.top/gteoszaksf.html

[R33] 捕获错误并提示行号
来源：http://hz.cqqwz.cn/gtbinljtdi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jiagoushi.top/gtidkgyxyk.html

[R34] 退出时清理
来源：http://hz.chenlongwang.top/gtvmbitccl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtsykybihz.html

[R35] 后台执行并等待
来源：http://hz.xingfuxueyuan.xyz/gtsaqsjoog.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tianlin.xyz/gtemazrkei.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangtech.top/gtwyvhxovj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhijiandao.cn/gtctxvrosn.html

[R37] 把输出赋给变量
来源：http://hz.316326.xyz/gtktwptpgm.html

files=$(ls -1)
来源：http://hz.tianlin.xyz/gtgnohcloq.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtdzqiwjiz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gthooewtyr.html

[R39] 重定向标准输出与错误
来源：http://hz.yuxming.cn/gtuodpevrt.html

cmd > out.log 2>&1
来源：http://hz.birdmap.top/gtnnupgxfl.html

[R40] 追加写日志
来源：http://hz.dashuyun.cn/gtguhopmxq.html

echo "log" >> out.log
来源：http://hz.shanyushiyangkeji.top/gtijygvtvi.html

[R41] 丢弃输出
来源：http://hz.xinyue.icu/gtwbwtxwbe.html

cmd >/dev/null 2>&1
来源：http://hz.daxiang520.top/gtjklwzwfz.html

[R42] 输入重定向
来源：http://hz.zhixingplan.top/gtjpdqlwcv.html

wc -l < a.txt
来源：http://hz.shangyingyoupin.top/gtvpactgsz.html

[R43] 按名字查找文件
来源：http://hz.dashuyun.cn/gtnwpvxcmk.html

find . -name "*.log" -type f
来源：http://hz.xylfe.cn/gtielpbcgf.html

[R44] 按修改时间查找
来源：http://hz.hysaishi.cn/gtabizsyvc.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtbkatbuwc.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtgjhjkazy.html

find . -name "*.tmp" -delete
来源：http://hz.yuanzhike.top/gtlwlxahsc.html

[R46] 递归替换文件内容
来源：http://hz.ybcxt.top/gtkxwidxxq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhaomingkeji.xyz/gtnfdprctj.html

[R47] sed 单行替换
来源：http://hz.ydjk.org.cn/gtokqodzja.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pycfn.com/gtppvibzqj.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gtnewnzoor.html

awk '{print $1, $3}' a.txt
来源：http://hz.sxryk.cn/gtbxweareh.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtzmupmwdo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sysykeji.top/gtxkzsrwdr.html

[R50] awk 求和
来源：http://hz.andypj.xyz/gtgnkswjrm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sufxvd.cn/gtdrqcwtwv.html

[R51] 排序去重取前几
来源：http://hz.svipenyu.cn/gtsiceuyht.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhixingplan.top/gtyinuirhy.html

[R52] 统计行数
来源：http://hz.redwolf501.top/gtzhoinxoz.html

wc -l a.txt
来源：http://hz.havefunace.top/gtnhauitrv.html

[R53] 查看文件头与实时尾
来源：http://hz.zhiwuduotai.top/gtrfahmjga.html


<!-- 参考信息 -->