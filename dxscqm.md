代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258.top/gtkovbfcwm.html

[Q11] 一次插入多行
来源：http://hz.jlsjyb.cn/gtidcdakwf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ppjwa.cn/gtsrhcmtim.html

[Q12] 插入后取自增 ID
来源：http://hz.cdnleiting.top/gtoywijouv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zycfv.cn/gtqkyeccln.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.havefunace.top/gtzobaazfh.html

[Q13] 忽略重复插入
来源：http://hz.9152youxi.cn/gtjwalhnig.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenlongwang.top/gthybafayi.html

[Q14] 存在则更新（upsert）
来源：http://hz.havefunace.top/gtsmxmtnck.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jlsjyb.cn/gtgrlphwty.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigufen.top/gtsptfsvqv.html

[Q15] 查询全部
来源：http://hz.havefunace.top/gttljzcszr.html

SELECT * FROM users;
来源：http://hz.ehwqpu.com/gtcoqqxdwx.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangkeji.top/gtzodwbaar.html

SELECT id, name FROM users;
来源：http://hz.tanke756.top/gtvkjpqzzs.html

[Q17] 条件查询
来源：http://hz.jianghu66.top/gtfgpkhcpq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gtuindkbci.html

[Q18] 模糊匹配
来源：http://hz.ybcxt.top/gtlspvhbnj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.snrcjt.cn/gtlxqlmdoz.html

[Q19] 范围查询
来源：http://hz.ivvv.top/gtelcnbrfh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ppjwa.cn/gtegaftkha.html

[Q20] IN 列表
来源：http://hz.hywenlv.cn/gthqjhalqf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yvedp.cn/gtkyucdaoj.html

[Q21] 空值判断
来源：http://hz.shanyushiyangtech.top/gtyqpqbtml.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zdqjudy.top/gtrinycibx.html

[Q22] 排序
来源：http://hz.0kj1m.cn/gtvzbqegzh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guowangkeji.top/gtwswuguab.html

[Q23] 分页
来源：http://hz.guannengcc.top/gttmuaphwu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gaohongyu789.top/gtfkzkzdhn.html

[Q24] 去重
来源：http://hz.hnqzz.top/gtlhtobhea.html

SELECT DISTINCT city FROM users;
来源：http://hz.jyoumei.cn/gtwxbiwayg.html

[Q25] 只取前 N 条
来源：http://hz.cqqwz.cn/gtkxekkoxw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ivvv.top/gthlvhskck.html

[Q26] 计数
来源：http://hz.ydjk.org.cn/gtqlcihdph.html

SELECT COUNT(*) FROM users;
来源：http://hz.cheryme.top/gtnpbhpnsf.html

[Q27] 条件计数
来源：http://hz.aibaodan.cn/gttshlezsm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnxiangtu.top/gticeoekwf.html

[Q28] 求和与平均
来源：http://hz.gogol.net.cn/gtjkshzylg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nwbrower.top/gttnfxnvfh.html

[Q29] 最大最小值
来源：http://hz.dianchejie.cn/gtpxtcuipt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigufen.top/gtimgvpbaq.html

[Q30] 分组统计
来源：http://hz.52xcode.cn/gtpfmdqzys.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtlgqublmi.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gtfdoocxhm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhaomingkeji.xyz/gtosxxjhse.html

[Q32] 分组拼接字符串
来源：http://hz.yj20258.top/gteemjgpko.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtuvwzrxmf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gtnbkhoxxw.html

[Q33] 多列分组
来源：http://hz.ywan-chungtsiang.top/gtsgppghtv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.0kj1m.cn/gtpnrstvea.html

[Q34] 每组取第一条
来源：http://hz.aizwys.cn/gtsglzhixu.html

SELECT * FROM (
来源：http://hz.tian-w.cn/gtcqylxfkx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhaomingkeji.xyz/gtwtewwuma.html

) t WHERE rn = 1;
来源：http://hz.cashguo.top/gttarwlbjo.html

[Q35] 内连接
来源：http://hz.quarkkingdee.top/gttzblqfad.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtnlqazmbl.html

