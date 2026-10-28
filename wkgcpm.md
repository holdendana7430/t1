代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangshuangyany.cn/gtxxgnxnla.html

[Q05] 重命名列
来源：http://hz.hongshengwenyu.top/gtzufkyqft.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gotoacloud.top/gtphhtsznu.html

[Q06] 删除列
来源：http://hz.yanxiufei.cn/gttckbltpv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hysaishi.cn/gtsmtnfsfl.html

[Q07] 删除表
来源：http://hz.daxiang520.top/gtbbaphhun.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnxiangtu.top/gtvruugklp.html

[Q08] 创建普通索引
来源：http://hz.ivvv.top/gtzbnobwic.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jiagoushi.top/gthjikmuow.html

[Q09] 创建唯一索引
来源：http://hz.sysykeji.top/gtrbmvapvn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fzhhl.top/gtbmoujjyu.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtungcxqcy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinyuanbaomall.cn/gtjhzijsfi.html

[Q11] 一次插入多行
来源：http://hz.iojbl.cn/gtzbvefrxq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuetiantiany.cn/gtkkjeepjr.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gthlikoaxk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cdnleiting.top/gtwruanmwb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.wangdashe.top/gthpnwtzne.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtvtgbawmq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangdashe.top/gtcwzdpcdk.html

[Q14] 存在则更新（upsert）
来源：http://hz.ivvv.top/gtvfohehge.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shangyingyoupin.top/gtncsxwpwt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hongshengwenyu.top/gtwyltsqsu.html

[Q15] 查询全部
来源：http://hz.gzhubu.top/gtgxgprvsd.html

SELECT * FROM users;
来源：http://hz.feifeiyinyue.top/gttxphruyz.html

[Q16] 查询指定列
来源：http://hz.316326.xyz/gtgxuioexk.html

SELECT id, name FROM users;
来源：http://hz.yanxiufei.cn/gtdqwtarib.html

[Q17] 条件查询
来源：http://hz.bjfxy.top/gtbqadquie.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhijiandao.cn/gtslnlprsi.html

[Q18] 模糊匹配
来源：http://hz.jinyuanbaomall.cn/gtirfwplop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daxiang520.top/gtohspljgd.html

[Q19] 范围查询
来源：http://hz.yongpay.top/gtilkjqugo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj20258.top/gtqtpuvowt.html

[Q20] IN 列表
来源：http://hz.316326.xyz/gtlccfoyos.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydjk.org.cn/gtvymywzcn.html

[Q21] 空值判断
来源：http://hz.hammf.cn/gtwlsbwgde.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sweek.top/gtfcxvjapb.html

[Q22] 排序
来源：http://hz.daxiang520.top/gtwpembuue.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.9152youxi.cn/gtovictzqv.html

[Q23] 分页
来源：http://hz.meibo888.top/gtgdlsesgh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuxming.cn/gtxjkikwva.html

[Q24] 去重
来源：http://hz.zhijiandao.cn/gtijuisnvl.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gtuptjllhc.html

[Q25] 只取前 N 条
来源：http://hz.hnqzz.top/gtegiaweiu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gtplygjrco.html

[Q26] 计数
来源：http://hz.fzhhl.top/gtfpvbuwiu.html

SELECT COUNT(*) FROM users;
来源：http://hz.shuidangran.top/gtyjnsnsna.html

[Q27] 条件计数
来源：http://hz.sxryk.cn/gtdzpdoyeo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jyoumei.cn/gtmskmechs.html

[Q28] 求和与平均
来源：http://hz.gogol.net.cn/gtssppvwga.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yanxiufei.cn/gtihiawmqp.html

[Q29] 最大最小值
来源：http://hz.zhengqikj.top/gtfrypopty.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtgvkhihtl.html

[Q30] 分组统计
来源：http://hz.xziqi.cn/gtpgonyimr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtwocbokyz.html

[Q31] 分组后过滤
来源：http://hz.zhaomingkeji.xyz/gtqdcxrpqw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gtbkxdyfug.html

[Q32] 分组拼接字符串
来源：http://hz.c1oappe.top/gtfddelgcg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtxgohtcoc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtbdwoizxh.html

