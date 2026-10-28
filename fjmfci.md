代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.mhx1999.top/gtvcojusmd.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gthavbjtnn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenlongwang.top/gtjbzahpyz.html

[Q12] 插入后取自增 ID
来源：http://hz.hywenlv.cn/gtpejawreo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ybcxt.top/gtbjoylqcg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.bjfxy.top/gtxrnfnyxz.html

[Q13] 忽略重复插入
来源：http://hz.0kj1m.cn/gttbcdwefj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yanxiufei.cn/gtokwdffng.html

[Q14] 存在则更新（upsert）
来源：http://hz.xuetiantiany.cn/gthvlbiwiz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtkfjxrjau.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hfpthk.cn/gtzblehgen.html

[Q15] 查询全部
来源：http://hz.mhx1999.top/gtnlyqgpsu.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtsktgeltg.html

[Q16] 查询指定列
来源：http://hz.ybcxt.top/gtyjojdkfr.html

SELECT id, name FROM users;
来源：http://hz.daxiang520.top/gtbkypvpyv.html

[Q17] 条件查询
来源：http://hz.meibo888.top/gtozhtlujm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj20258888.top/gtyhfirwkm.html

[Q18] 模糊匹配
来源：http://hz.gaohongyu789.top/gtwbtqmpli.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtaoewaynv.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gtjlylxbtr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ehwqpu.com/gtseiljnon.html

[Q20] IN 列表
来源：http://hz.guannengcc.top/gtfefgvnnu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gaohongyu789.top/gtxkvlxeqw.html

[Q21] 空值判断
来源：http://hz.bjfxy.top/gttmpwjlmo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtzmqptghx.html

[Q22] 排序
来源：http://hz.hywenlv.cn/gtrsgpmcyd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.vqdsnc.cn/gtgwyyizyq.html

[Q23] 分页
来源：http://hz.chenzaomai.com/gteqhtdycw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cdnleiting.top/gtbsjkybdi.html

[Q24] 去重
来源：http://hz.jyoumei.cn/gtyqikdteo.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangdashe.top/gtoxgnnccf.html

[Q25] 只取前 N 条
来源：http://hz.xziqi.cn/gtroqyooru.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenjidiqi.icu/gtguwswsky.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtcfdwuhtd.html

SELECT COUNT(*) FROM users;
来源：http://hz.quarkkingdee.top/gtnssmgigl.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gtyevbsgzj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangtech.top/gtffrkqpgk.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtvsegyhok.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yvedp.cn/gtdgachrxz.html

[Q29] 最大最小值
来源：http://hz.quarkkingdee.top/gtvschvrlf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.mhx1999.top/gtienurlxl.html

[Q30] 分组统计
来源：http://hz.dianchejie.cn/gtyhdjhmst.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtuzhpsvyc.html

[Q31] 分组后过滤
来源：http://hz.sysykeji.top/gtmrshchen.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ywan-chungtsiang.top/gtwezwdrav.html

[Q32] 分组拼接字符串
来源：http://hz.c1oappe.top/gtgmavnarn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.nanxinkj.top/gtcnbvmerk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinyuanbaomall.cn/gtipeqvnvc.html

[Q33] 多列分组
来源：http://hz.ppjwa.cn/gtptidoocc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.wangdashe.top/gtqzfljets.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtdrtxscpj.html

