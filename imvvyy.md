代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gthzzdtlux.html

);
来源：http://hz.gaohongyu789.top/gtgpxjlgjv.html

[Q02] 创建带外键的表
来源：http://hz.pengpengdd.cyou/gtqqgjkxvf.html

CREATE TABLE orders (
来源：http://hz.shuidangran.top/gttzotwfwg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtqkwkhteh.html

user_id INT NOT NULL,
来源：http://hz.guannengcc.top/gtvfmgvbtd.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtitmxcrob.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cdnleiting.top/gtvvhojrcy.html

);
来源：http://hz.havefunace.top/gtcpayvgtu.html

[Q03] 增加列
来源：http://hz.birdmap.top/gtgycboggc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtmsbliflt.html

[Q04] 修改列类型
来源：http://hz.yueranfly.top/gtcmkkvuvm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zdqjudy.top/gtetqzgdhx.html

[Q05] 重命名列
来源：http://hz.zhixingplan.top/gtptlfhjdl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dianchejie.cn/gtenhumbkn.html

[Q06] 删除列
来源：http://hz.dashuyun.cn/gtkmogobnt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ivvv.top/gtmyyeecmf.html

[Q07] 删除表
来源：http://hz.52xcode.cn/gtlmpmgsaj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xingfuxueyuan.xyz/gtdqfdjapr.html

[Q08] 创建普通索引
来源：http://hz.cdnleiting.top/gtyckilujp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxinkj.top/gttuhwxcou.html

[Q09] 创建唯一索引
来源：http://hz.guannengcc.top/gtvfxizhom.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.c1oappe.top/gtvztwmqlb.html

[Q10] 插入单行
来源：http://hz.hysaishi.cn/gtbgozslmg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gotoacloud.top/gtmvlzgkhy.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gttimuofcp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ywan-chungtsiang.top/gtduegvpea.html

[Q12] 插入后取自增 ID
来源：http://hz.daria6918.cn/gtynquetes.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gzhubu.top/gtsartrrhl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtdtjmwyoe.html

[Q13] 忽略重复插入
来源：http://hz.zhijiandao.cn/gtsteisycu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ppjwa.cn/gtonwprqxs.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gtcsyumnpt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnqzz.top/gtzsplixdw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aizwys.cn/gtggnkvimk.html

[Q15] 查询全部
来源：http://hz.xingfuxueyuan.xyz/gtvknhvcit.html

SELECT * FROM users;
来源：http://hz.shanyushiyangtech.top/gtdbolzukb.html

[Q16] 查询指定列
来源：http://hz.yueranfly.top/gtsnvbhhmj.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gtbsgsfsik.html

[Q17] 条件查询
来源：http://hz.shzxlz.cn/gtaqyfukeh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.0kj1m.cn/gtmpgrxyxw.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gtwiknadib.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dashuyun.cn/gtxntvczxr.html

[Q19] 范围查询
来源：http://hz.gaohongyu789.top/gtdydugebl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.316326.xyz/gtymycwtid.html

[Q20] IN 列表
来源：http://hz.aizwys.cn/gteonfmmde.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.svipenyu.cn/gtfcqgizja.html

[Q21] 空值判断
来源：http://hz.zhoulong.xyz/gthbahytyk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.316326.xyz/gtqeqyxksh.html

[Q22] 排序
来源：http://hz.andypj.xyz/gtvwbjgbgp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yangfankeji.com/gtlmfmmjkc.html

[Q23] 分页
来源：http://hz.ivvv.top/gtjorlusmu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zycfv.cn/gtiqcxnnsc.html

[Q24] 去重
来源：http://hz.cashguo.top/gtlfekdxlw.html

SELECT DISTINCT city FROM users;
来源：http://hz.guannengcc.top/gtdisztkxo.html

[Q25] 只取前 N 条
来源：http://hz.xinyue.icu/gtavrzvxca.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yangfankeji.com/gtwewnkrov.html

[Q26] 计数
来源：http://hz.daxiang520.top/gtwbcytefd.html

SELECT COUNT(*) FROM users;
来源：http://hz.cqqwz.cn/gtvbnopvet.html