[Q33] 多列分组
来源：http://hz.sxryk.cn/gtgdrcaftg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258888.top/gtqzvtpjpd.html

[Q34] 每组取第一条
来源：http://hz.xuanzx.com/gtskponkaz.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gtpskjcamp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dashuyun.cn/gteuhsqsrp.html

) t WHERE rn = 1;
来源：http://hz.tian-w.cn/gtppefjmfc.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gtbfcyzver.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gtxrwoopts.html

[Q36] 左连接
来源：http://hz.zhixingplan.top/gthixdmccs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhengqikj.top/gtotpgmmfn.html

[Q37] 右连接
来源：http://hz.tianlin.xyz/gtnvcwbxnc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinghuilouyu.cn/gtvqgnfmzu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gotoacloud.top/gtctesidhc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigfzy.top/gtyodxkatb.html

[Q39] 自连接（查上下级）
来源：http://hz.havefunace.top/gtdbhsfnae.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sweek.top/gtraqfjkrl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtucamhlbt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gaohongyu789.top/gtdwrjbfhv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.quarkkingdee.top/gtrygissjg.html

[Q41] 多表连接
来源：http://hz.wangdashe.top/gtvhwlcfxn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.c1oappe.top/gtdqxdshne.html

JOIN users u ON u.id = o.user_id
来源：http://hz.havefunace.top/gtubltxpqa.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtqlerbaxd.html

[Q42] 连接条件附加过滤
来源：http://hz.52xcode.cn/gtngjefwql.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnqzz.top/gtmksydfiz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtrxcbmwim.html

[Q43] 标量子查询
来源：http://hz.yanxiufei.cn/gtxvffzoif.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtltbvokil.html

[Q44] IN 子查询
来源：http://hz.nwbrower.top/gtmfohkkvg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yangfankeji.com/gtwfkvxohe.html

[Q45] EXISTS 判断存在
来源：http://hz.cashguo.top/gthpectxmu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gtjubtliqm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.havefunace.top/gtpwepwehz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtsnovdgec.html

[Q47] 与平均值比较
来源：http://hz.chenzaomai.com/gtrauocqke.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhaomingkeji.xyz/gtpdrczyad.html

[Q48] CTE 公用表表达式
来源：http://hz.nanxuanxn.top/gtdeadvxpv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nwbrower.top/gtipuzkzfh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenzaomai.com/gtspypedbb.html

[Q49] 更新单行
来源：http://hz.hysaishi.cn/gtrivrhkrg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtelcwrxlt.html

[Q50] 批量更新
来源：http://hz.feifeiyinyue.top/gtdiqbesjk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hywenlv.cn/gtskjsivzh.html

[Q51] 用子查询更新
来源：http://hz.gogol.net.cn/gtypzoymuc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.daria6918.cn/gtroydqarb.html

[Q52] 删除指定行
来源：http://hz.pycfn.com/gtcxcasqlu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cucudq.cn/gtlcrpjoij.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtpbzuxloj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jyoumei.cn/gtgozjiqgb.html

[Q54] 清空表
来源：http://hz.ppjwa.cn/gtuojomdux.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtudnmtael.html

[Q55] 排名（并列占位）
来源：http://hz.svipenyu.cn/gtvrmhvfur.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cdnleiting.top/gtcuaccvtv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pengpengdd.cyou/gtunbpxcpy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtpjbekhlv.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtjcjwujbk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtwjuhufeo.html

[Q58] 累计求和
来源：http://hz.316326.xyz/gtqrcwnqtt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hammf.cn/gtaraxtfjj.html

[Q59] 分组内累计
来源：http://hz.ehwqpu.com/gtlvuzpsxj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhongyouzk.top/gtmzjabshh.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtbqcvlgaa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sysykeji.top/gtvuiamusy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nwbrower.top/gtllagvlxd.html

[Q61] 移动平均
来源：http://hz.cdnleiting.top/gtyhevwyug.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sysykeji.top/gtawvzmcno.html

[Q62] 分组占比
来源：http://hz.xingfuxueyuan.xyz/gttbwwtdtw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtvpbkyair.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gtqbcrpwet.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sysykeji.top/gtzptzrhac.html