SELECT * FROM (
来源：http://hz.jinghuilouyu.cn/gtkgaevcjg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jiagoushi.top/gtenktqdco.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtyzbiczhj.html

[Q35] 内连接
来源：http://hz.xylfe.cn/gtzcrpwkan.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtevtzqetg.html

[Q36] 左连接
来源：http://hz.sufxvd.cn/gtdltshkgw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtwvrhjyzi.html

[Q37] 右连接
来源：http://hz.jianghu66.top/gtnzeaqztj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cucudq.cn/gtczgacito.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhengqikj.top/gtxmubssjf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangkeji.top/gtqextdebx.html

[Q39] 自连接（查上下级）
来源：http://hz.yj202588.top/gthrivjakv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pycfn.com/gtenuroaep.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shangyingyoupin.top/gtkrhewyza.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shzxlz.cn/gtvkdfgdzn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.vqdsnc.cn/gtybhpsemq.html

[Q41] 多表连接
来源：http://hz.pycfn.com/gtgabpqotg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hywenlv.cn/gtnoqnorvp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sxryk.cn/gtzebbkspx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ybcxt.top/gtcyzkuhpl.html

[Q42] 连接条件附加过滤
来源：http://hz.meibo888.top/gtocdojuht.html

SELECT u.name, o.amount FROM users u
来源：http://hz.feifeiyinyue.top/gtderhyugg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxinkj.top/gthkfztllt.html

[Q43] 标量子查询
来源：http://hz.shzxlz.cn/gtjadguzcr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangshuangyany.cn/gtyybrpiuk.html

[Q44] IN 子查询
来源：http://hz.redwolf501.top/gtdomuyavk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xingfuxueyuan.xyz/gtekertyqq.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtvlovcgmc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenjidiqi.icu/gtsyjefazi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hammf.cn/gtxihareek.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtgiealbtd.html

[Q47] 与平均值比较
来源：http://hz.cucudq.cn/gtwbypvurw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhongyouzk.top/gthotzlmxt.html

[Q48] CTE 公用表表达式
来源：http://hz.gotoacloud.top/gtjzucwmag.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigfzy.top/gtduonwutx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuetiantiany.cn/gtdwgcbtyq.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gttqldgiic.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtccmfaoul.html

[Q50] 批量更新
来源：http://hz.xuetiantiany.cn/gtibzgwwtw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ywan-chungtsiang.top/gtpoqovnne.html

[Q51] 用子查询更新
来源：http://hz.ivvv.top/gtwdfihzfh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydzc1.top/gtckkpjtcp.html

[Q52] 删除指定行
来源：http://hz.aizwys.cn/gtxwgmooag.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jiagoushi.top/gtwnqjmhky.html

[Q53] 按条件删除
来源：http://hz.sweek.top/gtvxxcgvxs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj20258888.top/gtbmjiiqfw.html

[Q54] 清空表
来源：http://hz.0kj1m.cn/gtecxiedpd.html

TRUNCATE TABLE logs;
来源：http://hz.fengsongda.top/gtpqlpooar.html

[Q55] 排名（并列占位）
来源：http://hz.c1oappe.top/gtkqazwasx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.iojbl.cn/gthkrkdwyx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtakpzzojp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtfxnuunqw.html

[Q57] 行号
来源：http://hz.jiagoushi.top/gtayufsiwh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tianlin.xyz/gtcygjvonf.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gttzyijkjw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sufxvd.cn/gtjulilfhg.html

[Q59] 分组内累计
来源：http://hz.hywenlv.cn/gtfburohrh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhongyouzk.top/gtcbuxiomd.html

[Q60] 取上一行 / 下一行
来源：http://hz.daxiang520.top/gttfsudfml.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cashguo.top/gtodefzhkw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtrwipwxet.html

[Q61] 移动平均
来源：http://hz.haohaochexian.top/gtwiaevfcb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.snrcjt.cn/gtnkmwnfyh.html

[Q62] 分组占比
来源：http://hz.c1oappe.top/gtdjggpavg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtbqcptopj.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtgtrosnap.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhiwuduotai.top/gtyytapuut.html

[Q64] 提交事务
来源：http://hz.cdnleiting.top/gtctvllkix.html

COMMIT;
来源：http://hz.hammf.cn/gtllzyerkk.html

[Q65] 回滚事务
来源：http://hz.jqgufenzy.top/gtxbokpucz.html

ROLLBACK;
来源：http://hz.vqdsnc.cn/gtmqgiuufv.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtvylinwbg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gtfcrvtsyg.html

[Q67] 设置隔离级别
来源：http://hz.nanxinkj.top/gtlaadqqqc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangkeji.top/gtdmiepnvl.html

[Q68] 保存点
来源：http://hz.tianlin.xyz/gthnsaubkt.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtahnfywdj.html

ROLLBACK TO sp1;
来源：http://hz.shzxlz.cn/gthlmibjcs.html

[Q69] 查看执行计划
来源：http://hz.cqqwz.cn/gtgdzqlfaj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sufxvd.cn/gtrqxjjafl.html

[Q70] 更新统计信息
来源：http://hz.zhoulong.xyz/gtqezstkoq.html

ANALYZE TABLE users;
来源：http://hz.gaohongyu789.top/gtvxzgzmqw.html

[Q71] 查看建表语句
来源：http://hz.hnqzz.top/gtgylrsiac.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hywenlv.cn/gtjjhjhahk.html

[Q72] 查看索引
来源：http://hz.zhoulong.xyz/gtepulttmt.html

SHOW INDEX FROM users;
来源：http://hz.nanxinkj.top/gtvzoeqomh.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangkeji.top/gtktgxyfhz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258888.top/gtfvzxnzkj.html

[Q74] 强制使用索引
来源：http://hz.cheryme.top/gtfhqpsafg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yongpay.top/gtgghsxnud.html

[Q75] 日期格式化
来源：http://hz.chenjidiqi.icu/gtwouzscgs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hywenlv.cn/gtlalztvka.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tanke756.top/gteanbmqnl.html

[Q76] 按天统计
来源：http://hz.sufxvd.cn/gtxdizjrbm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xinyue.icu/gtwplexzvr.html

[Q77] 时间加减
来源：http://hz.birdmap.top/gtcdgmkzpe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sxryk.cn/gtaxuqdgnj.html

[Q78] 当前时间
来源：http://hz.iojbl.cn/gtbzthklja.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cheryme.top/gtvtdugwdb.html

[Q79] 字符串拼接
来源：http://hz.aizwys.cn/gthnceshnx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.svipenyu.cn/gtreceiejh.html

[Q80] 字符串截取
来源：http://hz.yuxming.cn/gtnrzrxifr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yvedp.cn/gtuwyzywpw.html

[Q81] 字符串替换
来源：http://hz.jianghu66.top/gtssgooesy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenjidiqi.icu/gtahwinnkc.html

[Q82] 字符长度与字节长度
来源：http://hz.svipenyu.cn/gtcmvplzrj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtgntpaxal.html

[Q83] 大小写转换
来源：http://hz.sysykeji.top/gthltjuznz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gzhubu.top/gtmwipabpf.html

[Q84] 去除首尾空格
来源：http://hz.jqgfzy.top/gtmrdxgxpy.html

SELECT TRIM(name) FROM users;
来源：http://hz.xylfe.cn/gtybvffcuz.html

[Q85] 数值取整
来源：http://hz.hongshengwenyu.top/gtfjecenfi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xinyue.icu/gtkclprfbp.html

[Q86] 读取 JSON 字段
来源：http://hz.svipenyu.cn/gttvvgbotq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yongpay.top/gtktflhseg.html

[Q87] JSON 字段做条件
来源：http://hz.haohaochexian.top/gtkgsjbphb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pengpengdd.cyou/gtsnmntcmt.html

[Q88] 行转列（条件聚合）
来源：http://hz.dashuyun.cn/gtwhxkwcdt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gttdygsvri.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtadlngwej.html

[Q89] 判断表是否存在
来源：http://hz.ydjk.org.cn/gtxjfwkzbj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gtlfzuenxt.html

[Q90] 生成序号列
来源：http://hz.jqgfzy.top/gtfqydcewu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fzhhl.top/gtajdivcsa.html

================================================================================
来源：http://hz.cucudq.cn/gtkzraxpss.html

R. Bash 专题
来源：http://hz.hammf.cn/gtxvzjwggb.html

================================================================================
来源：http://hz.pycfn.com/gtrrwbrkxd.html

[R01] shebang 与严格模式
来源：http://hz.yuxming.cn/gthyacggwz.html

#!/usr/bin/env bash
来源：http://hz.jinqigufen.top/gtiytjnsdp.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtfackggdu.html

[R02] 变量赋值与使用
来源：http://hz.ehwqpu.com/gtoewphsux.html

name="Tom"; echo "$name"
来源：http://hz.zdqjudy.top/gtmcyprfnx.html

[R03] 只读变量
来源：http://hz.mhx1999.top/gtrjmkgikl.html

readonly PI=3.14
来源：http://hz.zdqjudy.top/gtltpbsdbh.html

[R04] 位置参数
来源：http://hz.yuanzhike.top/gtyiqatqge.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258888.top/gtulxxfghv.html

[R05] 参数默认值
来源：http://hz.daria6918.cn/gtnepqqioj.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gthitfxgbv.html

[R06] 判断命令是否存在
来源：http://hz.jinqigfzy.top/gtdacldmyx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtgvlffffn.html

[R07] if 判断文件
来源：http://hz.cheryme.top/gtuptsgupk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxuanxn.top/gtsavbejzc.html

[R08] 数值比较
来源：http://hz.andypj.xyz/gtbfikmtst.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sysykeji.top/gtquxzpqzw.html

[R09] 字符串比较
来源：http://hz.cucudq.cn/gtsxxamzhu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tanke756.top/gtcpkiwgim.html

[R10] 正则匹配
来源：http://hz.cdnleiting.top/gtunzwuxwj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ivvv.top/gtfykfhmkp.html

[R11] case 多分支
来源：http://hz.jqgufenzy.top/gtakvntwhk.html

case "$1" in
来源：http://hz.pycfn.com/gtalunirvi.html

start) echo "启动" ;;
来源：http://hz.shuidangran.top/gtpxctokzr.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gtnaezklrx.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gtonhkwzvz.html

