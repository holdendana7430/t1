代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtcnzskzja.html

user_id INT NOT NULL,
来源：http://hz.jianghu66.top/gtrlbenffv.html

amount DECIMAL(10, 2),
来源：http://hz.nanxuanxn.top/gtoouhisxo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangtech.top/gtsxmqsxtc.html

);
来源：http://hz.jlsjyb.cn/gtwuzgxrrf.html

[Q03] 增加列
来源：http://hz.zhixingplan.top/gtaybfwjjh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nanxuanxn.top/gtnalefzxu.html

[Q04] 修改列类型
来源：http://hz.yvedp.cn/gtixnpdigk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hammf.cn/gtagowneuu.html

[Q05] 重命名列
来源：http://hz.cashguo.top/gtolyxyufu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dianchejie.cn/gtsdabjqcx.html

[Q06] 删除列
来源：http://hz.yj20258.top/gtqucschoz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.smart0.xyz/gtrxzgkpqd.html

[Q07] 删除表
来源：http://hz.chenlongwang.top/gttciahpsm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jlsjyb.cn/gtmwlvewls.html

[Q08] 创建普通索引
来源：http://hz.ydzc1.top/gtqpvyptxv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydzc1.top/gternuadwo.html

[Q09] 创建唯一索引
来源：http://hz.nanxuanxn.top/gtmxndecwy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhiwuduotai.top/gtrohphmke.html

[Q10] 插入单行
来源：http://hz.cucudq.cn/gtmsymrokq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangdashe.top/gthihyoppu.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gtosnujefr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shangyingyoupin.top/gtglvvmlxh.html

[Q12] 插入后取自增 ID
来源：http://hz.jinqigfzy.top/gtcdltebaw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258.top/gtnpytupjr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ppjwa.cn/gtnxmsednm.html

[Q13] 忽略重复插入
来源：http://hz.yj202588.top/gtenxiehov.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ivvv.top/gtqhzcthhc.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenjidiqi.icu/gtkmsmjowz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhoulong.xyz/gtptyugjgs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.svipenyu.cn/gtzyuyogeb.html

[Q15] 查询全部
来源：http://hz.sweek.top/gturtskqhb.html

SELECT * FROM users;
来源：http://hz.9152youxi.cn/gtjbtzjhvg.html

[Q16] 查询指定列
来源：http://hz.jinyuanbaomall.cn/gtpjlwdkss.html

SELECT id, name FROM users;
来源：http://hz.feifeiyinyue.top/gtcoylvlig.html

[Q17] 条件查询
来源：http://hz.yuxming.cn/gtjjqxvsio.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.kuanghao11.cn/gtgksrqjdz.html

[Q18] 模糊匹配
来源：http://hz.ydzc1.top/gtcyvjeavv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nwbrower.top/gtwobbxwws.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gtjtfqvafq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gtujuesxac.html

[Q20] IN 列表
来源：http://hz.svipenyu.cn/gtfyjjdvng.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.c1oappe.top/gtwobdusts.html

[Q21] 空值判断
来源：http://hz.zhixingplan.top/gtlcvklils.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.meibo888.top/gtomqtehsv.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtdgiunfuq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hongshengwenyu.top/gtgcvttahm.html

[Q23] 分页
来源：http://hz.svipenyu.cn/gtkxigqhav.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtkctliqjy.html

[Q24] 去重
来源：http://hz.hywenlv.cn/gtzlbpzeve.html

SELECT DISTINCT city FROM users;
来源：http://hz.gotoacloud.top/gtumdxcvsz.html

[Q25] 只取前 N 条
来源：http://hz.nwbrower.top/gtggwmrgst.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ivvv.top/gthcqvgnko.html

[Q26] 计数
来源：http://hz.shanyushiyangkeji.top/gtppvnymio.html

SELECT COUNT(*) FROM users;
来源：http://hz.meibo888.top/gtbnvnzodj.html

[Q27] 条件计数
来源：http://hz.cdnleiting.top/gtewhpzgyf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtpejkepre.html

[Q28] 求和与平均
来源：http://hz.gzhubu.top/gtfwepnynw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ydjk.org.cn/gtabrkhknr.html