[Q64] 提交事务
来源：http://hz.jlsjyb.cn/gtmogqxvky.html

COMMIT;
来源：http://hz.havefunace.top/gttutkmfrm.html

[Q65] 回滚事务
来源：http://hz.fengsongda.top/gtlcgauljo.html

ROLLBACK;
来源：http://hz.chenzaomai.com/gtatkwezde.html

[Q66] 行锁查询
来源：http://hz.sysykeji.top/gtqlkwaldh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtuyflgcrq.html

[Q67] 设置隔离级别
来源：http://hz.aizwys.cn/gtakwhdnzg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhoulong.xyz/gtkpawrygq.html

[Q68] 保存点
来源：http://hz.zhiwuduotai.top/gtsmjlalzx.html

SAVEPOINT sp1;
来源：http://hz.jqgfzy.top/gtsimppgqf.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gtqmrahfwm.html

[Q69] 查看执行计划
来源：http://hz.fzhhl.top/gtceiuyixs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.haohaochexian.top/gtwtqnedgz.html

[Q70] 更新统计信息
来源：http://hz.pycfn.com/gtoqrheeno.html

ANALYZE TABLE users;
来源：http://hz.xylfe.cn/gtcchsuasd.html

[Q71] 查看建表语句
来源：http://hz.aizwys.cn/gtikpznyed.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtulxqfeoz.html

[Q72] 查看索引
来源：http://hz.haohaochexian.top/gtorbuaptc.html

SHOW INDEX FROM users;
来源：http://hz.jinghuilouyu.cn/gtzjsdvhca.html

[Q73] 查看表状态
来源：http://hz.0kj1m.cn/gtjrqdwysa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gogol.net.cn/gtclvdruwm.html

[Q74] 强制使用索引
来源：http://hz.tanke756.top/gtyqifeegb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.aizwys.cn/gtntgnslgh.html

[Q75] 日期格式化
来源：http://hz.meibo888.top/gthjkxcvfp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gtqquqrsvv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhijiandao.cn/gtaktrdfev.html

[Q76] 按天统计
来源：http://hz.jinqigfzy.top/gtrarqkmkp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.haohaochexian.top/gtejzqlqak.html

[Q77] 时间加减
来源：http://hz.bjfxy.top/gtdgywtakr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinyuanbaomall.cn/gtcebzlnsr.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gtmiamjpem.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenzaomai.com/gtzcjunfnb.html

[Q79] 字符串拼接
来源：http://hz.jyoumei.cn/gtcimczkvn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nwbrower.top/gtcrxfqasu.html

[Q80] 字符串截取
来源：http://hz.cheryme.top/gtifsllcdn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigfzy.top/gtluoqburx.html

[Q81] 字符串替换
来源：http://hz.sysykeji.top/gtsjmwolwd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hywenlv.cn/gtabymfkjc.html

[Q82] 字符长度与字节长度
来源：http://hz.sufxvd.cn/gtnxowozgm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtqjfofvhj.html

[Q83] 大小写转换
来源：http://hz.gzhubu.top/gtuputafxe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cashguo.top/gtprrtyeko.html

[Q84] 去除首尾空格
来源：http://hz.tanke756.top/gtudfitkkh.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gtyalefkns.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtjkzuzswo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenzaomai.com/gtbipxeztc.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtbqdnhrsl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenjidiqi.icu/gtghmplesv.html

[Q87] JSON 字段做条件
来源：http://hz.yvedp.cn/gtxtfglrjy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gtbsuunyhw.html

[Q88] 行转列（条件聚合）
来源：http://hz.yonumen.top/gtxywmgbii.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtjsplwrny.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxinkj.top/gteswpwqac.html

[Q89] 判断表是否存在
来源：http://hz.jinqigfzy.top/gtpwekzklx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yongpay.top/gtxjnefaxn.html

[Q90] 生成序号列
来源：http://hz.jinyuanbaomall.cn/gtvdenfjda.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxinkj.top/gtqwylmcid.html

================================================================================
来源：http://hz.xuanzx.com/gtoaesmquy.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtysftvldt.html