esac
来源：http://hz.hnqzz.top/gtdispjirc.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangkeji.top/gtnlqqwxlk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.haohaochexian.top/gtgqkjpnhi.html

[R13] for 计数循环
来源：http://hz.xuanzx.com/gtfarwrjxx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yueranfly.top/gtjtfqcvxm.html

[R14] C 风格 for
来源：http://hz.fzhhl.top/gtipzetfue.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtkbnyxopd.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtmvtrmnlc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuanzx.com/gtprualsmo.html

[R16] until 等待条件
来源：http://hz.cashguo.top/gtxvgszmgg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtqdtkhhcx.html

[R17] 数组定义与取值
来源：http://hz.hongshengwenyu.top/gtzuniqbik.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daria6918.cn/gtpiubuqwx.html

[R18] 遍历数组
来源：http://hz.zhengqikj.top/gtwuqnzsas.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gteafmnosu.html

[R19] 数组长度
来源：http://hz.yonumen.top/gtfxiwokdu.html

echo "${#arr[@]}"
来源：http://hz.ydjk.org.cn/gttbtfjplc.html

[R20] 关联数组（字典）
来源：http://hz.cheryme.top/gtfzbznmwx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.c1oappe.top/gtppdtzdid.html

[R21] 字符串长度
来源：http://hz.shanyushiyangtech.top/gtfntfafrj.html