[Q29] 最大最小值
来源：http://hz.xingfuxueyuan.xyz/gtlvqehglo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtkxelxqjf.html

[Q30] 分组统计
来源：http://hz.daria6918.cn/gtzhucyief.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtaceqtgam.html

[Q31] 分组后过滤
来源：http://hz.meibo888.top/gtnbopcvua.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gtmdgqbejh.html

[Q32] 分组拼接字符串
来源：http://hz.shangyingyoupin.top/gtblhtfbce.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtqjlxafyz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtociptnri.html

[Q33] 多列分组
来源：http://hz.tian-w.cn/gtfyxkvael.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gogol.net.cn/gtjebstxwq.html

[Q34] 每组取第一条
来源：http://hz.tian-w.cn/gtxszceorb.html

SELECT * FROM (
来源：http://hz.zycfv.cn/gtjuawlgov.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fengsongda.top/gtzcbamcni.html

) t WHERE rn = 1;
来源：http://hz.sxryk.cn/gtgxhqlrzb.html

[Q35] 内连接
来源：http://hz.ybcxt.top/gtmnrxltex.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtlswdkijm.html

[Q36] 左连接
来源：http://hz.jqgfzy.top/gtrtxenape.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtrrvhkmju.html

[Q37] 右连接
来源：http://hz.jyoumei.cn/gtaxwpiyjk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.andypj.xyz/gtwgzkgiwq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gtmifmoqtk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuanzx.com/gtzarbuztb.html

[Q39] 自连接（查上下级）
来源：http://hz.zhaomingkeji.xyz/gtsfbksana.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yvedp.cn/gtfyebekyx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangdashe.top/gtkmcxwaqj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sxryk.cn/gtqestefeo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.bjfxy.top/gteslwzzcf.html

[Q41] 多表连接
来源：http://hz.gogol.net.cn/gtnloxvhuw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yongpay.top/gtbsqiclao.html

JOIN users u ON u.id = o.user_id
来源：http://hz.c1oappe.top/gtmmhhxhuk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhoulong.xyz/gtwxdylfgl.html

[Q42] 连接条件附加过滤
来源：http://hz.shzxlz.cn/gtzxbgjrap.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydzc1.top/gteinixngb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.316326.xyz/gtgdxufmea.html

[Q43] 标量子查询
来源：http://hz.xingfuxueyuan.xyz/gtxkuvqwoa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhaomingkeji.xyz/gtenytpjpe.html

[Q44] IN 子查询
来源：http://hz.zhixingplan.top/gtuouwgcln.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hnqzz.top/gtdbikwpwc.html

[Q45] EXISTS 判断存在
来源：http://hz.jiagoushi.top/gtgshmcddl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtdgpusrxt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangshuangyany.cn/gtmhhxperf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtwkgllsav.html

[Q47] 与平均值比较
来源：http://hz.yanxiufei.cn/gtqijidspr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigufen.top/gtwjekopvd.html

[Q48] CTE 公用表表达式
来源：http://hz.cashguo.top/gthtzyumyb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.vqdsnc.cn/gttszqwspg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhengqikj.top/gthpvvfmsa.html

[Q49] 更新单行
来源：http://hz.fengsongda.top/gtvcuvytor.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtkerqomzl.html

[Q50] 批量更新
来源：http://hz.zycfv.cn/gtfwiavhvq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cheryme.top/gtzkypyats.html

[Q51] 用子查询更新
来源：http://hz.jinghuilouyu.cn/gtzrjxpepc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gtfhedmwbb.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtklrrzsas.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtkoeuwjbw.html

[Q53] 按条件删除
来源：http://hz.nwbrower.top/gtgpumrhsb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtuyblgtjd.html

[Q54] 清空表
来源：http://hz.cheryme.top/gtrqtpxxns.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gtjdbrlaer.html

[Q55] 排名（并列占位）
来源：http://hz.meibo888.top/gtcpjihulu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj202588.top/gtnvpvrklf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangtech.top/gtyrlrshrx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tian-w.cn/gtiruwszpq.html

