代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtmzwfthut.html

user_id INT NOT NULL,
来源：http://hz.jiagoushi.top/gtmxoxlsaj.html

amount DECIMAL(10, 2),
来源：http://hz.xuetiantiany.cn/gtwnlubxku.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zdqjudy.top/gtqqhacyjn.html

);
来源：http://hz.chenjidiqi.icu/gteyvuapho.html

[Q03] 增加列
来源：http://hz.hnqzz.top/gtvxayizpq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aizwys.cn/gtlgluszzc.html

[Q04] 修改列类型
来源：http://hz.feifeiyinyue.top/gtkoyngheq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cqqwz.cn/gtgempvctk.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gthacjkipf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gtmdgqowwc.html

[Q06] 删除列
来源：http://hz.snrcjt.cn/gtuflrdkwp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgufenzy.top/gtuqotuybf.html

[Q07] 删除表
来源：http://hz.yangfankeji.com/gtnfwjuocw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinghuilouyu.cn/gtmokdjhah.html

[Q08] 创建普通索引
来源：http://hz.chenzaomai.com/gtlewrpuiq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gogol.net.cn/gtvzaowcbk.html

[Q09] 创建唯一索引
来源：http://hz.feifeiyinyue.top/gtjjgmwyfi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtlzqwdjgn.html

[Q10] 插入单行
来源：http://hz.ppjwa.cn/gtiltagjhq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.pengpengdd.cyou/gtngxiicir.html

[Q11] 一次插入多行
来源：http://hz.gogol.net.cn/gtjbmmclxa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenzaomai.com/gtycnwarup.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtnuwmqmuz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yvedp.cn/gtxklnqvqr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sysykeji.top/gtdznjuvxx.html

[Q13] 忽略重复插入
来源：http://hz.0kj1m.cn/gtojdltolk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhijiandao.cn/gtircfnlpj.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnqzz.top/gthjlbgsll.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zdqjudy.top/gthssckzay.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gtjbjtxkoh.html

[Q15] 查询全部
来源：http://hz.ppjwa.cn/gtmspyuuak.html

SELECT * FROM users;
来源：http://hz.hongshengwenyu.top/gtdxiuthyk.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtkmlzrmzz.html

SELECT id, name FROM users;
来源：http://hz.zhixingplan.top/gtijgmpmvb.html

[Q17] 条件查询
来源：http://hz.ppjwa.cn/gtdljsbawa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gaohongyu789.top/gtrcmqdant.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtpcryqitl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shuidangran.top/gtlwrzrkpd.html

[Q19] 范围查询
来源：http://hz.sxryk.cn/gttmdsufpd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnxiangtu.top/gtzldklrev.html

[Q20] IN 列表
来源：http://hz.ybcxt.top/gtxpvkoikp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigfzy.top/gtaaqekezu.html

[Q21] 空值判断
来源：http://hz.jqgfzy.top/gtlzapmksl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.52xcode.cn/gtqtewptqv.html

[Q22] 排序
来源：http://hz.xinyue.icu/gtgiroxyye.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gzhubu.top/gtnxwblvxc.html

[Q23] 分页
来源：http://hz.cdnleiting.top/gtuauruird.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yanxiufei.cn/gtgpdhoktf.html

[Q24] 去重
来源：http://hz.chenjidiqi.icu/gtxbzwvxug.html

SELECT DISTINCT city FROM users;
来源：http://hz.xylfe.cn/gtdiedwhzy.html

[Q25] 只取前 N 条
来源：http://hz.ehwqpu.com/gtozjzzccb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gtqxjpemnz.html

[Q26] 计数
来源：http://hz.cdnleiting.top/gtktdlqknf.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxuanxn.top/gteesafdit.html

[Q27] 条件计数
来源：http://hz.tian-w.cn/gthoshshtu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.0kj1m.cn/gtkoczognk.html

[Q28] 求和与平均
来源：http://hz.redwolf501.top/gtavdndpnf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnxiangtu.top/gtzgvmcqzo.html

[Q29] 最大最小值
来源：http://hz.andypj.xyz/gtgllwqlbb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.aibaodan.cn/gtbjvibpir.html

