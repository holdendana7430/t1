代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.0kj1m.cn/gtmctvdlyb.html

[Q05] 重命名列
来源：http://hz.zhongyouzk.top/gtzjsugbjo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.vqdsnc.cn/gtijuakzfr.html

[Q06] 删除列
来源：http://hz.aibaodan.cn/gtblxcsohe.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.guannengcc.top/gtigznfnyr.html

[Q07] 删除表
来源：http://hz.zhoulong.xyz/gthztfmvvs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jyoumei.cn/gtvqxmmguw.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtqibafzyz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtjdmvengu.html

[Q09] 创建唯一索引
来源：http://hz.nanxuanxn.top/gtvzzvpvuj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cdnleiting.top/gtarfqjoej.html

[Q10] 插入单行
来源：http://hz.zhengqikj.top/gtumtgfcyw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xinyue.icu/gtopqekpbo.html

[Q11] 一次插入多行
来源：http://hz.andypj.xyz/gtaqpdgfhf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ivvv.top/gtqwibvrfv.html

[Q12] 插入后取自增 ID
来源：http://hz.zhongyouzk.top/gternkwlbm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dianchejie.cn/gtnorcitsa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jianghu66.top/gtxnfcupoj.html

[Q13] 忽略重复插入
来源：http://hz.aizwys.cn/gtpjmcjwlr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gzhubu.top/gtjhkkixbu.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenjidiqi.icu/gtaftmlemj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yangfankeji.com/gtiwmqdeec.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hammf.cn/gtoainqayr.html

[Q15] 查询全部
来源：http://hz.ywan-chungtsiang.top/gtdfaxceul.html

SELECT * FROM users;
来源：http://hz.xuetiantiany.cn/gtptdbwbyn.html

[Q16] 查询指定列
来源：http://hz.guowangkeji.top/gtzldqzafm.html

SELECT id, name FROM users;
来源：http://hz.yuxming.cn/gtgaanhqmf.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtbjgwpkdy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cqqwz.cn/gtmhuemeun.html

[Q18] 模糊匹配
来源：http://hz.xziqi.cn/gtktfaneko.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.redwolf501.top/gtzujptgtv.html

[Q19] 范围查询
来源：http://hz.hnxiangtu.top/gtljmdswom.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj20258.top/gtjrzchlxs.html

[Q20] IN 列表
来源：http://hz.sweek.top/gtpeorcvpf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shzxlz.cn/gtikqmqtbg.html

[Q21] 空值判断
来源：http://hz.fengsongda.top/gtaxqryqrg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gaohongyu789.top/gtayvottrp.html

[Q22] 排序
来源：http://hz.ywan-chungtsiang.top/gtixjxtbsd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sxryk.cn/gtsbstspot.html

[Q23] 分页
来源：http://hz.aizwys.cn/gtzryiavcw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shangyingyoupin.top/gtjpyyszlm.html

[Q24] 去重
来源：http://hz.shzxlz.cn/gttzwyqoio.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gtsmlrkzve.html

[Q25] 只取前 N 条
来源：http://hz.316326.xyz/gtsosucacw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gttjyjwybs.html

[Q26] 计数
来源：http://hz.andypj.xyz/gtlqzlfwjk.html

SELECT COUNT(*) FROM users;
来源：http://hz.sufxvd.cn/gtbuqynhtv.html

[Q27] 条件计数
来源：http://hz.tian-w.cn/gtilruxjjr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuanzx.com/gtrajkvcqu.html

[Q28] 求和与平均
来源：http://hz.yanxiufei.cn/gtbemanwdj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gttuncmxkl.html

[Q29] 最大最小值
来源：http://hz.hywenlv.cn/gtynyyzsth.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dianchejie.cn/gtoiwqsbdk.html

[Q30] 分组统计
来源：http://hz.svipenyu.cn/gtvljzeclj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtvrsvnbyk.html

[Q31] 分组后过滤
来源：http://hz.zhixingplan.top/gtutmjqzlr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daxiang520.top/gtowbeeewc.html