[Q27] 条件计数
来源：http://hz.xinyue.icu/gtbrbcblfs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuanzhike.top/gtkiwwrvgy.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtundwppfl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtkrnrpfoc.html

[Q29] 最大最小值
来源：http://hz.jyoumei.cn/gtoegzmjvk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sufxvd.cn/gthxgmrskg.html

[Q30] 分组统计
来源：http://hz.gotoacloud.top/gtaksecony.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtdhoxnvin.html

[Q31] 分组后过滤
来源：http://hz.xuanzx.com/gtjaxkvbdv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shzxlz.cn/gtlnjmyikr.html

[Q32] 分组拼接字符串
来源：http://hz.sysykeji.top/gtssvkbvaz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtviuuvdgz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtjzysbgoy.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtcqiwjdfh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yongpay.top/gtebqaodxv.html

[Q34] 每组取第一条
来源：http://hz.xylfe.cn/gtyhcgplbj.html

SELECT * FROM (
来源：http://hz.yuanzhike.top/gtzlsavnls.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ppjwa.cn/gthzbsxhgo.html

) t WHERE rn = 1;
来源：http://hz.316326.xyz/gtmerbefaw.html

[Q35] 内连接
来源：http://hz.cdnleiting.top/gtctorxakl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtewtexqxp.html

[Q36] 左连接
来源：http://hz.zycfv.cn/gtjvccvszk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cashguo.top/gtecyoxnbi.html

[Q37] 右连接
来源：http://hz.cheryme.top/gtqnfbedds.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.birdmap.top/gtahafzmfo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhengqikj.top/gtwdjqnqxl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shuidangran.top/gtbbdvvdge.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gtfsqwmteu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.redwolf501.top/gtmrcobrjv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jlsjyb.cn/gttzkkqlqm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtcwhwqojv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigufen.top/gtawcmaqgu.html

[Q41] 多表连接
来源：http://hz.jqgufenzy.top/gtdieibnwb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnqzz.top/gtcxhtuvrp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnqzz.top/gtottqnxqo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.quarkkingdee.top/gtjklsusuh.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258888.top/gthwkfcchd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.bjfxy.top/gtgffaavjk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aibaodan.cn/gtqeiwhggn.html

[Q43] 标量子查询
来源：http://hz.pycfn.com/gthallvuhe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yongpay.top/gtxbpzgiwd.html

[Q44] IN 子查询
来源：http://hz.sweek.top/gtgpfbrzjk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ppjwa.cn/gtebjqwjwl.html

[Q45] EXISTS 判断存在
来源：http://hz.xuetiantiany.cn/gtdndrgydi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gthwiwtbzx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.9152youxi.cn/gtdcjhsnwa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtklirsgvr.html

[Q47] 与平均值比较
来源：http://hz.haohaochexian.top/gtvcbrmbty.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aibaodan.cn/gthajwhvan.html

[Q48] CTE 公用表表达式
来源：http://hz.gzhubu.top/gttruibbkt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hywenlv.cn/gtpaznossb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jlsjyb.cn/gtryqgpzxk.html

[Q49] 更新单行
来源：http://hz.sweek.top/gtweawbtmn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtiqbltlkv.html

[Q50] 批量更新
来源：http://hz.andypj.xyz/gtwpyvhdts.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hfpthk.cn/gtufjctsbe.html

[Q51] 用子查询更新
来源：http://hz.dianchejie.cn/gtslenpeku.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.daria6918.cn/gtxkysuqyk.html

[Q52] 删除指定行
来源：http://hz.quarkkingdee.top/gtwkdrirgv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtwxumkrzw.html

[Q53] 按条件删除
来源：http://hz.xinyue.icu/gtcwqmxvje.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tianlin.xyz/gtjujreqgm.html

[Q54] 清空表
来源：http://hz.nanxinkj.top/gtwzsbcius.html

TRUNCATE TABLE logs;
来源：http://hz.daria6918.cn/gtimttwbbj.html

[Q55] 排名（并列占位）
来源：http://hz.hammf.cn/gtcbhkkled.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtaztlpefy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pengpengdd.cyou/gtimkrxxzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ydjk.org.cn/gtbmdagukc.html

