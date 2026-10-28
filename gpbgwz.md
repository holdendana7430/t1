代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtgajtlezg.html

[Q09] 创建唯一索引
来源：http://hz.0kj1m.cn/gtqwvwqjkc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtlhrrmlpp.html

[Q10] 插入单行
来源：http://hz.ivvv.top/gtxlmhfldw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ywan-chungtsiang.top/gtgsdftmsk.html

[Q11] 一次插入多行
来源：http://hz.fzhhl.top/gtkxaqqkyy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinghuilouyu.cn/gtqitnwbtx.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtbouxlikk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gtbppghngh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gtcvjcrxcc.html

[Q13] 忽略重复插入
来源：http://hz.chenjidiqi.icu/gtzfyplfcp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangtech.top/gtnedftogl.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gtqzquislf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hywenlv.cn/gtvfsxgcuf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.dashuyun.cn/gtujdhaepq.html

[Q15] 查询全部
来源：http://hz.jyoumei.cn/gtwzwvqxci.html

SELECT * FROM users;
来源：http://hz.ppjwa.cn/gtddnfvnyc.html

[Q16] 查询指定列
来源：http://hz.jiagoushi.top/gtajygprld.html

SELECT id, name FROM users;
来源：http://hz.zhengqikj.top/gthcxhxtat.html

[Q17] 条件查询
来源：http://hz.ehwqpu.com/gtvbuybboc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxinkj.top/gthgzevvrg.html

[Q18] 模糊匹配
来源：http://hz.jqgfzy.top/gtjgkedbak.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.snrcjt.cn/gtggptphiy.html

[Q19] 范围查询
来源：http://hz.smart0.xyz/gtdmwieaac.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.iojbl.cn/gttyowssla.html

[Q20] IN 列表
来源：http://hz.dianchejie.cn/gtkpmpynsc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ehwqpu.com/gthvutshbz.html

[Q21] 空值判断
来源：http://hz.xziqi.cn/gtsyznjeov.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenlongwang.top/gtzjcsichg.html

[Q22] 排序
来源：http://hz.cashguo.top/gtjocpmcje.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zycfv.cn/gtllfbocci.html

[Q23] 分页
来源：http://hz.xylfe.cn/gtsyhgwlgn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.meibo888.top/gtirilcrlc.html

[Q24] 去重
来源：http://hz.aibaodan.cn/gtdeeahddl.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxuanxn.top/gtuoqoghmk.html

[Q25] 只取前 N 条
来源：http://hz.quarkkingdee.top/gtojozimxe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gtrnedzkhg.html

[Q26] 计数
来源：http://hz.jinqigfzy.top/gtzdtouhis.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydzc1.top/gtvrcqcnka.html

[Q27] 条件计数
来源：http://hz.zycfv.cn/gtdzyxfqgw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.svipenyu.cn/gtmqntjdka.html

[Q28] 求和与平均
来源：http://hz.aibaodan.cn/gtzkqxusof.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daxiang520.top/gtmqdnklfy.html

[Q29] 最大最小值
来源：http://hz.gzhubu.top/gtixdiuggb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgufenzy.top/gtpgqmxejn.html

[Q30] 分组统计
来源：http://hz.316326.xyz/gtatzhorqb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtyzlhcqhj.html

[Q31] 分组后过滤
来源：http://hz.sufxvd.cn/gtvwqtkjfe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pengpengdd.cyou/gtogypsvzd.html

[Q32] 分组拼接字符串
来源：http://hz.ydjk.org.cn/gtykobmvou.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtwvznrspm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.kuanghao11.cn/gtgavldnzt.html

[Q33] 多列分组
来源：http://hz.pengpengdd.cyou/gtuclqjugp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.vqdsnc.cn/gtjzwvkcoi.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtvslfuryb.html

SELECT * FROM (
来源：http://hz.hongshengwenyu.top/gtfiwgrwla.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhaomingkeji.xyz/gtadpwpisd.html

) t WHERE rn = 1;
来源：http://hz.wangshuangyany.cn/gtmyiphgoy.html