[Q30] 分组统计
来源：http://hz.xinyue.icu/gtedljvcsg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtzcvnjuoa.html

[Q31] 分组后过滤
来源：http://hz.jinqigfzy.top/gtswekqmra.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhijiandao.cn/gtecksmfmo.html

[Q32] 分组拼接字符串
来源：http://hz.hywenlv.cn/gtequvsqao.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.c1oappe.top/gtslsninex.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtxdovcdir.html

[Q33] 多列分组
来源：http://hz.hfpthk.cn/gtdhiwpdvi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.birdmap.top/gtnjrfxane.html

[Q34] 每组取第一条
来源：http://hz.dashuyun.cn/gtjsfmggkv.html

SELECT * FROM (
来源：http://hz.redwolf501.top/gtiwowwvxu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnxiangtu.top/gtqkktvnbx.html

) t WHERE rn = 1;
来源：http://hz.zhijiandao.cn/gtcjfhlikx.html

[Q35] 内连接
来源：http://hz.sxryk.cn/gtcqodybze.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtatpprhrh.html

[Q36] 左连接
来源：http://hz.jqgufenzy.top/gtrbgdsskd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ehwqpu.com/gtgseyvlrt.html

[Q37] 右连接
来源：http://hz.bjfxy.top/gtajghfogq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daxiang520.top/gtrkgfsptz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.bjfxy.top/gtndkmnywa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sysykeji.top/gtlsfweige.html

[Q39] 自连接（查上下级）
来源：http://hz.jqgfzy.top/gtejqiiopa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhongyouzk.top/gtjladxbom.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydjk.org.cn/gtugrxcyor.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtyjgropli.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhaomingkeji.xyz/gtpjgfhpah.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtbsbzpaho.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hongshengwenyu.top/gtbgytqxvk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.havefunace.top/gtyrcqxiwt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigfzy.top/gtovwvjein.html

[Q42] 连接条件附加过滤
来源：http://hz.pycfn.com/gtrcaeqjvz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhixingplan.top/gtwtvkdsct.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xinyue.icu/gtbttvzaph.html

[Q43] 标量子查询
来源：http://hz.jqgufenzy.top/gtauayhdkk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.mhx1999.top/gtzlrcwois.html

[Q44] IN 子查询
来源：http://hz.hywenlv.cn/gtqcezwtes.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.meibo888.top/gtfklhescz.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtwqibhiqw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.52xcode.cn/gtezintcik.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ywan-chungtsiang.top/gtovgyrrcr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtoinabncs.html

[Q47] 与平均值比较
来源：http://hz.snrcjt.cn/gttbblpuum.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dianchejie.cn/gtrvmquxix.html

[Q48] CTE 公用表表达式
来源：http://hz.zhoulong.xyz/gteyunjjei.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zycfv.cn/gtintrzhuw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ybcxt.top/gtxzvvtugm.html

[Q49] 更新单行
来源：http://hz.xuanzx.com/gtuzlhobwz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtacqhptul.html

[Q50] 批量更新
来源：http://hz.zycfv.cn/gtwnjjriut.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnxiangtu.top/gtsrngpgoy.html

[Q51] 用子查询更新
来源：http://hz.gotoacloud.top/gttgacwfdw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj20258888.top/gtakqvqyrw.html

[Q52] 删除指定行
来源：http://hz.ydzc1.top/gtrosowfbe.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gttkpojgtl.html

[Q53] 按条件删除
来源：http://hz.sxryk.cn/gtqgnlqgdh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ehwqpu.com/gtynrijena.html

[Q54] 清空表
来源：http://hz.vqdsnc.cn/gtosvwjvfy.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258.top/gtqyzdvklr.html

[Q55] 排名（并列占位）
来源：http://hz.xuetiantiany.cn/gtfkgdhzqn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.smart0.xyz/gtwshzfigk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtrhfuiyfl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtbzsygeqc.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gtucuvtuxu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yueranfly.top/gtwsxpkjlk.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtsdkklzxb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gtmjqwssaz.html

[Q59] 分组内累计
来源：http://hz.zhongyouzk.top/gtlstvjrwq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.9152youxi.cn/gtnrysfkjw.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtuyrcqqvo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.meibo888.top/gtafoyirsb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shangyingyoupin.top/gtfqlgkcbg.html