[Q32] 分组拼接字符串
来源：http://hz.chenzaomai.com/gtjwycvpsp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtcuylkoza.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pycfn.com/gthdknpvxn.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gttvngyaeu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258.top/gttyiincga.html

[Q34] 每组取第一条
来源：http://hz.shuidangran.top/gtvsokmzhk.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtruqznrno.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fengsongda.top/gticzmmuan.html

) t WHERE rn = 1;
来源：http://hz.mhx1999.top/gtnuizqazv.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gtlrzrppql.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtxbtwjniq.html

[Q36] 左连接
来源：http://hz.feifeiyinyue.top/gtpgdsmyjo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtchoftzcd.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gtridynsli.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ppjwa.cn/gtgsmbtlso.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhiwuduotai.top/gtonpouiis.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sweek.top/gtcdlndynv.html

[Q39] 自连接（查上下级）
来源：http://hz.xuanzx.com/gtvgqofohe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.guowangkeji.top/gtblrxncbh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aizwys.cn/gtzhadlonn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj20258.top/gtsyfnmwfr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hammf.cn/gtzbcukppc.html

[Q41] 多表连接
来源：http://hz.sweek.top/gtfudlpcbx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tanke756.top/gttegnogkc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtqrqlhtkz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aibaodan.cn/gtkabwyvrl.html

[Q42] 连接条件附加过滤
来源：http://hz.gogol.net.cn/gttwuznysa.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangshuangyany.cn/gtgoybaids.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhixingplan.top/gttyfwjduo.html

[Q43] 标量子查询
来源：http://hz.nanxinkj.top/gtyxbnkrcz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhengqikj.top/gtojidrcpw.html

[Q44] IN 子查询
来源：http://hz.yuxming.cn/gtzzhsckic.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtdotmaijr.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtlsggvdne.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtotpsohcf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gzhubu.top/gtglobbgsy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gtqnivnyxn.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtfbzufcku.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.mhx1999.top/gtrmfmordm.html

[Q48] CTE 公用表表达式
来源：http://hz.yanxiufei.cn/gtgexohvwu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aizwys.cn/gtytogxhtq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cheryme.top/gtgmlsdqvz.html

[Q49] 更新单行
来源：http://hz.gaohongyu789.top/gtggoqmlah.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.c1oappe.top/gtxdhsqvtl.html

[Q50] 批量更新
来源：http://hz.nanxinkj.top/gtkmpmbwpj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtswnsfrsm.html

[Q51] 用子查询更新
来源：http://hz.gotoacloud.top/gtzpzilgon.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtnwknyyal.html

[Q52] 删除指定行
来源：http://hz.jianghu66.top/gtphhmtvuu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtftjdczdc.html

[Q53] 按条件删除
来源：http://hz.cqqwz.cn/gthhnvvcyg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinyuanbaomall.cn/gtbqafvzzc.html

[Q54] 清空表
来源：http://hz.snrcjt.cn/gtegjucxkb.html

TRUNCATE TABLE logs;
来源：http://hz.fzhhl.top/gtksmvmjbx.html

[Q55] 排名（并列占位）
来源：http://hz.ydjk.org.cn/gtrhsjpglj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtnrscwuln.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgufenzy.top/gtjmfwqtfe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtibpvhkye.html

[Q57] 行号
来源：http://hz.zhongyouzk.top/gtkspxnpjf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yvedp.cn/gtwdvedfov.html

[Q58] 累计求和
来源：http://hz.yangfankeji.com/gtnxuaozov.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.vqdsnc.cn/gtxhpeodpf.html

[Q59] 分组内累计
来源：http://hz.andypj.xyz/gtrfqfzyiv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guannengcc.top/gtrygvmlik.html

[Q60] 取上一行 / 下一行
来源：http://hz.sweek.top/gtvazvafxs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gtelzfqaop.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shuidangran.top/gtbaiasegi.html

[Q61] 移动平均
来源：http://hz.yonumen.top/gtfpzljwkl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ybcxt.top/gtxwenrwef.html

[Q62] 分组占比
来源：http://hz.iojbl.cn/gtyazzpsws.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtkqrlfvpj.html