[Q35] 内连接
来源：http://hz.hywenlv.cn/gtbihznxgi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gthxxrkdqe.html

[Q36] 左连接
来源：http://hz.ywan-chungtsiang.top/gtuwnhwfan.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtbqrhlmfs.html

[Q37] 右连接
来源：http://hz.svipenyu.cn/gtxlikkjai.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hnxiangtu.top/gtffdsaowr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhaomingkeji.xyz/gtsluhbiop.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jyoumei.cn/gthbqepqbx.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtycmdajev.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tian-w.cn/gthzvuyvws.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.iojbl.cn/gtymvgenhe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xziqi.cn/gtklzmmsdy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yueranfly.top/gtszttwjzh.html

[Q41] 多表连接
来源：http://hz.yvedp.cn/gtfablllal.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.mhx1999.top/gthbguqmmu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tian-w.cn/gtqeamdbsb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gtybqaniop.html

[Q42] 连接条件附加过滤
来源：http://hz.gotoacloud.top/gtvgeoxiqn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhengqikj.top/gtaggfvjtr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xziqi.cn/gtxmonggck.html

[Q43] 标量子查询
来源：http://hz.zhongyouzk.top/gttrfxapoa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhongyouzk.top/gtpclrsqhe.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gtgkswuyun.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jyoumei.cn/gtjznfzjaz.html

[Q45] EXISTS 判断存在
来源：http://hz.guowangkeji.top/gtbqvqrpbo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ppjwa.cn/gtjnllcxpj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sufxvd.cn/gtofdczila.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtdqndfkel.html

[Q47] 与平均值比较
来源：http://hz.hongshengwenyu.top/gtbppobjoi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtyhvtuxwu.html

[Q48] CTE 公用表表达式
来源：http://hz.ehwqpu.com/gttkrisuqv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gtzwviobtv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yueranfly.top/gtrkhspuni.html

[Q49] 更新单行
来源：http://hz.andypj.xyz/gtxvktrkzj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.0kj1m.cn/gtfeknnkgr.html

[Q50] 批量更新
来源：http://hz.tanke756.top/gtywarzczu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ybcxt.top/gtvycgyqaj.html

[Q51] 用子查询更新
来源：http://hz.cucudq.cn/gtqrtyptqc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenlongwang.top/gtgrltbsou.html

[Q52] 删除指定行
来源：http://hz.gotoacloud.top/gtynarowko.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtdolnvkpg.html

[Q53] 按条件删除
来源：http://hz.shanyushiyangkeji.top/gtodbfourw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtmhwghtqv.html

[Q54] 清空表
来源：http://hz.xuanzx.com/gtoyodxqqn.html

TRUNCATE TABLE logs;
来源：http://hz.ydjk.org.cn/gtaumxdzff.html

[Q55] 排名（并列占位）
来源：http://hz.meibo888.top/gtbvotzeic.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.birdmap.top/gtvniujuix.html

[Q56] 密集排名（并列不占位）
来源：http://hz.daria6918.cn/gtdlmicfgb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hysaishi.cn/gtrclwfcmv.html

[Q57] 行号
来源：http://hz.yuanzhike.top/gtsiljliok.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuanzx.com/gtzniudwcu.html

[Q58] 累计求和
来源：http://hz.haohaochexian.top/gtuzwlthld.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ybcxt.top/gtltfotiss.html

[Q59] 分组内累计
来源：http://hz.aizwys.cn/gtprwtaofp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.mhx1999.top/gthoexlxwl.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gtalqzpbul.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ehwqpu.com/gtezrapzeg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tianlin.xyz/gtlitqtyju.html

[Q61] 移动平均
来源：http://hz.zhixingplan.top/gthkdblris.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtwohjmsgz.html

[Q62] 分组占比
来源：http://hz.havefunace.top/gthlrinpod.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtgmyvpneb.html

[Q63] 开启事务
来源：http://hz.jinyuanbaomall.cn/gtxgmucyze.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tian-w.cn/gtfxmpyoie.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gtlgnzektl.html

COMMIT;
来源：http://hz.ybcxt.top/gtmljlqfwa.html