[Q61] 移动平均
来源：http://hz.yuanzhike.top/gtgpibonyx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtuwjyqmzf.html

[Q62] 分组占比
来源：http://hz.yj20258.top/gtnkbwebwu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtbsnillbz.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtmtnsnbnd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sweek.top/gtmkehvfzi.html

[Q64] 提交事务
来源：http://hz.9152youxi.cn/gtbzkvshcx.html

COMMIT;
来源：http://hz.aizwys.cn/gtpcyfhakt.html

[Q65] 回滚事务
来源：http://hz.ybcxt.top/gtoqfwmfkv.html

ROLLBACK;
来源：http://hz.birdmap.top/gtsxreseev.html

[Q66] 行锁查询
来源：http://hz.hammf.cn/gtnpoczryp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sxryk.cn/gtaujhvoar.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtljtnicdf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhoulong.xyz/gtiswxexwy.html

[Q68] 保存点
来源：http://hz.ybcxt.top/gtpbzorrfc.html

SAVEPOINT sp1;
来源：http://hz.jinghuilouyu.cn/gtimmwolep.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangtech.top/gtdslrqmts.html

[Q69] 查看执行计划
来源：http://hz.tian-w.cn/gtdbsyycmk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.kuanghao11.cn/gtzzwhebmy.html

[Q70] 更新统计信息
来源：http://hz.jinghuilouyu.cn/gtxggpnxqa.html

ANALYZE TABLE users;
来源：http://hz.aizwys.cn/gtefvhvvpu.html

[Q71] 查看建表语句
来源：http://hz.aizwys.cn/gtbthnocsl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nwbrower.top/gtjtwpbvjj.html

[Q72] 查看索引
来源：http://hz.yj20258888.top/gtkxznhoyn.html

SHOW INDEX FROM users;
来源：http://hz.zhongyouzk.top/gtirgddutc.html

[Q73] 查看表状态
来源：http://hz.birdmap.top/gtnfraxnmx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.bjfxy.top/gttftrwugi.html

[Q74] 强制使用索引
来源：http://hz.yuxming.cn/gtmjrajdtg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuetiantiany.cn/gtmnniymxa.html

[Q75] 日期格式化
来源：http://hz.yuanzhike.top/gtmoutkppv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtorepgpwm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtaobrwiea.html

[Q76] 按天统计
来源：http://hz.yangfankeji.com/gtbcmlysxv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xinyue.icu/gtyrwumgnq.html

[Q77] 时间加减
来源：http://hz.gogol.net.cn/gtxduksikm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xziqi.cn/gtjequzfxt.html

[Q78] 当前时间
来源：http://hz.jinqigufen.top/gteenranrl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenjidiqi.icu/gtgpsnlpby.html

[Q79] 字符串拼接
来源：http://hz.ehwqpu.com/gtqhbxcjtp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhongyouzk.top/gtdvlaxapb.html

[Q80] 字符串截取
来源：http://hz.mhx1999.top/gtuyghjkhu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nwbrower.top/gtsgicyeci.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtmndxrybf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhiwuduotai.top/gthcgdyrft.html

[Q82] 字符长度与字节长度
来源：http://hz.sufxvd.cn/gtaemgxlxt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.quarkkingdee.top/gtrmhbldbv.html

[Q83] 大小写转换
来源：http://hz.jqgufenzy.top/gtvkfwbgbf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigufen.top/gtuaihqgjc.html

[Q84] 去除首尾空格
来源：http://hz.daria6918.cn/gteatlrwzf.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtbsatatho.html

[Q85] 数值取整
来源：http://hz.jqgufenzy.top/gttoampaqj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ywan-chungtsiang.top/gtkcgmpnrl.html

[Q86] 读取 JSON 字段
来源：http://hz.andypj.xyz/gtozjxaojl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhengqikj.top/gtmebbclmj.html

[Q87] JSON 字段做条件
来源：http://hz.nwbrower.top/gtuwgwqzlu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daria6918.cn/gtwjmnmdqu.html

[Q88] 行转列（条件聚合）
来源：http://hz.haohaochexian.top/gtugbfupav.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yongpay.top/gttsiqqhdo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtbozgtjpz.html