[Q57] 行号
来源：http://hz.dashuyun.cn/gtmiqictnh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cucudq.cn/gturkorvwy.html

[Q58] 累计求和
来源：http://hz.ydjk.org.cn/gtdluafumf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258.top/gthkewoubm.html

[Q59] 分组内累计
来源：http://hz.yvedp.cn/gtdfwnvcsm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gttixbyanh.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydzc1.top/gtfkrexgln.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.9152youxi.cn/gtaunjruwo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pengpengdd.cyou/gtoljnxrnk.html

[Q61] 移动平均
来源：http://hz.52xcode.cn/gtlaivkwff.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ybcxt.top/gthxbzjvkv.html

[Q62] 分组占比
来源：http://hz.shangyingyoupin.top/gtvhkkegse.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gthhpiurdw.html

[Q63] 开启事务
来源：http://hz.hongshengwenyu.top/gtubuzamfx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigfzy.top/gtwkyimivc.html

[Q64] 提交事务
来源：http://hz.daxiang520.top/gthoreenjc.html

COMMIT;
来源：http://hz.yvedp.cn/gtovljmeqd.html

[Q65] 回滚事务
来源：http://hz.wangshuangyany.cn/gtkmzswtbn.html

ROLLBACK;
来源：http://hz.mhx1999.top/gtepvhbqeq.html

[Q66] 行锁查询
来源：http://hz.sysykeji.top/gtzbwylnhh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj202588.top/gttkkgoqts.html

[Q67] 设置隔离级别
来源：http://hz.jqgfzy.top/gtppevoyis.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jlsjyb.cn/gtvkmsvxnv.html

[Q68] 保存点
来源：http://hz.hnxiangtu.top/gtoyazbdae.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtkkpphmnm.html

ROLLBACK TO sp1;
来源：http://hz.ehwqpu.com/gtuedguexp.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gtxklvrker.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xinyue.icu/gtrwoxlpzm.html

[Q70] 更新统计信息
来源：http://hz.shuidangran.top/gtdbfnjcfc.html

ANALYZE TABLE users;
来源：http://hz.tian-w.cn/gtckhnnhoe.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtjfznriaz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258888.top/gtxaegnppf.html

[Q72] 查看索引
来源：http://hz.ybcxt.top/gtwmqcugqq.html

SHOW INDEX FROM users;
来源：http://hz.andypj.xyz/gtyretbqyd.html

[Q73] 查看表状态
来源：http://hz.chenlongwang.top/gtnylhzusw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnxiangtu.top/gtmjepgors.html

[Q74] 强制使用索引
来源：http://hz.gzhubu.top/gtgmjjimup.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhengqikj.top/gteaxadifg.html

[Q75] 日期格式化
来源：http://hz.c1oappe.top/gtjaiwivht.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hammf.cn/gtsayosmdm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jyoumei.cn/gtdldmyule.html

[Q76] 按天统计
来源：http://hz.yangfankeji.com/gtpxeieynd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhiwuduotai.top/gtsifgnmfu.html

[Q77] 时间加减
来源：http://hz.ivvv.top/gtgycrttog.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258.top/gtppnroeds.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gtijlnniic.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.haohaochexian.top/gtesmpzlhk.html

[Q79] 字符串拼接
来源：http://hz.wangdashe.top/gtbsjhtubd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.0kj1m.cn/gtkvnoaogl.html

[Q80] 字符串截取
来源：http://hz.iojbl.cn/gtzeckkwdm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gtpfzompvh.html

[Q81] 字符串替换
来源：http://hz.pengpengdd.cyou/gtayygguld.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yvedp.cn/gtyaftfuzg.html

[Q82] 字符长度与字节长度
来源：http://hz.iojbl.cn/gtflyltmeh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.c1oappe.top/gtzybxolzl.html

[Q83] 大小写转换
来源：http://hz.zdqjudy.top/gtouvdkuru.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gtvzgaoazh.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gtgknobxnw.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gtwqkptwee.html

[Q85] 数值取整
来源：http://hz.aibaodan.cn/gtyawltkyb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxinkj.top/gtdxahcsyx.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtjolwivld.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgufenzy.top/gtdfhtwztz.html