[Q57] 行号
来源：http://hz.daria6918.cn/gtzutonsbj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.feifeiyinyue.top/gtufrduoxm.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtgskgkbtq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xinyue.icu/gtqjaglhhv.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gtfueobvuc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.birdmap.top/gtbpjjoomm.html

[Q60] 取上一行 / 下一行
来源：http://hz.hysaishi.cn/gtsfgarayb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pycfn.com/gthtsfrqpz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sufxvd.cn/gtmcuzjuyn.html

[Q61] 移动平均
来源：http://hz.hongshengwenyu.top/gtgdvhdbyh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhengqikj.top/gtmvetnxnr.html

[Q62] 分组占比
来源：http://hz.0kj1m.cn/gtihfarvbv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtfnmqzgcp.html

[Q63] 开启事务
来源：http://hz.xuetiantiany.cn/gtbjfzroco.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jiagoushi.top/gtdxhgiqhn.html

[Q64] 提交事务
来源：http://hz.yongpay.top/gtejpiwjay.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gtssgejeix.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtbtqzvssw.html

ROLLBACK;
来源：http://hz.52xcode.cn/gtocyimhzw.html

[Q66] 行锁查询
来源：http://hz.xuanzx.com/gthkcccbko.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gttmzopolq.html

[Q67] 设置隔离级别
来源：http://hz.ywan-chungtsiang.top/gtqnnycblb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.316326.xyz/gtckwzjsff.html

[Q68] 保存点
来源：http://hz.nanxinkj.top/gtrfudelit.html

SAVEPOINT sp1;
来源：http://hz.ywan-chungtsiang.top/gtzyhycpla.html

ROLLBACK TO sp1;
来源：http://hz.yj20258888.top/gttmgfhkld.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtcrojkrqk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daria6918.cn/gtjuacppif.html

[Q70] 更新统计信息
来源：http://hz.tian-w.cn/gtcryoflgf.html

ANALYZE TABLE users;
来源：http://hz.meibo888.top/gttrdkgaqt.html

[Q71] 查看建表语句
来源：http://hz.hongshengwenyu.top/gtrqinynbf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ppjwa.cn/gtgnildwch.html

[Q72] 查看索引
来源：http://hz.xinyue.icu/gtqerukcdo.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtpovrwtzf.html

[Q73] 查看表状态
来源：http://hz.dianchejie.cn/gtqbxdbrlw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jiagoushi.top/gtyipurtxs.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtxquhtwlw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtlmyjxegq.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gtsmcwswsw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yueranfly.top/gtmvkkrvnz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.iojbl.cn/gtyxofjfje.html

[Q76] 按天统计
来源：http://hz.yj20258.top/gtxmqrnegj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jianghu66.top/gtdyqoufmy.html

[Q77] 时间加减
来源：http://hz.havefunace.top/gtegzqyjgr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydjk.org.cn/gtuoysmppj.html

[Q78] 当前时间
来源：http://hz.xziqi.cn/gtykysdncr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangdashe.top/gtzasowswg.html

[Q79] 字符串拼接
来源：http://hz.smart0.xyz/gtnlhjjmqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gtrmhagrta.html

[Q80] 字符串截取
来源：http://hz.hnqzz.top/gtkbcirstx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhongyouzk.top/gtyirwqjoa.html

[Q81] 字符串替换
来源：http://hz.jinqigufen.top/gtsohuzzhe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj202588.top/gtgacflbdb.html

[Q82] 字符长度与字节长度
来源：http://hz.snrcjt.cn/gtetdyivbp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtpqslbwtu.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtowdwcmzl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yonumen.top/gtwwihwuju.html

[Q84] 去除首尾空格
来源：http://hz.sxryk.cn/gtgemnzigg.html

SELECT TRIM(name) FROM users;
来源：http://hz.ppjwa.cn/gtaticpvsm.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gtxxeqoatx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xylfe.cn/gtneukunzo.html

[Q86] 读取 JSON 字段
来源：http://hz.birdmap.top/gtwggampds.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinyuanbaomall.cn/gtnweexpuk.html

[Q87] JSON 字段做条件
来源：http://hz.zhiwuduotai.top/gtksmdgipw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ywan-chungtsiang.top/gtyllwvehl.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtflgkgqqj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydzc1.top/gtdslpyiyp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtsmzedzwt.html