[Q63] 开启事务
来源：http://hz.sxryk.cn/gtjspwbcff.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhongyouzk.top/gtasthpbxr.html

[Q64] 提交事务
来源：http://hz.zhixingplan.top/gtcnsfdulp.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gtzmlrznmt.html

[Q65] 回滚事务
来源：http://hz.yj20258888.top/gtvxcwcodz.html

ROLLBACK;
来源：http://hz.hammf.cn/gtecyistgs.html

[Q66] 行锁查询
来源：http://hz.gaohongyu789.top/gtexdzeazh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jlsjyb.cn/gtsaxrxizw.html

[Q67] 设置隔离级别
来源：http://hz.birdmap.top/gtovsbzyvg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xinyue.icu/gtshsdiqgg.html

[Q68] 保存点
来源：http://hz.wangshuangyany.cn/gtwqjbbvoo.html

SAVEPOINT sp1;
来源：http://hz.aizwys.cn/gtuweschjw.html

ROLLBACK TO sp1;
来源：http://hz.316326.xyz/gtgqgnikqx.html

[Q69] 查看执行计划
来源：http://hz.zhoulong.xyz/gtcdygular.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenzaomai.com/gtfkorfodn.html

[Q70] 更新统计信息
来源：http://hz.tian-w.cn/gtywmxdnzv.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gtgpvtzmxp.html

[Q71] 查看建表语句
来源：http://hz.jqgfzy.top/gtnfjzijwr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sxryk.cn/gtfztogkhj.html

[Q72] 查看索引
来源：http://hz.zhixingplan.top/gtpnorornd.html

SHOW INDEX FROM users;
来源：http://hz.52xcode.cn/gtfbfwpzcn.html

[Q73] 查看表状态
来源：http://hz.jqgfzy.top/gteawkfmrq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtowzzypbh.html

[Q74] 强制使用索引
来源：http://hz.jlsjyb.cn/gtfuxyjzgo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gtgsympzks.html

[Q75] 日期格式化
来源：http://hz.ywan-chungtsiang.top/gtwdncnpfi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtickczvbd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtwswvujui.html

[Q76] 按天统计
来源：http://hz.pycfn.com/gtbvfznpyc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jianghu66.top/gtaekzrxhi.html

[Q77] 时间加减
来源：http://hz.gogol.net.cn/gtqmiectxm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydjk.org.cn/gtsyrryoyn.html

[Q78] 当前时间
来源：http://hz.wangdashe.top/gthznlbxnd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hywenlv.cn/gtblsbzskc.html

[Q79] 字符串拼接
来源：http://hz.jianghu66.top/gtxdcprnrl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.bjfxy.top/gtbsfzwlqy.html

[Q80] 字符串截取
来源：http://hz.gogol.net.cn/gtbtxpqjyh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtzfmlwkyj.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtiwdswhbb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dianchejie.cn/gtaldlzfsv.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gthgijqlwx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgfzy.top/gtvydqctgf.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtbhcmdxjo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.quarkkingdee.top/gtzliaoqvc.html

[Q84] 去除首尾空格
来源：http://hz.c1oappe.top/gtqtzwlnec.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gtjzsorxto.html

[Q85] 数值取整
来源：http://hz.tianlin.xyz/gtlsiqdzug.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jyoumei.cn/gtlkzbtrsb.html

[Q86] 读取 JSON 字段
来源：http://hz.yj202588.top/gtuuboaojr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gotoacloud.top/gtzktcxzph.html

[Q87] JSON 字段做条件
来源：http://hz.xingfuxueyuan.xyz/gtrhmkfnuy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zdqjudy.top/gtbvuiceqq.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtztzrgizv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sxryk.cn/gtwalqvhbx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxuanxn.top/gtuytniqed.html

[Q89] 判断表是否存在
来源：http://hz.yuanzhike.top/gtczthzxkq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtrtikfxqm.html

[Q90] 生成序号列
来源：http://hz.iojbl.cn/gtmxtsmuvs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xylfe.cn/gtjtowyzed.html

================================================================================
来源：http://hz.ydzc1.top/gtcdpsktnx.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtxrnwzyvn.html