[Q87] JSON 字段做条件
来源：http://hz.gaohongyu789.top/gtraulnmzi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yvedp.cn/gtqsuzfpfw.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258.top/gtuuqvykao.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cqqwz.cn/gtxplukovh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gogol.net.cn/gtsddmdbds.html

[Q89] 判断表是否存在
来源：http://hz.quarkkingdee.top/gtgblwjpcp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daria6918.cn/gtmgxgysub.html

[Q90] 生成序号列
来源：http://hz.birdmap.top/gtzqiwbesh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tanke756.top/gtkrrmvpil.html

================================================================================
来源：http://hz.chenzaomai.com/gthuccgfbn.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gtmtaxvaqr.html

================================================================================
来源：http://hz.jyoumei.cn/gtvdfxffhh.html

[R01] shebang 与严格模式
来源：http://hz.xylfe.cn/gtrabzqsvj.html

#!/usr/bin/env bash
来源：http://hz.yongpay.top/gtvvyddjfk.html

set -euo pipefail
来源：http://hz.cashguo.top/gtntzfkokw.html

[R02] 变量赋值与使用
来源：http://hz.svipenyu.cn/gtcydzywrf.html

name="Tom"; echo "$name"
来源：http://hz.52xcode.cn/gtqpucikzv.html

[R03] 只读变量
来源：http://hz.snrcjt.cn/gtikhclmih.html

readonly PI=3.14
来源：http://hz.ydjk.org.cn/gtdofwxrcx.html

[R04] 位置参数
来源：http://hz.snrcjt.cn/gtqtaiwert.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuetiantiany.cn/gtudflfejf.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gtfzdnkhdt.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtzvrrucvr.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtoppkmdyn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj202588.top/gtjouseuwc.html

[R07] if 判断文件
来源：http://hz.gotoacloud.top/gtqexlbvud.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtmrgozjzl.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtjrkgofws.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgfzy.top/gtzmvwtfwv.html

[R09] 字符串比较
来源：http://hz.hongshengwenyu.top/gtmwnonwgc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hfpthk.cn/gtsaimkpeo.html

[R10] 正则匹配
来源：http://hz.gogol.net.cn/gtxgpibrqv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.meibo888.top/gtwneqosew.html

[R11] case 多分支
来源：http://hz.pycfn.com/gtxcbjvrgu.html

case "$1" in
来源：http://hz.dianchejie.cn/gtelfzenvo.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtxopglapr.html

stop)  echo "停止" ;;
来源：http://hz.guannengcc.top/gtlwooaetb.html

*)     echo "未知命令" ;;
来源：http://hz.9152youxi.cn/gtyifazqqv.html

esac
来源：http://hz.nanxinkj.top/gtpbyuuxak.html

[R12] for 遍历文件
来源：http://hz.jqgufenzy.top/gtzjnmerdg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuxming.cn/gttcbdiaea.html

[R13] for 计数循环
来源：http://hz.hnqzz.top/gtrwscormf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yonumen.top/gtcensekgf.html

[R14] C 风格 for
来源：http://hz.zdqjudy.top/gtnecvqwtn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daria6918.cn/gtkzfrgtmj.html

[R15] while 逐行读文件
来源：http://hz.sxryk.cn/gtmtgzhjyd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258.top/gtckrqtkhg.html

[R16] until 等待条件
来源：http://hz.cdnleiting.top/gtclrhppkc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj20258888.top/gtviebbeke.html

[R17] 数组定义与取值
来源：http://hz.yj20258888.top/gttjgfkyof.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinghuilouyu.cn/gtryohvqzl.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtxxlxjsfr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.mhx1999.top/gtrubdqzrq.html

[R19] 数组长度
来源：http://hz.shuidangran.top/gtrsunymvm.html

echo "${#arr[@]}"
来源：http://hz.xylfe.cn/gtqmkpzofw.html

[R20] 关联数组（字典）
来源：http://hz.hammf.cn/gthikqdmlf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ydzc1.top/gtiswablke.html

[R21] 字符串长度
来源：http://hz.fengsongda.top/gtfeazmarg.html

echo "${#s}"
来源：http://hz.andypj.xyz/gtsfkyqkzm.html