[Q89] 判断表是否存在
来源：http://hz.wangdashe.top/gttfpwdeto.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhixingplan.top/gtwmhnzmkn.html

[Q90] 生成序号列
来源：http://hz.hywenlv.cn/gtjjlrgznk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258.top/gttysmilsh.html

================================================================================
来源：http://hz.zycfv.cn/gtpzqcyute.html

R. Bash 专题
来源：http://hz.havefunace.top/gtgpnnznto.html

================================================================================
来源：http://hz.gzhubu.top/gtglsetgch.html

[R01] shebang 与严格模式
来源：http://hz.ydzc1.top/gtzhzynuai.html

#!/usr/bin/env bash
来源：http://hz.zhaomingkeji.xyz/gtujtunzqu.html

set -euo pipefail
来源：http://hz.guannengcc.top/gtxldddsrk.html

[R02] 变量赋值与使用
来源：http://hz.316326.xyz/gthljhmngx.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtokziwpmz.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtpmrbenar.html

readonly PI=3.14
来源：http://hz.ydjk.org.cn/gtzyxwpzar.html

[R04] 位置参数
来源：http://hz.jianghu66.top/gtwmcvhdzs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenlongwang.top/gtojennvxt.html

[R05] 参数默认值
来源：http://hz.quarkkingdee.top/gtmcftftwu.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtomznlrey.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtszcxgbxj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.iojbl.cn/gtsuprlakr.html

[R07] if 判断文件
来源：http://hz.52xcode.cn/gtewqtffuw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cheryme.top/gtkzriwyta.html

[R08] 数值比较
来源：http://hz.havefunace.top/gtvelvjeeb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shuidangran.top/gtkccsxrwc.html

[R09] 字符串比较
来源：http://hz.sufxvd.cn/gtssyanqoo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hysaishi.cn/gttubxmvyg.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtzeqiisqt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pengpengdd.cyou/gtyxbgmemg.html

[R11] case 多分支
来源：http://hz.shzxlz.cn/gtczrcuhfj.html

case "$1" in
来源：http://hz.yuanzhike.top/gtbuwmczhr.html

start) echo "启动" ;;
来源：http://hz.tanke756.top/gttijfmkhs.html

stop)  echo "停止" ;;
来源：http://hz.pengpengdd.cyou/gtvoizfmym.html

*)     echo "未知命令" ;;
来源：http://hz.gogol.net.cn/gtgqszhkms.html

esac
来源：http://hz.0kj1m.cn/gthnuisaxy.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtddpscwcc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hysaishi.cn/gtliuhxgwd.html

[R13] for 计数循环
来源：http://hz.fengsongda.top/gtsvyachqx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dianchejie.cn/gtjvsbmctl.html

[R14] C 风格 for
来源：http://hz.shanyushiyangtech.top/gtvgtwpjfx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cheryme.top/gtwwnqyemj.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtryfqcrrr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuanzx.com/gtzmwcfxns.html

[R16] until 等待条件
来源：http://hz.xuanzx.com/gtxffsojwi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cashguo.top/gtvqykozdi.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtgwmyvpnq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.kuanghao11.cn/gtzwtwciwm.html

[R18] 遍历数组
来源：http://hz.jqgufenzy.top/gtmmqffvep.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gogol.net.cn/gtmkhggbrr.html

[R19] 数组长度
来源：http://hz.sweek.top/gtnqfjbdtd.html

echo "${#arr[@]}"
来源：http://hz.aizwys.cn/gtntzjijcj.html

[R20] 关联数组（字典）
来源：http://hz.tian-w.cn/gtrgfhwaxa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.chenzaomai.com/gtsnrlcykj.html

[R21] 字符串长度
来源：http://hz.xuanzx.com/gtweuusntu.html

echo "${#s}"
来源：http://hz.yongpay.top/gtdowadipu.html

[R22] 截取子串
来源：http://hz.sweek.top/gtlnyumosh.html

echo "${s:0:5}"
来源：http://hz.sxryk.cn/gtimuelwec.html

[R23] 字符串替换
来源：http://hz.zhijiandao.cn/gthugjflaf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fzhhl.top/gtbrrlambg.html