[Q36] 左连接
来源：http://hz.jqgfzy.top/gtvbgmqzwn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtdzabfyda.html

[Q37] 右连接
来源：http://hz.fzhhl.top/gtofxhyhsp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yangfankeji.com/gtlwobickj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cqqwz.cn/gtxkdwjxwt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtzryddyii.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigufen.top/gtcbyvbcit.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtwcumsqab.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jlsjyb.cn/gtxzhououd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhaomingkeji.xyz/gtlajfldbk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pengpengdd.cyou/gtpoitpoyn.html

[Q41] 多表连接
来源：http://hz.hfpthk.cn/gtjqgkzcpe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhongyouzk.top/gtatnejtsq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydzc1.top/gtnlvqkwin.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sweek.top/gtlegsnpbd.html

[Q42] 连接条件附加过滤
来源：http://hz.zdqjudy.top/gtvlnitdio.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258.top/gtszskyeqb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yonumen.top/gtmtnlmhho.html

[Q43] 标量子查询
来源：http://hz.ywan-chungtsiang.top/gtckxffpxs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj202588.top/gtdlrzeixc.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtnulqwcan.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yueranfly.top/gtqxwgnkkj.html

[Q45] EXISTS 判断存在
来源：http://hz.nwbrower.top/gtirlfavbu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtfyodosni.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhengqikj.top/gtepxgbmsh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fzhhl.top/gtjlgitoej.html

[Q47] 与平均值比较
来源：http://hz.haohaochexian.top/gtwkrrecgr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tanke756.top/gtypgqzyul.html

[Q48] CTE 公用表表达式
来源：http://hz.smart0.xyz/gtowbmbdux.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pycfn.com/gtsfirizto.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinyuanbaomall.cn/gtzhyasicv.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gttdwuqorl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ybcxt.top/gtjmgnwumd.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtbdwtzicp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ydjk.org.cn/gtzytyeoqv.html

[Q51] 用子查询更新
来源：http://hz.mhx1999.top/gtkrzeouzn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zdqjudy.top/gttgvafccx.html

[Q52] 删除指定行
来源：http://hz.jinqigfzy.top/gtatqcgbru.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtaaxagvol.html

[Q53] 按条件删除
来源：http://hz.jinghuilouyu.cn/gtngwphhoj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.meibo888.top/gtssggpgsv.html

[Q54] 清空表
来源：http://hz.ivvv.top/gtktnflyro.html

TRUNCATE TABLE logs;
来源：http://hz.feifeiyinyue.top/gtppyraxux.html

[Q55] 排名（并列占位）
来源：http://hz.hywenlv.cn/gtxcivnqkz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtrofvcgku.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ehwqpu.com/gtsyzzbmwz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenzaomai.com/gteeoqinjy.html

[Q57] 行号
来源：http://hz.sweek.top/gtpyppgawo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.birdmap.top/gtrvzaxpmk.html

[Q58] 累计求和
来源：http://hz.nwbrower.top/gtsynkbezj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtuvfhwctc.html

[Q59] 分组内累计
来源：http://hz.gotoacloud.top/gtifyjngzf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgfzy.top/gtweyfeili.html

[Q60] 取上一行 / 下一行
来源：http://hz.yangfankeji.com/gtjljanpqi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cqqwz.cn/gtsauoeqnl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhijiandao.cn/gtopvugvvw.html

[Q61] 移动平均
来源：http://hz.ehwqpu.com/gtxrzjhxsi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.iojbl.cn/gtzxjnpxri.html

[Q62] 分组占比
来源：http://hz.hywenlv.cn/gtqpqfxxoj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtdcerrqkn.html

[Q63] 开启事务
来源：http://hz.shuidangran.top/gtyqxcrvzn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258888.top/gtvonkjdep.html

[Q64] 提交事务
来源：http://hz.jyoumei.cn/gtlbnfeayu.html

COMMIT;
来源：http://hz.wangshuangyany.cn/gtkbalmdtn.html

[Q65] 回滚事务
来源：http://hz.zhiwuduotai.top/gtyjgbmzvb.html