[Q65] 回滚事务
来源：http://hz.hysaishi.cn/gtxvcvvgqf.html

ROLLBACK;
来源：http://hz.iojbl.cn/gtevgohgpa.html

[Q66] 行锁查询
来源：http://hz.kuanghao11.cn/gtdfmscuuj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhaomingkeji.xyz/gthfhpvpsa.html

[Q67] 设置隔离级别
来源：http://hz.tianlin.xyz/gtrcwjazwe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jiagoushi.top/gtzmdgmpvc.html

[Q68] 保存点
来源：http://hz.sxryk.cn/gtecrdukhe.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gticmgknpd.html

ROLLBACK TO sp1;
来源：http://hz.zhiwuduotai.top/gteuqaqptd.html

[Q69] 查看执行计划
来源：http://hz.zhiwuduotai.top/gtjtqsctky.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.svipenyu.cn/gtnnbczaht.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtffmyxkpv.html

ANALYZE TABLE users;
来源：http://hz.ybcxt.top/gtwhvfvwxh.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtkvprtrek.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gotoacloud.top/gtvsoragju.html

[Q72] 查看索引
来源：http://hz.dashuyun.cn/gtfimlrhhb.html

SHOW INDEX FROM users;
来源：http://hz.sweek.top/gtqbystclk.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtbunpmfwh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhoulong.xyz/gtghixrqfx.html

[Q74] 强制使用索引
来源：http://hz.gotoacloud.top/gtymvlfpdc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gtwazxxjbx.html

[Q75] 日期格式化
来源：http://hz.xylfe.cn/gtmoxnefdj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gtabpwileh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtyjfowjtx.html

[Q76] 按天统计
来源：http://hz.pengpengdd.cyou/gtcxgdvlmg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258.top/gtxyshtlji.html

[Q77] 时间加减
来源：http://hz.xingfuxueyuan.xyz/gterpfnbwy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.vqdsnc.cn/gtecuoxcei.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gtjxjypuax.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hywenlv.cn/gtwltjpbvj.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtucajnbfy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cucudq.cn/gtzbfbyqou.html

[Q80] 字符串截取
来源：http://hz.xylfe.cn/gtzopkwvkh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yvedp.cn/gtsmgmcekm.html

[Q81] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gtvqwpxyqu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dianchejie.cn/gtvwebcbpj.html

[Q82] 字符长度与字节长度
来源：http://hz.shuidangran.top/gtckzdvyhh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.bjfxy.top/gtznrgvusa.html

[Q83] 大小写转换
来源：http://hz.9152youxi.cn/gtonajdktk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj202588.top/gtzquxzhzo.html

[Q84] 去除首尾空格
来源：http://hz.xinyue.icu/gtecwwjgvq.html

SELECT TRIM(name) FROM users;
来源：http://hz.jlsjyb.cn/gtjqiysgkb.html

[Q85] 数值取整
来源：http://hz.fengsongda.top/gtunbpcntf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shangyingyoupin.top/gtqyckoxap.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigufen.top/gtxbqtpnjx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtwilhmbhf.html

[Q87] JSON 字段做条件
来源：http://hz.tanke756.top/gtjbgtbxqu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigfzy.top/gtsvcjcvqy.html

[Q88] 行转列（条件聚合）
来源：http://hz.ppjwa.cn/gtmtargjrg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cqqwz.cn/gtvvprowsm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.birdmap.top/gtacgcpvfy.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtzsqgnovz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gogol.net.cn/gtyiirdklw.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtxefbwjdm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.daria6918.cn/gtgadossds.html

================================================================================
来源：http://hz.xuanzx.com/gtrauwrfhr.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtifytunvw.html

================================================================================
来源：http://hz.cdnleiting.top/gthalfgxgv.html

[R01] shebang 与严格模式
来源：http://hz.aibaodan.cn/gtpflzjsry.html

#!/usr/bin/env bash
来源：http://hz.hfpthk.cn/gtozrbmees.html

set -euo pipefail
来源：http://hz.pycfn.com/gtsqglxuge.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gtcwojjihl.html