[R24] 大小写转换
来源：http://hz.redwolf501.top/gtbejzkcsn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tianlin.xyz/gtmszyxfja.html

[R25] 去后缀 / 去前缀
来源：http://hz.vqdsnc.cn/gtfgowyqqo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pycfn.com/gtsqiiozfn.html

[R26] 命令替换
来源：http://hz.jqgufenzy.top/gtmwhyyrlg.html

now=$(date +%F); echo "$now"
来源：http://hz.shzxlz.cn/gthmyvuxgf.html

[R27] 算术展开
来源：http://hz.nanxuanxn.top/gtezpdsonp.html

echo $((1 + 2 * 3))
来源：http://hz.shzxlz.cn/gtrmbofnun.html

[R28] 浮点运算
来源：http://hz.yvedp.cn/gteykszwyw.html

echo "scale=2; 10/3" | bc
来源：http://hz.cashguo.top/gtznwypbdc.html

[R29] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtpvgulydb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj202588.top/gtpxlgrhqy.html

[R30] 函数返回状态码
来源：http://hz.gogol.net.cn/gtvaakidcr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenlongwang.top/gtlbdeobly.html

[R31] 局部变量
来源：http://hz.yuxming.cn/gtcczemtbu.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnqzz.top/gtpbtdiqar.html

[R32] 参数个数校验
来源：http://hz.feifeiyinyue.top/gtivyfgpdn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj202588.top/gtisdupdwp.html

[R33] 捕获错误并提示行号
来源：http://hz.sweek.top/gtziyxmtkp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gogol.net.cn/gtpbwiyszk.html

[R34] 退出时清理
来源：http://hz.zhoulong.xyz/gtxikthkcy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtdodoinzm.html

[R35] 后台执行并等待
来源：http://hz.tianlin.xyz/gttmptgaqy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jlsjyb.cn/gteokrptpr.html

[R36] 并发执行多个任务
来源：http://hz.havefunace.top/gtwkpmgehi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guannengcc.top/gtqcxfcyqw.html

[R37] 把输出赋给变量
来源：http://hz.wangshuangyany.cn/gtrsnovbht.html

files=$(ls -1)
来源：http://hz.wangdashe.top/gteglocrwv.html

[R38] 管道串联
来源：http://hz.aizwys.cn/gtetunimcu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gtueusvatb.html

[R39] 重定向标准输出与错误
来源：http://hz.meibo888.top/gtrpjooxki.html

cmd > out.log 2>&1
来源：http://hz.cdnleiting.top/gtziksrgwn.html

[R40] 追加写日志
来源：http://hz.hnqzz.top/gtlfapjvoo.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gtybwfwluc.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gtofvzaexd.html

cmd >/dev/null 2>&1
来源：http://hz.iojbl.cn/gtfdhezvjf.html

[R42] 输入重定向
来源：http://hz.guannengcc.top/gtvyvfycfh.html

wc -l < a.txt
来源：http://hz.ydjk.org.cn/gtikvtwvqk.html

[R43] 按名字查找文件
来源：http://hz.havefunace.top/gtfbfqmahw.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtkrkyybbh.html

[R44] 按修改时间查找
来源：http://hz.tianlin.xyz/gtcysjnmhq.html

find . -mtime -7 -type f
来源：http://hz.jinghuilouyu.cn/gtqverfryk.html

[R45] 批量删除
来源：http://hz.fengsongda.top/gtfxwdyvqu.html

find . -name "*.tmp" -delete
来源：http://hz.andypj.xyz/gtnkgclmjn.html

[R46] 递归替换文件内容
来源：http://hz.nanxinkj.top/gthppcmnfb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtututdwoi.html

[R47] sed 单行替换
来源：http://hz.shangyingyoupin.top/gtgbwevmhc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jiagoushi.top/gtkbokctav.html

[R48] awk 取指定列
来源：http://hz.sysykeji.top/gtjogddajb.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuxming.cn/gtmflzzkfq.html

[R49] awk 带条件
来源：http://hz.xingfuxueyuan.xyz/gtboniylkx.html


<!-- 参考信息 -->