ROLLBACK;
来源：http://hz.jinqigfzy.top/gtyonmlebz.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtezsqitmt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigfzy.top/gtoayhpncl.html

[Q67] 设置隔离级别
来源：http://hz.quarkkingdee.top/gtwwttiqtf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sysykeji.top/gtnxzfboai.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gtkjjjkkve.html

SAVEPOINT sp1;
来源：http://hz.sweek.top/gtsvdmgpoy.html

ROLLBACK TO sp1;
来源：http://hz.chenlongwang.top/gttpluzygr.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtmzdiioib.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hysaishi.cn/gtrxjabawb.html

[Q70] 更新统计信息
来源：http://hz.nwbrower.top/gtoosmijhm.html

ANALYZE TABLE users;
来源：http://hz.jqgufenzy.top/gtdswanhvo.html

[Q71] 查看建表语句
来源：http://hz.ydzc1.top/gtmpcnctrw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhijiandao.cn/gtqauimzfp.html

[Q72] 查看索引
来源：http://hz.haohaochexian.top/gtplkioaaz.html

SHOW INDEX FROM users;
来源：http://hz.tian-w.cn/gtqsjjgztm.html

[Q73] 查看表状态
来源：http://hz.316326.xyz/gtudeatmca.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtqmlqmuwl.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gtwbhndlne.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj202588.top/gtwwdnfkwu.html

[Q75] 日期格式化
来源：http://hz.yuxming.cn/gtwjjuydym.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ybcxt.top/gtbazampeu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gtwreoqouh.html

[Q76] 按天统计
来源：http://hz.tian-w.cn/gtvciklxwy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jqgfzy.top/gtaaxrjywm.html

[Q77] 时间加减
来源：http://hz.meibo888.top/gtofziedhy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hywenlv.cn/gtbojdblct.html

[Q78] 当前时间
来源：http://hz.dashuyun.cn/gtiybowtma.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xziqi.cn/gtkehmjxpy.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtmrterckz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangshuangyany.cn/gtmzabliyy.html

[Q80] 字符串截取
来源：http://hz.yangfankeji.com/gtsgifyybe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fzhhl.top/gtjjrhllry.html

[Q81] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtmtjojkbu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jianghu66.top/gtizmnghvz.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtlomfxvfb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gaohongyu789.top/gtrmfkliiw.html

[Q83] 大小写转换
来源：http://hz.sweek.top/gtjgvmzjlp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sufxvd.cn/gtwbdnarzp.html

[Q84] 去除首尾空格
来源：http://hz.havefunace.top/gtzdlparjd.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtzlvwxdzl.html

[Q85] 数值取整
来源：http://hz.zhaomingkeji.xyz/gthohtixtu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jyoumei.cn/gtpryjqfhs.html

[Q86] 读取 JSON 字段
来源：http://hz.guowangkeji.top/gtapnuneuu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gtgqabcobh.html

[Q87] JSON 字段做条件
来源：http://hz.sxryk.cn/gtgonevcod.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.iojbl.cn/gtzbfrxzqc.html

[Q88] 行转列（条件聚合）
来源：http://hz.316326.xyz/gtxzrhdkkr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pycfn.com/gtbjuvjhuj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shangyingyoupin.top/gtiimvnxhv.html

[Q89] 判断表是否存在
来源：http://hz.vqdsnc.cn/gtlbxscfpf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.svipenyu.cn/gtpyjylhxw.html

[Q90] 生成序号列
来源：http://hz.gogol.net.cn/gtytuubgzu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gterfcpgnr.html

================================================================================
来源：http://hz.jqgfzy.top/gtctscitza.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtxhfqkhuc.html

================================================================================
来源：http://hz.yj20258888.top/gtwakhpsvc.html

[R01] shebang 与严格模式
来源：http://hz.hnqzz.top/gtyhmwbshk.html

#!/usr/bin/env bash
来源：http://hz.yonumen.top/gtelqihuch.html

set -euo pipefail
来源：http://hz.pycfn.com/gtcvfflptz.html

[R02] 变量赋值与使用
来源：http://hz.wangdashe.top/gtfvpauojk.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtgaemkaye.html