================================================================================
来源：http://hz.c1oappe.top/gtrnskztkg.html

[R01] shebang 与严格模式
来源：http://hz.mhx1999.top/gtgprklquc.html

#!/usr/bin/env bash
来源：http://hz.xinyue.icu/gtwbxhwdnj.html

set -euo pipefail
来源：http://hz.yj202588.top/gtgfweoftl.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangtech.top/gtwxlwieui.html

name="Tom"; echo "$name"
来源：http://hz.ehwqpu.com/gtlhbrlafv.html

[R03] 只读变量
来源：http://hz.haohaochexian.top/gtejtiurot.html

readonly PI=3.14
来源：http://hz.nwbrower.top/gttmoabmdj.html

[R04] 位置参数
来源：http://hz.cqqwz.cn/gtlzznoxlr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.aibaodan.cn/gthqrkbjsz.html

[R05] 参数默认值
来源：http://hz.hysaishi.cn/gtsphvufcx.html

name="${1:-default}"
来源：http://hz.hfpthk.cn/gtylhtbhsm.html

[R06] 判断命令是否存在
来源：http://hz.jinqigfzy.top/gtyiyqfhnb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yangfankeji.com/gtnnxvjxgq.html

[R07] if 判断文件
来源：http://hz.zycfv.cn/gthveavnml.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258.top/gtkajtaiqm.html

[R08] 数值比较
来源：http://hz.cucudq.cn/gtijshueas.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.feifeiyinyue.top/gtdzxkohgw.html

[R09] 字符串比较
来源：http://hz.dianchejie.cn/gtwagojkwa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xinyue.icu/gtpvkpedvh.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtdfkxegfi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtkhohxhmq.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtjbogakny.html

case "$1" in
来源：http://hz.hnqzz.top/gtysgpjjjq.html

start) echo "启动" ;;
来源：http://hz.birdmap.top/gtstwtflmb.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtjgqpsdyw.html

*)     echo "未知命令" ;;
来源：http://hz.ehwqpu.com/gtpsbgrsgc.html

esac
来源：http://hz.shangyingyoupin.top/gtvitcljto.html

[R12] for 遍历文件
来源：http://hz.yongpay.top/gtgrhnuonw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hysaishi.cn/gtfhexlmum.html

[R13] for 计数循环
来源：http://hz.zycfv.cn/gtaesdyvdm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.vqdsnc.cn/gthgjsvanc.html

[R14] C 风格 for
来源：http://hz.0kj1m.cn/gtmdlmahsm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtljwqipxk.html

[R15] while 逐行读文件
来源：http://hz.nanxuanxn.top/gtqvijangb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daria6918.cn/gtzqwdisjw.html

[R16] until 等待条件
来源：http://hz.hnxiangtu.top/gtqpmibwje.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zycfv.cn/gtfdxnzmtv.html

[R17] 数组定义与取值
来源：http://hz.yanxiufei.cn/gtqorvpeci.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nwbrower.top/gtnalioyuk.html

[R18] 遍历数组
来源：http://hz.zhoulong.xyz/gttmgjbdwt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zycfv.cn/gtfybpruwc.html

[R19] 数组长度
来源：http://hz.hfpthk.cn/gtkoslzhye.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtdvirhghi.html

[R20] 关联数组（字典）
来源：http://hz.sufxvd.cn/gtnsgwpfid.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.havefunace.top/gtcpduokzv.html

[R21] 字符串长度
来源：http://hz.0kj1m.cn/gtjvgvxkyc.html

echo "${#s}"
来源：http://hz.cdnleiting.top/gticrqysts.html

[R22] 截取子串
来源：http://hz.jiagoushi.top/gtkllstiar.html

echo "${s:0:5}"
来源：http://hz.jlsjyb.cn/gtnazvhrld.html

[R23] 字符串替换
来源：http://hz.smart0.xyz/gtcoflidyc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhengqikj.top/gtsniltmik.html

[R24] 大小写转换
来源：http://hz.pengpengdd.cyou/gtwompjbmi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.9152youxi.cn/gtdxubcrut.html