================================================================================
来源：http://hz.shzxlz.cn/gtxybkeekl.html

[R01] shebang 与严格模式
来源：http://hz.ppjwa.cn/gtxgabfpqw.html

#!/usr/bin/env bash
来源：http://hz.hongshengwenyu.top/gtokhgvqso.html

set -euo pipefail
来源：http://hz.tian-w.cn/gtuokesemk.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtoswonhjo.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtbwkubpyx.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtqoupbrjp.html

readonly PI=3.14
来源：http://hz.shanyushiyangtech.top/gtiterdfva.html

[R04] 位置参数
来源：http://hz.ivvv.top/gtptretwjv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hongshengwenyu.top/gtfhehranx.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtnrhfjnhc.html

name="${1:-default}"
来源：http://hz.shzxlz.cn/gtpmptqjkl.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtbuqullzv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtrccowwzy.html

[R07] if 判断文件
来源：http://hz.fengsongda.top/gtttvfaqzf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigfzy.top/gtvqydgihe.html

[R08] 数值比较
来源：http://hz.cheryme.top/gtfjcogtvb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cucudq.cn/gtqupmzddy.html

[R09] 字符串比较
来源：http://hz.ivvv.top/gtmogvojfb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtctfxrdab.html

[R10] 正则匹配
来源：http://hz.haohaochexian.top/gtssvinofo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gtesyhgpye.html

[R11] case 多分支
来源：http://hz.hfpthk.cn/gtkfgktwhz.html

case "$1" in
来源：http://hz.jinqigufen.top/gtlpcaxsfz.html

start) echo "启动" ;;
来源：http://hz.yanxiufei.cn/gtcsuvvfnh.html

stop)  echo "停止" ;;
来源：http://hz.nanxinkj.top/gtwntzbnjp.html

*)     echo "未知命令" ;;
来源：http://hz.zhengqikj.top/gttwwayvqe.html

esac
来源：http://hz.jqgfzy.top/gtpdcnhcfv.html

[R12] for 遍历文件
来源：http://hz.yueranfly.top/gtkkrcuxbv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sweek.top/gtfvjhoxgz.html

[R13] for 计数循环
来源：http://hz.zhijiandao.cn/gtpftbmmkt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jyoumei.cn/gtzbpcqlpb.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gtwyiwuqin.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtmfnjrtir.html

[R15] while 逐行读文件
来源：http://hz.yongpay.top/gtrvrkyqrg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhaomingkeji.xyz/gtooxkpxsy.html

[R16] until 等待条件
来源：http://hz.nanxuanxn.top/gtlryojxlw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aizwys.cn/gtohptmpqa.html

[R17] 数组定义与取值
来源：http://hz.zhijiandao.cn/gthikkdnnf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnqzz.top/gtiuijemyg.html

[R18] 遍历数组
来源：http://hz.yvedp.cn/gtfbianzml.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtfjoonhwn.html

[R19] 数组长度
来源：http://hz.birdmap.top/gtrqwnddey.html

echo "${#arr[@]}"
来源：http://hz.xinyue.icu/gtsdbyepek.html

[R20] 关联数组（字典）
来源：http://hz.gzhubu.top/gtxhiivoho.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.chenzaomai.com/gtnnuocghc.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtiinyujgc.html

echo "${#s}"
来源：http://hz.ydjk.org.cn/gtylczxqwz.html

[R22] 截取子串
来源：http://hz.tian-w.cn/gtoduqxtcy.html

echo "${s:0:5}"
来源：http://hz.316326.xyz/gtabzkozku.html

[R23] 字符串替换
来源：http://hz.andypj.xyz/gthfppqfuo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuanzx.com/gtqhdocxkr.html

[R24] 大小写转换
来源：http://hz.yj20258888.top/gtidjdzotd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtudjngycs.html

[R25] 去后缀 / 去前缀
来源：http://hz.yongpay.top/gtwzfcpmjb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tian-w.cn/gtdmmecqxb.html

[R26] 命令替换
来源：http://hz.yonumen.top/gtbtmpqoaa.html