[R03] 只读变量
来源：http://hz.smart0.xyz/gthuvqoeot.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtddvgmbiw.html

[R04] 位置参数
来源：http://hz.zhiwuduotai.top/gtogqvucrh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yanxiufei.cn/gthdclxylh.html

[R05] 参数默认值
来源：http://hz.wangshuangyany.cn/gtsabgneol.html

name="${1:-default}"
来源：http://hz.shanyushiyangkeji.top/gtczzbfhan.html

[R06] 判断命令是否存在
来源：http://hz.birdmap.top/gtjyvbqfux.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ehwqpu.com/gtgirnzjup.html

[R07] if 判断文件
来源：http://hz.nanxinkj.top/gtavsjodxy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinghuilouyu.cn/gteakaaqch.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtjinvhjck.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tianlin.xyz/gtgqqlxpmf.html

[R09] 字符串比较
来源：http://hz.shuidangran.top/gteiopdgfk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yvedp.cn/gtovxuhgcw.html

[R10] 正则匹配
来源：http://hz.zhiwuduotai.top/gtqgindeut.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xylfe.cn/gtjljnigsf.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtwyznsuyo.html

case "$1" in
来源：http://hz.sufxvd.cn/gttsstsnft.html

start) echo "启动" ;;
来源：http://hz.smart0.xyz/gtkoxbywis.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtbdhmjcuy.html

*)     echo "未知命令" ;;
来源：http://hz.hammf.cn/gthfinhznw.html

esac
来源：http://hz.xziqi.cn/gtsrddccpo.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gtggndptly.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj202588.top/gtkinmzrow.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtvebtyays.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtlztibtjx.html

[R14] C 风格 for
来源：http://hz.gzhubu.top/gtjiusppuo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.52xcode.cn/gtjmtufadb.html

[R15] while 逐行读文件
来源：http://hz.yangfankeji.com/gtzdryjarm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yanxiufei.cn/gtizntngqz.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gtwvmrwryl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sysykeji.top/gtsyxqkpik.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gtqkvnrmaj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jianghu66.top/gtfqxadhnh.html

[R18] 遍历数组
来源：http://hz.yj202588.top/gtuubesopi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtbmmaxwwg.html

[R19] 数组长度
来源：http://hz.yj20258888.top/gtvomtltyd.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtzvbrdsgn.html

[R20] 关联数组（字典）
来源：http://hz.yj20258888.top/gtfzqizfdq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhengqikj.top/gtxktjmpgs.html

[R21] 字符串长度
来源：http://hz.feifeiyinyue.top/gtlimwdaid.html

echo "${#s}"
来源：http://hz.ywan-chungtsiang.top/gtbkpomqip.html

[R22] 截取子串
来源：http://hz.havefunace.top/gtcbhfcqzm.html

echo "${s:0:5}"
来源：http://hz.zhongyouzk.top/gtstjpzfrm.html

[R23] 字符串替换
来源：http://hz.xziqi.cn/gtlovqlvjq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gogol.net.cn/gtpcmsoicy.html

[R24] 大小写转换
来源：http://hz.redwolf501.top/gtepwpszfd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gogol.net.cn/gtamncnxjb.html

[R25] 去后缀 / 去前缀
来源：http://hz.yvedp.cn/gtuhyjnpfg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtnsecadpm.html

[R26] 命令替换
来源：http://hz.hammf.cn/gtqcufbvda.html

now=$(date +%F); echo "$now"
来源：http://hz.shzxlz.cn/gtwaxrkbxl.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtoyawncai.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtpgmuqdnk.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gthuwjtorh.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinqigfzy.top/gtkykzclxy.html

[R29] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtultwbwzw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cheryme.top/gtxfjpqnmp.html

[R30] 函数返回状态码
来源：http://hz.jinqigfzy.top/gttecroypv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shanyushiyangtech.top/gthjtaitri.html

[R31] 局部变量
来源：http://hz.shuidangran.top/gtlfvovaks.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenjidiqi.icu/gtbmsjhcgl.html