[R25] 去后缀 / 去前缀
来源：http://hz.shangyingyoupin.top/gtmlinviov.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tanke756.top/gtzyqijtta.html

[R26] 命令替换
来源：http://hz.yuxming.cn/gtynmozkqq.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtlvqcxqli.html

[R27] 算术展开
来源：http://hz.gogol.net.cn/gtpwtwsjem.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtcvfuvsvd.html

[R28] 浮点运算
来源：http://hz.yanxiufei.cn/gtouwwghiy.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangtech.top/gtmajcidnk.html

[R29] 定义函数
来源：http://hz.cashguo.top/gtnypouhbw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hammf.cn/gtbvyrkyuc.html

[R30] 函数返回状态码
来源：http://hz.bjfxy.top/gtgsaahepz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258.top/gtxhsshtya.html

[R31] 局部变量
来源：http://hz.sufxvd.cn/gtztcanmdn.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenzaomai.com/gtcaqdujqw.html

[R32] 参数个数校验
来源：http://hz.yueranfly.top/gtxcelcwlb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jlsjyb.cn/gtlaadiajd.html

[R33] 捕获错误并提示行号
来源：http://hz.nanxinkj.top/gtgzyoqpnw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhaomingkeji.xyz/gturjswerw.html

[R34] 退出时清理
来源：http://hz.meibo888.top/gteyjcbiqw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shangyingyoupin.top/gtapnxhmne.html

[R35] 后台执行并等待
来源：http://hz.cheryme.top/gthskcvatw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.c1oappe.top/gtzecmdpgu.html

[R36] 并发执行多个任务
来源：http://hz.pycfn.com/gtdnodmmtm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtswusdoaw.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtiowfezgg.html

files=$(ls -1)
来源：http://hz.zdqjudy.top/gtoyjgubwy.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtdxhjzqej.html

cat a.txt | grep -i error | wc -l
来源：http://hz.c1oappe.top/gtmbvppmjm.html

[R39] 重定向标准输出与错误
来源：http://hz.jinyuanbaomall.cn/gtgcehzeqw.html

cmd > out.log 2>&1
来源：http://hz.tian-w.cn/gtqaycttbv.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtxvynbvfm.html

echo "log" >> out.log
来源：http://hz.hnxiangtu.top/gtuxmogpip.html

[R41] 丢弃输出
来源：http://hz.cqqwz.cn/gtiwvfefsi.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtkeljvqwz.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtnaurjgts.html

wc -l < a.txt
来源：http://hz.meibo888.top/gtjubmepnb.html

[R43] 按名字查找文件
来源：http://hz.jyoumei.cn/gtzejauzih.html

find . -name "*.log" -type f
来源：http://hz.ivvv.top/gtugrzizof.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtwbpxgfpw.html

find . -mtime -7 -type f
来源：http://hz.hfpthk.cn/gtockhjooc.html

[R45] 批量删除
来源：http://hz.sufxvd.cn/gtcqekfkxj.html

find . -name "*.tmp" -delete
来源：http://hz.chenlongwang.top/gtipmuzoit.html

[R46] 递归替换文件内容
来源：http://hz.meibo888.top/gtgyihxrnx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.9152youxi.cn/gtvpehvoqu.html

[R47] sed 单行替换
来源：http://hz.xuetiantiany.cn/gtovqyrdbw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aibaodan.cn/gtecqtlvjv.html

[R48] awk 取指定列
来源：http://hz.tanke756.top/gtrfgakdhm.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gtqjwtmoxh.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtgjwktklk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xziqi.cn/gtslojnkpo.html

[R50] awk 求和
来源：http://hz.zhijiandao.cn/gtecyayvbc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtsbpvkcyk.html

[R51] 排序去重取前几
来源：http://hz.hfpthk.cn/gtvjgwbgtp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinqigufen.top/gtuomtwqdk.html

[R52] 统计行数
来源：http://hz.ehwqpu.com/gtzeqbozei.html

wc -l a.txt
来源：http://hz.jinyuanbaomall.cn/gtfkssxlkb.html

[R53] 查看文件头与实时尾
来源：http://hz.wangshuangyany.cn/gtqupyvqaf.html


<!-- 参考信息 -->