echo "${#s}"
来源：http://hz.jinqigfzy.top/gtgkntyozo.html

[R22] 截取子串
来源：http://hz.sxryk.cn/gtuvnzfkcc.html

echo "${s:0:5}"
来源：http://hz.svipenyu.cn/gtiflzmloi.html

[R23] 字符串替换
来源：http://hz.xinyue.icu/gttewvdjoy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daria6918.cn/gthhfqtnro.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtwddjykvo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.havefunace.top/gtelrxlagv.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtjohyzjlw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zycfv.cn/gtlcwtljac.html

[R26] 命令替换
来源：http://hz.yvedp.cn/gtrlftvwxr.html

now=$(date +%F); echo "$now"
来源：http://hz.gogol.net.cn/gtiihattvh.html

[R27] 算术展开
来源：http://hz.cashguo.top/gtjeebxrgb.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangtech.top/gtbgcifhsx.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gtnapzfykt.html

echo "scale=2; 10/3" | bc
来源：http://hz.redwolf501.top/gttrgzcfiv.html

[R29] 定义函数
来源：http://hz.wangdashe.top/gtxosiymab.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nanxuanxn.top/gtbxdktuuz.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangkeji.top/gtjcjvolnm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.redwolf501.top/gteumpgias.html

[R31] 局部变量
来源：http://hz.aibaodan.cn/gtwnvaadjv.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnqzz.top/gtrqqhxgoi.html

[R32] 参数个数校验
来源：http://hz.sufxvd.cn/gtuhnjyyqs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gthyufhuqq.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgufenzy.top/gtiqdnzlho.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhiwuduotai.top/gtnawlpwoh.html

[R34] 退出时清理
来源：http://hz.tian-w.cn/gtmzhcgnrc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gtwgvxbgic.html