[R32] 参数个数校验
来源：http://hz.shuidangran.top/gtovwmzavp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nwbrower.top/gtsobnbnfo.html

[R33] 捕获错误并提示行号
来源：http://hz.yvedp.cn/gtcmddvyky.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.fzhhl.top/gtsfdmnmhg.html

[R34] 退出时清理
来源：http://hz.pengpengdd.cyou/gtbxogpgbq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtilgnlsna.html

[R35] 后台执行并等待
来源：http://hz.cashguo.top/gtapgpduzg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.daxiang520.top/gtkllognjw.html

[R36] 并发执行多个任务
来源：http://hz.hysaishi.cn/gtxovowteu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shuidangran.top/gtedagyonl.html

[R37] 把输出赋给变量
来源：http://hz.xuetiantiany.cn/gtpkkcpizj.html

files=$(ls -1)
来源：http://hz.pycfn.com/gtluienwbv.html

[R38] 管道串联
来源：http://hz.jqgfzy.top/gtxgqlugwc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ppjwa.cn/gtfxwxhvsv.html

[R39] 重定向标准输出与错误
来源：http://hz.zhaomingkeji.xyz/gtomwkofzf.html

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gtnpqhwmne.html

[R40] 追加写日志
来源：http://hz.jinyuanbaomall.cn/gtctfddwmi.html

echo "log" >> out.log
来源：http://hz.yj202588.top/gtrggtaqlo.html

[R41] 丢弃输出
来源：http://hz.tian-w.cn/gttdeixbwi.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtqspnxqml.html

[R42] 输入重定向
来源：http://hz.cdnleiting.top/gtozznteou.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gteevkwrex.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtmhdzbprr.html

find . -name "*.log" -type f
来源：http://hz.guannengcc.top/gtfppqunvt.html

[R44] 按修改时间查找
来源：http://hz.bjfxy.top/gtiggemyxo.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtdmizghzb.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtuvtlmdlz.html

find . -name "*.tmp" -delete
来源：http://hz.havefunace.top/gtxxkdpwzm.html

[R46] 递归替换文件内容
来源：http://hz.mhx1999.top/gtvnfvpeju.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zdqjudy.top/gtyzryttcp.html

[R47] sed 单行替换
来源：http://hz.zhongyouzk.top/gttzhcmojw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shangyingyoupin.top/gtsfjqxika.html

[R48] awk 取指定列
来源：http://hz.hnqzz.top/gtrcycxhcg.html

awk '{print $1, $3}' a.txt
来源：http://hz.ybcxt.top/gtknrgpfws.html

[R49] awk 带条件
来源：http://hz.yuxming.cn/gtqedovhxd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxinkj.top/gtviewojnw.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gtubcupjxu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ppjwa.cn/gttnvrqmcr.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtffhoiehm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangkeji.top/gtukkgqyet.html

[R52] 统计行数
来源：http://hz.shzxlz.cn/gttbggdxlb.html

wc -l a.txt
来源：http://hz.ywan-chungtsiang.top/gtfxtjlwpp.html

[R53] 查看文件头与实时尾
来源：http://hz.yvedp.cn/gtozgzoxbr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cdnleiting.top/gtsflgmgmm.html

[R54] 比较两个文件
来源：http://hz.52xcode.cn/gtapvmbnku.html

diff a.txt b.txt
来源：http://hz.yj20258888.top/gtcoqbowcy.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtbagkpnfw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ybcxt.top/gtzwkjpytb.html

[R56] 远程拷贝
来源：http://hz.xuanzx.com/gtugrbllsb.html

scp file user@host:/path/
来源：http://hz.chenzaomai.com/gthoefwesg.html

[R57] 远程执行命令
来源：http://hz.nwbrower.top/gtbspyllge.html

ssh user@host 'uptime'
来源：http://hz.mhx1999.top/gtkuilsclg.html

[R58] 下载文件
来源：http://hz.ywan-chungtsiang.top/gtxloazcfv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guannengcc.top/gtbaryqspx.html

[R59] 发 POST JSON
来源：http://hz.aibaodan.cn/gtacxbsttd.html


<!-- 参考信息 -->