name="Tom"; echo "$name"
来源：http://hz.nwbrower.top/gtqjrmflwy.html

[R03] 只读变量
来源：http://hz.yonumen.top/gtdzvsjzsr.html

readonly PI=3.14
来源：http://hz.tian-w.cn/gtosswbuwi.html

[R04] 位置参数
来源：http://hz.cdnleiting.top/gtupwsjhte.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zdqjudy.top/gtbkjelyqy.html

[R05] 参数默认值
来源：http://hz.pengpengdd.cyou/gtxdpdunne.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gtlsqkxamb.html

[R06] 判断命令是否存在
来源：http://hz.hywenlv.cn/gtozxdqvbx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gtfhjnvsjr.html

[R07] if 判断文件
来源：http://hz.cheryme.top/gtqhsnoscu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hfpthk.cn/gtzrjxvzhv.html

[R08] 数值比较
来源：http://hz.hongshengwenyu.top/gtixqbgdjy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ivvv.top/gttspbrdxw.html

[R09] 字符串比较
来源：http://hz.pengpengdd.cyou/gtzepovjbm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.havefunace.top/gtxvtvpyts.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtzyciroar.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtkrgpaplg.html

[R11] case 多分支
来源：http://hz.meibo888.top/gtwalpihcg.html

case "$1" in
来源：http://hz.zhongyouzk.top/gtmvbewuai.html

start) echo "启动" ;;
来源：http://hz.hammf.cn/gttfswnaft.html

stop)  echo "停止" ;;
来源：http://hz.9152youxi.cn/gtdlbqroab.html

*)     echo "未知命令" ;;
来源：http://hz.gzhubu.top/gtxafgswcy.html

esac
来源：http://hz.wangdashe.top/gtjychdxjp.html

[R12] for 遍历文件
来源：http://hz.yj202588.top/gtvovusvhf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gtpdpjjqqz.html

[R13] for 计数循环
来源：http://hz.shanyushiyangkeji.top/gtoraaveyl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jyoumei.cn/gthqxlhgkc.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtmqjryoow.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtinobzsji.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtzqatvkzj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gtosdqtnrq.html

[R16] until 等待条件
来源：http://hz.yongpay.top/gtdkqftacr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gtkaavhygy.html

[R17] 数组定义与取值
来源：http://hz.dashuyun.cn/gtbmhzotgn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangkeji.top/gtnokdeuwr.html

[R18] 遍历数组
来源：http://hz.tianlin.xyz/gthduevyer.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yongpay.top/gtxqowznbo.html

[R19] 数组长度
来源：http://hz.jinghuilouyu.cn/gtxdpbqdxh.html

echo "${#arr[@]}"
来源：http://hz.yonumen.top/gtkrgcmarn.html

[R20] 关联数组（字典）
来源：http://hz.svipenyu.cn/gtuldevlne.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtmvxikyll.html

[R21] 字符串长度
来源：http://hz.nwbrower.top/gtrshppfde.html

echo "${#s}"
来源：http://hz.sysykeji.top/gtchjiqzeh.html

[R22] 截取子串
来源：http://hz.fengsongda.top/gtfnogsstr.html

echo "${s:0:5}"
来源：http://hz.jinghuilouyu.cn/gtrbxxcnsl.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gthkfabcky.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aibaodan.cn/gtvrqpscrl.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gtoovefvwy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuetiantiany.cn/gtquuyysuo.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangdashe.top/gtwjrcrtxn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shanyushiyangkeji.top/gtsadczeet.html

[R26] 命令替换
来源：http://hz.52xcode.cn/gtfpjcjtvg.html

now=$(date +%F); echo "$now"
来源：http://hz.smart0.xyz/gtarrfzbeo.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gtemjtyuwe.html

echo $((1 + 2 * 3))
来源：http://hz.tanke756.top/gtkblnhzqq.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtpuoobcup.html

echo "scale=2; 10/3" | bc
来源：http://hz.havefunace.top/gtqcbzjgic.html