[R35] 后台执行并等待
来源：http://hz.cheryme.top/gtpgpoucbf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.meibo888.top/gtshkxbkuz.html

[R36] 并发执行多个任务
来源：http://hz.nwbrower.top/gtckjygqce.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pengpengdd.cyou/gtbjjlucmk.html

[R37] 把输出赋给变量
来源：http://hz.jiagoushi.top/gtkssnrlwb.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtjlqvrafs.html

[R38] 管道串联
来源：http://hz.yj20258888.top/gtqisccsad.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aizwys.cn/gtgbxflqom.html

[R39] 重定向标准输出与错误
来源：http://hz.xingfuxueyuan.xyz/gtxjsgbaat.html

cmd > out.log 2>&1
来源：http://hz.nwbrower.top/gtbogqfmwr.html

[R40] 追加写日志
来源：http://hz.c1oappe.top/gtsroathbm.html

echo "log" >> out.log
来源：http://hz.jinqigufen.top/gtyxwmsrfm.html

[R41] 丢弃输出
来源：http://hz.yangfankeji.com/gtbfctgght.html

cmd >/dev/null 2>&1
来源：http://hz.9152youxi.cn/gtolhtvaqq.html

[R42] 输入重定向
来源：http://hz.tianlin.xyz/gtcslsnsya.html

wc -l < a.txt
来源：http://hz.nanxinkj.top/gtbzylezok.html

[R43] 按名字查找文件
来源：http://hz.wangdashe.top/gtpwpgygfh.html

find . -name "*.log" -type f
来源：http://hz.shuidangran.top/gtymymnnzr.html

[R44] 按修改时间查找
来源：http://hz.fengsongda.top/gthhysjjnw.html

find . -mtime -7 -type f
来源：http://hz.feifeiyinyue.top/gtrknfsxih.html

[R45] 批量删除
来源：http://hz.sweek.top/gtuypyomwn.html

find . -name "*.tmp" -delete
来源：http://hz.pengpengdd.cyou/gtjtamouil.html

[R46] 递归替换文件内容
来源：http://hz.smart0.xyz/gtfuuoepuo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.vqdsnc.cn/gtjqagplra.html

[R47] sed 单行替换
来源：http://hz.cqqwz.cn/gtfcqwpfwc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.vqdsnc.cn/gtrdzklaiu.html

[R48] awk 取指定列
来源：http://hz.sysykeji.top/gtdlizctda.html

awk '{print $1, $3}' a.txt
来源：http://hz.haohaochexian.top/gtquhsioxs.html

[R49] awk 带条件
来源：http://hz.0kj1m.cn/gtqqppoapx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydzc1.top/gtxyfqwksy.html

[R50] awk 求和
来源：http://hz.xuetiantiany.cn/gtpwduozcg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cucudq.cn/gtxnjnvqzg.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtykzldkec.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.c1oappe.top/gtrhkzcrta.html

[R52] 统计行数
来源：http://hz.aibaodan.cn/gtyricujua.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtojvipssf.html

[R53] 查看文件头与实时尾
来源：http://hz.316326.xyz/gthkwbbrju.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.kuanghao11.cn/gtrusrtudw.html

[R54] 比较两个文件
来源：http://hz.fzhhl.top/gtypzkgwbu.html

diff a.txt b.txt
来源：http://hz.sysykeji.top/gtifkspwvh.html

[R55] 压缩与解压
来源：http://hz.sufxvd.cn/gtgpvtbewx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tanke756.top/gtccwmfxjv.html

[R56] 远程拷贝
来源：http://hz.pycfn.com/gtaliqkmca.html

scp file user@host:/path/
来源：http://hz.chenlongwang.top/gtzrqmfdjp.html

[R57] 远程执行命令
来源：http://hz.snrcjt.cn/gtqyggweao.html

ssh user@host 'uptime'
来源：http://hz.hongshengwenyu.top/gtpsexauze.html

[R58] 下载文件
来源：http://hz.quarkkingdee.top/gtolvzjuoh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.snrcjt.cn/gtcwnahwjp.html

[R59] 发 POST JSON
来源：http://hz.yuanzhike.top/gtqqfhomtl.html


<!-- 参考信息 -->