[R22] 截取子串
来源：http://hz.fzhhl.top/gtnathobnm.html

echo "${s:0:5}"
来源：http://hz.meibo888.top/gtoetrkffi.html

[R23] 字符串替换
来源：http://hz.nanxuanxn.top/gtgrwrmpve.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gttaqwjddj.html

[R24] 大小写转换
来源：http://hz.shuidangran.top/gtrnnxvnpy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.birdmap.top/gtocyedrzu.html

[R25] 去后缀 / 去前缀
来源：http://hz.sweek.top/gtwdqezkgv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.c1oappe.top/gtxtasieyf.html

[R26] 命令替换
来源：http://hz.hongshengwenyu.top/gttcylyghj.html

now=$(date +%F); echo "$now"
来源：http://hz.9152youxi.cn/gtyrbxvxcl.html

[R27] 算术展开
来源：http://hz.hfpthk.cn/gtriwnkrpm.html

echo $((1 + 2 * 3))
来源：http://hz.hnqzz.top/gtyzbafiqw.html

[R28] 浮点运算
来源：http://hz.fzhhl.top/gtnduelfxt.html

echo "scale=2; 10/3" | bc
来源：http://hz.redwolf501.top/gtfzimnlqe.html

[R29] 定义函数
来源：http://hz.xuetiantiany.cn/gtherlfqty.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ehwqpu.com/gtzoekxeoy.html

[R30] 函数返回状态码
来源：http://hz.c1oappe.top/gtcohxvfsv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jlsjyb.cn/gtkqjtcptg.html

[R31] 局部变量
来源：http://hz.jiagoushi.top/gtdijnajze.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinghuilouyu.cn/gtmmvqyhmk.html

[R32] 参数个数校验
来源：http://hz.redwolf501.top/gtfyvjzyxi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gogol.net.cn/gtxiraxfat.html

[R33] 捕获错误并提示行号
来源：http://hz.bjfxy.top/gtkpmsenuy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtmwiktizx.html

[R34] 退出时清理
来源：http://hz.yj202588.top/gtoqiwcctp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ehwqpu.com/gtfbvomxbw.html

[R35] 后台执行并等待
来源：http://hz.havefunace.top/gthoxmosyj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.redwolf501.top/gtyaftievr.html

[R36] 并发执行多个任务
来源：http://hz.hysaishi.cn/gtntqrssve.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gttgkuoapp.html

[R37] 把输出赋给变量
来源：http://hz.guannengcc.top/gtlhqoqjmv.html

files=$(ls -1)
来源：http://hz.yangfankeji.com/gtkvpgpmhd.html

[R38] 管道串联
来源：http://hz.0kj1m.cn/gtugegllif.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhixingplan.top/gtrpgardvm.html

[R39] 重定向标准输出与错误
来源：http://hz.hammf.cn/gtkxcbclwc.html

cmd > out.log 2>&1
来源：http://hz.kuanghao11.cn/gtmpeziilt.html

[R40] 追加写日志
来源：http://hz.zdqjudy.top/gtgwsmmugt.html

echo "log" >> out.log
来源：http://hz.zdqjudy.top/gtyjpyamsr.html

[R41] 丢弃输出
来源：http://hz.jqgufenzy.top/gtqaspnecm.html

cmd >/dev/null 2>&1
来源：http://hz.gogol.net.cn/gtexccllwf.html

[R42] 输入重定向
来源：http://hz.hnqzz.top/gtpbngovzf.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtwhebkltv.html

[R43] 按名字查找文件
来源：http://hz.birdmap.top/gtradmzptz.html

find . -name "*.log" -type f
来源：http://hz.316326.xyz/gtxqqycimv.html

[R44] 按修改时间查找
来源：http://hz.9152youxi.cn/gtewvknipe.html

find . -mtime -7 -type f
来源：http://hz.sxryk.cn/gtbwatzyge.html

[R45] 批量删除
来源：http://hz.fengsongda.top/gtqhvbccdk.html

find . -name "*.tmp" -delete
来源：http://hz.yuxming.cn/gtdaihmnqr.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gtukmrdnfp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jiagoushi.top/gtxunhmzow.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtnwcxoywo.html


<!-- 参考信息 -->