now=$(date +%F); echo "$now"
来源：http://hz.c1oappe.top/gtjmjnujkn.html

[R27] 算术展开
来源：http://hz.gaohongyu789.top/gtmjcgflhr.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtpantzbjy.html

[R28] 浮点运算
来源：http://hz.fengsongda.top/gttnmyigyj.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gthyhivvmo.html

[R29] 定义函数
来源：http://hz.birdmap.top/gtztckfvnq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj202588.top/gtglbmttye.html

[R30] 函数返回状态码
来源：http://hz.bjfxy.top/gtmuuombpp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cucudq.cn/gtftpwricw.html

[R31] 局部变量
来源：http://hz.tianlin.xyz/gtrxxnlhhu.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj20258888.top/gtqfwrmube.html

[R32] 参数个数校验
来源：http://hz.jinqigfzy.top/gtmxxhaegz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hfpthk.cn/gtzyqiejcy.html

[R33] 捕获错误并提示行号
来源：http://hz.aibaodan.cn/gtjdubpoxe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.svipenyu.cn/gtlmffhrsr.html

[R34] 退出时清理
来源：http://hz.quarkkingdee.top/gtjnflrhpi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtugbjawed.html

[R35] 后台执行并等待
来源：http://hz.tian-w.cn/gtfjjieogd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtutxyzqfi.html

[R36] 并发执行多个任务
来源：http://hz.sufxvd.cn/gtlcfnabud.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.9152youxi.cn/gtioixrvms.html

[R37] 把输出赋给变量
来源：http://hz.cdnleiting.top/gtopinvrjk.html

files=$(ls -1)
来源：http://hz.kuanghao11.cn/gtitnwpmio.html

[R38] 管道串联
来源：http://hz.jiagoushi.top/gtrcpiydsd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yongpay.top/gtpdgqoulv.html

[R39] 重定向标准输出与错误
来源：http://hz.yvedp.cn/gthnhhnpdu.html

cmd > out.log 2>&1
来源：http://hz.zhijiandao.cn/gtopsrqssm.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtehmlmydl.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtzzzbhzlc.html

[R41] 丢弃输出
来源：http://hz.52xcode.cn/gtolnnbwye.html

cmd >/dev/null 2>&1
来源：http://hz.tianlin.xyz/gtmktgtlho.html

[R42] 输入重定向
来源：http://hz.cashguo.top/gtxpridgws.html

wc -l < a.txt
来源：http://hz.yongpay.top/gtikxyklcc.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gtctlulqdv.html

find . -name "*.log" -type f
来源：http://hz.guowangkeji.top/gtqnxnzbvf.html

[R44] 按修改时间查找
来源：http://hz.gotoacloud.top/gtyxxwavnq.html

find . -mtime -7 -type f
来源：http://hz.xuanzx.com/gtsbxjenqs.html

[R45] 批量删除
来源：http://hz.shzxlz.cn/gtedjmyxlq.html

find . -name "*.tmp" -delete
来源：http://hz.yj202588.top/gtmahpvnty.html

[R46] 递归替换文件内容
来源：http://hz.hywenlv.cn/gtsnmceuoo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sweek.top/gtzkehihoi.html

[R47] sed 单行替换
来源：http://hz.cqqwz.cn/gtsfkffgis.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guowangkeji.top/gthxorflit.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtunbyiftv.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhijiandao.cn/gtxuyniplz.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gtanueovmg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.9152youxi.cn/gtmadztxwv.html

[R50] awk 求和
来源：http://hz.cqqwz.cn/gtktsqevef.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hywenlv.cn/gtrjugdpwx.html

[R51] 排序去重取前几
来源：http://hz.aibaodan.cn/gtdqodiayu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shuidangran.top/gtflwohyet.html

[R52] 统计行数
来源：http://hz.yongpay.top/gtntoqqpak.html

wc -l a.txt
来源：http://hz.vqdsnc.cn/gtppnwcqnc.html

[R53] 查看文件头与实时尾
来源：http://hz.yanxiufei.cn/gtacugzblk.html


<!-- 参考信息 -->