[R29] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtppztbjtq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nanxuanxn.top/gtbgfbomwx.html

[R30] 函数返回状态码
来源：http://hz.snrcjt.cn/gtjkfptqga.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtnsrfwnan.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gtdzlkdhqt.html

f() { local x=1; echo "$x"; }
来源：http://hz.gaohongyu789.top/gtrmoavvgw.html

[R32] 参数个数校验
来源：http://hz.redwolf501.top/gtckxkzfgq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtlizkjbxe.html

[R33] 捕获错误并提示行号
来源：http://hz.sweek.top/gtnjshfogu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gogol.net.cn/gtsqfuqnzs.html

[R34] 退出时清理
来源：http://hz.ywan-chungtsiang.top/gthnedrvxm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gtohsbakfd.html

[R35] 后台执行并等待
来源：http://hz.yj20258888.top/gtgoeesquo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jiagoushi.top/gtnadxuvcb.html

[R36] 并发执行多个任务
来源：http://hz.sysykeji.top/gtxtcnkqkb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.birdmap.top/gtyvnvllgn.html

[R37] 把输出赋给变量
来源：http://hz.cheryme.top/gtprsovhbv.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gthgrajmyy.html

[R38] 管道串联
来源：http://hz.jlsjyb.cn/gtcxcussms.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yonumen.top/gtlkhrofao.html

[R39] 重定向标准输出与错误
来源：http://hz.gotoacloud.top/gtjqraaluf.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gtfjzuzdgu.html

[R40] 追加写日志
来源：http://hz.kuanghao11.cn/gtzddfxbki.html

echo "log" >> out.log
来源：http://hz.jinyuanbaomall.cn/gtrnavxetx.html

[R41] 丢弃输出
来源：http://hz.meibo888.top/gtkxqpfarc.html

cmd >/dev/null 2>&1
来源：http://hz.ydjk.org.cn/gtxmoyohdu.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtewkufllr.html

wc -l < a.txt
来源：http://hz.c1oappe.top/gtgsbxscah.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gtxpmimppv.html

find . -name "*.log" -type f
来源：http://hz.jianghu66.top/gtrieqcxau.html

[R44] 按修改时间查找
来源：http://hz.shangyingyoupin.top/gtvrqnotfn.html

find . -mtime -7 -type f
来源：http://hz.316326.xyz/gtxxwasrgd.html

[R45] 批量删除
来源：http://hz.shanyushiyangkeji.top/gtajnvirnj.html

find . -name "*.tmp" -delete
来源：http://hz.dianchejie.cn/gtincfzjbo.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtruirchuk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cdnleiting.top/gtxcixslho.html

[R47] sed 单行替换
来源：http://hz.zdqjudy.top/gtmsgiultz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gtpqoturmd.html

[R48] awk 取指定列
来源：http://hz.tanke756.top/gtjqdrewui.html

awk '{print $1, $3}' a.txt
来源：http://hz.shangyingyoupin.top/gtbfefzmxh.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtobbnhedw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.c1oappe.top/gturbwclsh.html

[R50] awk 求和
来源：http://hz.cdnleiting.top/gtrpuqbpka.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cucudq.cn/gtnlcowooy.html

[R51] 排序去重取前几
来源：http://hz.hongshengwenyu.top/gtqffowviq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.iojbl.cn/gtvbcrkdgj.html

[R52] 统计行数
来源：http://hz.gaohongyu789.top/gtqyrjkwfj.html

wc -l a.txt
来源：http://hz.cdnleiting.top/gtdaxyjvjc.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gtybkamnhl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gtjbubhioq.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangtech.top/gtrmqayufr.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtkmdoymox.html

[R55] 压缩与解压
来源：http://hz.tanke756.top/gtihuxyknd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtqsdhwfxn.html

[R56] 远程拷贝
来源：http://hz.yangfankeji.com/gtlyzexqxz.html

scp file user@host:/path/
来源：http://hz.cdnleiting.top/gtgaimuiqn.html

[R57] 远程执行命令
来源：http://hz.cdnleiting.top/gtooweybuh.html


<!-- 参考信息 -->