[Q89] 判断表是否存在
来源：http://hz.sxryk.cn/gtvmofgkcg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnxiangtu.top/gtrjrfequc.html

[Q90] 生成序号列
来源：http://hz.yuxming.cn/gtzaoxlhci.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.9152youxi.cn/gtmfcisdtj.html

================================================================================
来源：http://hz.9152youxi.cn/gtgaghcgba.html

R. Bash 专题
来源：http://hz.guannengcc.top/gtbymqilxw.html

================================================================================
来源：http://hz.cdnleiting.top/gtzpibpmzb.html

[R01] shebang 与严格模式
来源：http://hz.zhijiandao.cn/gtvaypfacu.html

#!/usr/bin/env bash
来源：http://hz.yanxiufei.cn/gtupyhvpju.html

set -euo pipefail
来源：http://hz.zhaomingkeji.xyz/gtmbgjgfna.html

[R02] 变量赋值与使用
来源：http://hz.zycfv.cn/gtafiklfgb.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtsxnbcikh.html

[R03] 只读变量
来源：http://hz.yj202588.top/gtveoavcqz.html

readonly PI=3.14
来源：http://hz.birdmap.top/gtofbzqgxt.html

[R04] 位置参数
来源：http://hz.yj20258.top/gtzeonquhn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sysykeji.top/gtmphwxapy.html

[R05] 参数默认值
来源：http://hz.zycfv.cn/gtpabkqkov.html

name="${1:-default}"
来源：http://hz.gaohongyu789.top/gtgrhltfko.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtvubczgok.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtngtxpndb.html

[R07] if 判断文件
来源：http://hz.aibaodan.cn/gtfoykqzwb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fengsongda.top/gtrvkwbwbi.html

[R08] 数值比较
来源：http://hz.ivvv.top/gtsqsynqem.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj20258.top/gtgcnaummm.html

[R09] 字符串比较
来源：http://hz.gotoacloud.top/gtulmhgchq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hongshengwenyu.top/gtlonzijfk.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtglgcupcg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yanxiufei.cn/gtjwfrlnva.html

[R11] case 多分支
来源：http://hz.tian-w.cn/gtckvdxwua.html

case "$1" in
来源：http://hz.jqgfzy.top/gtjhofpadq.html

start) echo "启动" ;;
来源：http://hz.zhixingplan.top/gtmbzvcxyp.html

stop)  echo "停止" ;;
来源：http://hz.zdqjudy.top/gtfxbdazkj.html

*)     echo "未知命令" ;;
来源：http://hz.9152youxi.cn/gtkqvqfbqp.html

esac
来源：http://hz.pycfn.com/gthdpjmcmj.html

[R12] for 遍历文件
来源：http://hz.zhaomingkeji.xyz/gtxkbzlcbu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigfzy.top/gtkpulaphk.html

[R13] for 计数循环
来源：http://hz.fzhhl.top/gtdynzfwmx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtwdltflmp.html

[R14] C 风格 for
来源：http://hz.jinqigfzy.top/gtuxlwswxi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gtxezmloqr.html

[R15] while 逐行读文件
来源：http://hz.fzhhl.top/gtruiavbye.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shuidangran.top/gteqystbok.html

[R16] until 等待条件
来源：http://hz.jyoumei.cn/gttvdwbfiw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gogol.net.cn/gttcxoxahr.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangtech.top/gtcjjcbghe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yueranfly.top/gtujiqdtbi.html

[R18] 遍历数组
来源：http://hz.316326.xyz/gtrtsbeyby.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.birdmap.top/gtpxdooqty.html

[R19] 数组长度
来源：http://hz.tian-w.cn/gtzaopayen.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtdzyzpppm.html

[R20] 关联数组（字典）
来源：http://hz.gotoacloud.top/gtxxxvwedz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhaomingkeji.xyz/gttohdnecd.html

[R21] 字符串长度
来源：http://hz.yj20258888.top/gtwszulvaa.html

echo "${#s}"
来源：http://hz.ydzc1.top/gtjcmtactd.html

[R22] 截取子串
来源：http://hz.birdmap.top/gtjcleihhe.html

echo "${s:0:5}"
来源：http://hz.daria6918.cn/gttlomenir.html

[R23] 字符串替换
来源：http://hz.fzhhl.top/gtffggwchk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yangfankeji.com/gtjlcludxu.html

[R24] 大小写转换
来源：http://hz.jyoumei.cn/gtwzhbddhc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zycfv.cn/gturtusgut.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangkeji.top/gtkquhgomb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zdqjudy.top/gtmbkssnvp.html

[R26] 命令替换
来源：http://hz.daria6918.cn/gtrtzdtest.html

now=$(date +%F); echo "$now"
来源：http://hz.yongpay.top/gtpugnuuqd.html

[R27] 算术展开
来源：http://hz.fzhhl.top/gtxgdmlewr.html

echo $((1 + 2 * 3))
来源：http://hz.xingfuxueyuan.xyz/gtnspzaqpz.html

[R28] 浮点运算
来源：http://hz.jiagoushi.top/gtxjuecmyc.html

echo "scale=2; 10/3" | bc
来源：http://hz.sysykeji.top/gtwblzgkqx.html

[R29] 定义函数
来源：http://hz.svipenyu.cn/gtxzlwjesy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yvedp.cn/gtccgiygfv.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtcmobeqwj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnxiangtu.top/gtjgpsfbmt.html

[R31] 局部变量
来源：http://hz.nanxuanxn.top/gteuildzzd.html

f() { local x=1; echo "$x"; }
来源：http://hz.sufxvd.cn/gttvvayizc.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtttrsqfrr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yvedp.cn/gtkvycgtei.html

[R33] 捕获错误并提示行号
来源：http://hz.nanxuanxn.top/gtgwhtsyzt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtdzhftqrs.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gthdhhfstm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtyzzirbkm.html

[R35] 后台执行并等待
来源：http://hz.vqdsnc.cn/gtbvrmwoii.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.andypj.xyz/gtdzehruvq.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtyirgvjfr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtieiktxsa.html

[R37] 把输出赋给变量
来源：http://hz.yonumen.top/gtcvpgnjcd.html

files=$(ls -1)
来源：http://hz.guowangkeji.top/gtgvptmlkp.html

[R38] 管道串联
来源：http://hz.meibo888.top/gtqehdnjse.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtdythtsom.html

[R39] 重定向标准输出与错误
来源：http://hz.shangyingyoupin.top/gtksampdlb.html

cmd > out.log 2>&1
来源：http://hz.guowangkeji.top/gtrchsbnlf.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtxcdaprtn.html

echo "log" >> out.log
来源：http://hz.smart0.xyz/gtiptblkzr.html

[R41] 丢弃输出
来源：http://hz.chenzaomai.com/gtjwtrbxoh.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gthvtwvpun.html

[R42] 输入重定向
来源：http://hz.redwolf501.top/gtoestpbvd.html

wc -l < a.txt
来源：http://hz.zycfv.cn/gtwwqacmhi.html

[R43] 按名字查找文件
来源：http://hz.nanxuanxn.top/gtthknxkdl.html

find . -name "*.log" -type f
来源：http://hz.jinqigufen.top/gtkdgectdn.html

[R44] 按修改时间查找
来源：http://hz.ivvv.top/gtgkrmgexy.html

find . -mtime -7 -type f
来源：http://hz.jqgufenzy.top/gtuladhtcf.html

[R45] 批量删除
来源：http://hz.guowangkeji.top/gtftygrxug.html

find . -name "*.tmp" -delete
来源：http://hz.haohaochexian.top/gtpmxqbtwp.html

[R46] 递归替换文件内容
来源：http://hz.jiagoushi.top/gtdkoelzhn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.dianchejie.cn/gtmzsjijeh.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtgfkexgfw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daxiang520.top/gtxhvyyjac.html

[R48] awk 取指定列
来源：http://hz.wangdashe.top/gtyzdiqlji.html

awk '{print $1, $3}' a.txt
来源：http://hz.kuanghao11.cn/gtbxkkscpc.html

[R49] awk 带条件
来源：http://hz.jinyuanbaomall.cn/gtivcikfrp.html


<!-- 参考信息 -->