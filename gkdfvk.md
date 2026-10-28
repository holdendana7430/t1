代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xylfe.cn/gtprzfpknd.html

[Q09] 创建唯一索引
来源：http://hz.tianlin.xyz/gtojyzaaiq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtuqeybhxs.html

[Q10] 插入单行
来源：http://hz.nwbrower.top/gtrwtvlszg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yangfankeji.com/gtstxfumce.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gtissqxijc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydzc1.top/gtkrokzyqf.html

[Q12] 插入后取自增 ID
来源：http://hz.c1oappe.top/gtncmmaysl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ppjwa.cn/gtcibifnkx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jlsjyb.cn/gtaszcmywg.html

[Q13] 忽略重复插入
来源：http://hz.vqdsnc.cn/gtfupijnrs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ydjk.org.cn/gtfctwvaow.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhoulong.xyz/gtdrtjinus.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yuxming.cn/gtzyjsaedk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigfzy.top/gtqcrhcjbt.html

[Q15] 查询全部
来源：http://hz.jiagoushi.top/gtljpnridp.html

SELECT * FROM users;
来源：http://hz.fzhhl.top/gtjfxrbupw.html

[Q16] 查询指定列
来源：http://hz.cucudq.cn/gtknzlwxcy.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gttfqaqjrr.html

[Q17] 条件查询
来源：http://hz.ydjk.org.cn/gtdoyyxiqa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.bjfxy.top/gttxztigvc.html

[Q18] 模糊匹配
来源：http://hz.pycfn.com/gtdpmnasbp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258888.top/gtrmyuvuta.html

[Q19] 范围查询
来源：http://hz.shangyingyoupin.top/gteuvjelim.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ppjwa.cn/gtkwrmnluv.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtjhowmpor.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gthhvjmvhe.html

[Q21] 空值判断
来源：http://hz.vqdsnc.cn/gtevnverkh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gzhubu.top/gtnahtrbtf.html

[Q22] 排序
来源：http://hz.tanke756.top/gtnvnmzgzt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cucudq.cn/gtbxaflfrv.html

[Q23] 分页
来源：http://hz.haohaochexian.top/gtsdiykvyo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.vqdsnc.cn/gtkedfknmv.html

[Q24] 去重
来源：http://hz.shuidangran.top/gtqjdvicwd.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenjidiqi.icu/gtvdlajjqs.html

[Q25] 只取前 N 条
来源：http://hz.tian-w.cn/gtbiuryeos.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hysaishi.cn/gtferandsf.html

[Q26] 计数
来源：http://hz.jinyuanbaomall.cn/gtsgazedik.html

SELECT COUNT(*) FROM users;
来源：http://hz.fzhhl.top/gtbiqoatwf.html

[Q27] 条件计数
来源：http://hz.wangdashe.top/gtbilkqstz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtgrystcea.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtyvnpzckj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtryojoqrl.html

[Q29] 最大最小值
来源：http://hz.tanke756.top/gtwstzvivs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.guannengcc.top/gtdzbjpphd.html

[Q30] 分组统计
来源：http://hz.cashguo.top/gtufrvskfj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtfrzxbkqq.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtzsnjafji.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hfpthk.cn/gtfgrajjut.html

[Q32] 分组拼接字符串
来源：http://hz.jiagoushi.top/gtmskyzzeh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtsmbyibah.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ivvv.top/gtfafgktqv.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtnyvlemai.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yvedp.cn/gtltaxswxq.html

[Q34] 每组取第一条
来源：http://hz.svipenyu.cn/gtkhzenaml.html

SELECT * FROM (
来源：http://hz.jinghuilouyu.cn/gtzzkhissu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhixingplan.top/gtqnyorpsw.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtkiscypaf.html

[Q35] 内连接
来源：http://hz.yuxming.cn/gtxvcgjdlt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtcyvbdunl.html

[Q36] 左连接
来源：http://hz.dashuyun.cn/gtbvfhrjca.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtsrgtrfmp.html

[Q37] 右连接
来源：http://hz.ydjk.org.cn/gtorrnngoi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ydjk.org.cn/gtgtycwavr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gtdrdnxjna.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ywan-chungtsiang.top/gtugxwrpsv.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigfzy.top/gtrzvkkmga.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenzaomai.com/gtffovinuh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gtusxpjhvq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fengsongda.top/gtzgisaubb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.aibaodan.cn/gtlzsmeycr.html

[Q41] 多表连接
来源：http://hz.cucudq.cn/gtskkwlvln.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daxiang520.top/gttkhrmbla.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gotoacloud.top/gtvukyyhyz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hammf.cn/gtyovpajrx.html

[Q42] 连接条件附加过滤
来源：http://hz.birdmap.top/gttmennpsn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtgzlzjhib.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gotoacloud.top/gtujozcxmo.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtjtcufeic.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gogol.net.cn/gtyiuhumeh.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gthirnljda.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.birdmap.top/gtppgmhiex.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtzimlwyue.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtdmzlllnf.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fengsongda.top/gtnxseumla.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtcinwbscx.html

[Q47] 与平均值比较
来源：http://hz.hammf.cn/gtqoojlreh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258.top/gtahaqpqpn.html

[Q48] CTE 公用表表达式
来源：http://hz.jianghu66.top/gttckuzvww.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhixingplan.top/gtzslwybyi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nanxinkj.top/gtjnipvdbd.html

[Q49] 更新单行
来源：http://hz.zdqjudy.top/gtbogoawui.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtwqheuwmq.html

[Q50] 批量更新
来源：http://hz.jlsjyb.cn/gtyacqywda.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtehmfhpes.html

[Q51] 用子查询更新
来源：http://hz.yongpay.top/gtwqkhyftw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtqydwrtrn.html

[Q52] 删除指定行
来源：http://hz.chenlongwang.top/gtfqjvfnic.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yvedp.cn/gthbfmmgun.html

[Q53] 按条件删除
来源：http://hz.yonumen.top/gtxrediirg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fzhhl.top/gtqvbwqpwg.html

[Q54] 清空表
来源：http://hz.jinghuilouyu.cn/gtopyxvxmx.html

TRUNCATE TABLE logs;
来源：http://hz.sweek.top/gthjpxxhyf.html

[Q55] 排名（并列占位）
来源：http://hz.dianchejie.cn/gtbkgontiy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tianlin.xyz/gtnsxbmqgq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zycfv.cn/gtnknjmqyz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yvedp.cn/gtdpvpevfa.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gtcoqgfflb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhixingplan.top/gtpgqnupyy.html

[Q58] 累计求和
来源：http://hz.gzhubu.top/gtctzlquio.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhijiandao.cn/gtiifdltwb.html

[Q59] 分组内累计
来源：http://hz.yanxiufei.cn/gtxfgrwrfc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jianghu66.top/gtibmyvvvc.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuetiantiany.cn/gtbrwhvunf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtacyfocpi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shuidangran.top/gtixgtkrfs.html

[Q61] 移动平均
来源：http://hz.sweek.top/gtlvqywkoc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinqigufen.top/gtyzzgvewx.html

[Q62] 分组占比
来源：http://hz.cqqwz.cn/gteamleupx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtlkhmflob.html

[Q63] 开启事务
来源：http://hz.jianghu66.top/gtrvxakmey.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhengqikj.top/gtyvrjylas.html

[Q64] 提交事务
来源：http://hz.sxryk.cn/gturphcjqb.html

COMMIT;
来源：http://hz.jyoumei.cn/gthiabdwup.html

[Q65] 回滚事务
来源：http://hz.yonumen.top/gtluegaijj.html

ROLLBACK;
来源：http://hz.iojbl.cn/gtgajjqosz.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gtbyfgvtun.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangshuangyany.cn/gtfatqqyud.html

[Q67] 设置隔离级别
来源：http://hz.shangyingyoupin.top/gtjarptnjk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yanxiufei.cn/gtcanvakie.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gthwyklucz.html

SAVEPOINT sp1;
来源：http://hz.pengpengdd.cyou/gtwpsehyjf.html

ROLLBACK TO sp1;
来源：http://hz.yuxming.cn/gtvkptqqez.html

[Q69] 查看执行计划
来源：http://hz.xuanzx.com/gtfoduboiy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.316326.xyz/gtjgapsecy.html

[Q70] 更新统计信息
来源：http://hz.ybcxt.top/gtendcanka.html

ANALYZE TABLE users;
来源：http://hz.yvedp.cn/gtbhzxcxop.html

[Q71] 查看建表语句
来源：http://hz.zhiwuduotai.top/gtnxjvwzyx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtgatoestu.html

[Q72] 查看索引
来源：http://hz.hongshengwenyu.top/gtrlfzmhud.html

SHOW INDEX FROM users;
来源：http://hz.daxiang520.top/gtwxyfhvll.html

[Q73] 查看表状态
来源：http://hz.ehwqpu.com/gtauwavmij.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guowangkeji.top/gtywcclexz.html

[Q74] 强制使用索引
来源：http://hz.zhiwuduotai.top/gtejmhnuds.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhaomingkeji.xyz/gtcazopzxp.html

[Q75] 日期格式化
来源：http://hz.gaohongyu789.top/gtutncncdg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pengpengdd.cyou/gtrxhjclfj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guowangkeji.top/gtvfipcstg.html

[Q76] 按天统计
来源：http://hz.gogol.net.cn/gtnrbklrwj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuxming.cn/gtgctrsmcr.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtqtuztumd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yonumen.top/gtlozukxhh.html

[Q78] 当前时间
来源：http://hz.dashuyun.cn/gtlwgouhjb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangtech.top/gtsnkucrnt.html

[Q79] 字符串拼接
来源：http://hz.kuanghao11.cn/gtlshailad.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ivvv.top/gtzclfuwbi.html

[Q80] 字符串截取
来源：http://hz.zycfv.cn/gtflmoyfoh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yangfankeji.com/gttlungvdj.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtetlnjpfy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtywnilwee.html

[Q82] 字符长度与字节长度
来源：http://hz.9152youxi.cn/gtesuvhrep.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtzjhqovyq.html

[Q83] 大小写转换
来源：http://hz.guowangkeji.top/gtkoxvkirt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hysaishi.cn/gturyicbro.html

[Q84] 去除首尾空格
来源：http://hz.sufxvd.cn/gtvuyaabgg.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhixingplan.top/gtcigtlmvy.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtxtxqksei.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydjk.org.cn/gtvqxpsggl.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxinkj.top/gtjxkkkvqd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuxming.cn/gtewgwfwcq.html

[Q87] JSON 字段做条件
来源：http://hz.jinyuanbaomall.cn/gtgssuhxgc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jyoumei.cn/gtqrekldgz.html

[Q88] 行转列（条件聚合）
来源：http://hz.52xcode.cn/gtuxgrktmm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yonumen.top/gttomnewyj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj20258888.top/gtidbfzlhh.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gtnotfhvvr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtjzhlkevx.html

[Q90] 生成序号列
来源：http://hz.aizwys.cn/gtdodrvqcs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhiwuduotai.top/gtelnlxeiw.html

================================================================================
来源：http://hz.havefunace.top/gtxsedgifo.html

R. Bash 专题
来源：http://hz.chenjidiqi.icu/gthaaeawon.html

================================================================================
来源：http://hz.yuxming.cn/gtxloisstk.html

[R01] shebang 与严格模式
来源：http://hz.yueranfly.top/gtwjjlahba.html

#!/usr/bin/env bash
来源：http://hz.gotoacloud.top/gtlvpmjjdk.html

set -euo pipefail
来源：http://hz.jinghuilouyu.cn/gthqplssui.html

[R02] 变量赋值与使用
来源：http://hz.dianchejie.cn/gtolycfxdm.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gtrguobgxq.html

[R03] 只读变量
来源：http://hz.haohaochexian.top/gtaqytrezr.html

readonly PI=3.14
来源：http://hz.sweek.top/gtslgizkfm.html

[R04] 位置参数
来源：http://hz.xuanzx.com/gtaovxqcxa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nanxuanxn.top/gtswyinyvl.html

[R05] 参数默认值
来源：http://hz.shanyushiyangkeji.top/gttubxvdnp.html

name="${1:-default}"
来源：http://hz.shangyingyoupin.top/gtthknxbvs.html

[R06] 判断命令是否存在
来源：http://hz.hongshengwenyu.top/gtrrzjarkb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nwbrower.top/gtqevioewk.html

[R07] if 判断文件
来源：http://hz.nanxuanxn.top/gtwngusznc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gogol.net.cn/gtiuwavkrp.html

[R08] 数值比较
来源：http://hz.vqdsnc.cn/gtpzuougix.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xingfuxueyuan.xyz/gtbgyfffab.html

[R09] 字符串比较
来源：http://hz.zycfv.cn/gtdgfsacqv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhengqikj.top/gtgkjbjbft.html

[R10] 正则匹配
来源：http://hz.pycfn.com/gtyyamczwv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtbbsfslty.html

[R11] case 多分支
来源：http://hz.nanxuanxn.top/gtnwflcsir.html

case "$1" in
来源：http://hz.meibo888.top/gtualalpkb.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gthcoafuzt.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangtech.top/gtbvyllctc.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gthvhunndf.html

esac
来源：http://hz.aizwys.cn/gthsnplttc.html

[R12] for 遍历文件
来源：http://hz.aibaodan.cn/gtghdzhxfl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.mhx1999.top/gtkhgusgzm.html

[R13] for 计数循环
来源：http://hz.316326.xyz/gteukdfcap.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yonumen.top/gtwuaplccp.html

[R14] C 风格 for
来源：http://hz.nanxuanxn.top/gtigfzxpex.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gtobbvhsus.html

[R15] while 逐行读文件
来源：http://hz.yanxiufei.cn/gtfbyjrrsz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenjidiqi.icu/gtvgydxdbt.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gtjqefrjpg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hammf.cn/gtlmyydkcp.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gttfsnzchj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shzxlz.cn/gtkbcxdhur.html

[R18] 遍历数组
来源：http://hz.zhixingplan.top/gtjfvjrquw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dianchejie.cn/gtihyelqse.html

[R19] 数组长度
来源：http://hz.mhx1999.top/gtjrmevkyd.html

echo "${#arr[@]}"
来源：http://hz.jqgfzy.top/gtycnpzfwc.html

[R20] 关联数组（字典）
来源：http://hz.ehwqpu.com/gtcdxodliu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aizwys.cn/gtpbktbtuj.html

[R21] 字符串长度
来源：http://hz.sufxvd.cn/gtbnyjqftu.html

echo "${#s}"
来源：http://hz.ywan-chungtsiang.top/gtnncazlee.html

[R22] 截取子串
来源：http://hz.shanyushiyangkeji.top/gtlusxgnmc.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtuuuxpiyu.html

[R23] 字符串替换
来源：http://hz.tianlin.xyz/gtsqtrsiiq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhixingplan.top/gtdrqkkici.html

[R24] 大小写转换
来源：http://hz.0kj1m.cn/gttcrlxdta.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daria6918.cn/gtuchnsyxo.html

[R25] 去后缀 / 去前缀
来源：http://hz.aizwys.cn/gttbfmnhdt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigfzy.top/gtqdwaapoy.html

[R26] 命令替换
来源：http://hz.aibaodan.cn/gthhnweehl.html

now=$(date +%F); echo "$now"
来源：http://hz.ywan-chungtsiang.top/gtebznjjzu.html

[R27] 算术展开
来源：http://hz.ydjk.org.cn/gtxbxuoelk.html

echo $((1 + 2 * 3))
来源：http://hz.gotoacloud.top/gttmrkjemq.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gtprwljbld.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenlongwang.top/gtlrgzcbde.html

[R29] 定义函数
来源：http://hz.ybcxt.top/gtrrpkgrsq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tianlin.xyz/gtypoyfqwq.html

[R30] 函数返回状态码
来源：http://hz.tian-w.cn/gtzlousmpw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.meibo888.top/gtohlggcad.html

[R31] 局部变量
来源：http://hz.gogol.net.cn/gtaylohoih.html

f() { local x=1; echo "$x"; }
来源：http://hz.yvedp.cn/gtrsmjzlrv.html

[R32] 参数个数校验
来源：http://hz.ywan-chungtsiang.top/gthfmepbkv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hfpthk.cn/gtskvwtoti.html

[R33] 捕获错误并提示行号
来源：http://hz.haohaochexian.top/gtcbfugvyz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.redwolf501.top/gtamsbagyh.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gtwpqrhisn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtrshnnrhs.html

[R35] 后台执行并等待
来源：http://hz.zhiwuduotai.top/gtnujimwmk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zycfv.cn/gtvfpuejxq.html

[R36] 并发执行多个任务
来源：http://hz.pycfn.com/gtrrbczbjq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinghuilouyu.cn/gtaebbvzwq.html

[R37] 把输出赋给变量
来源：http://hz.mhx1999.top/gthnhbygat.html

files=$(ls -1)
来源：http://hz.ydjk.org.cn/gtuxytmgco.html

[R38] 管道串联
来源：http://hz.xinyue.icu/gtvgxpudxp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shanyushiyangkeji.top/gttyvsckan.html

[R39] 重定向标准输出与错误
来源：http://hz.ydjk.org.cn/gtdbxnsttx.html

cmd > out.log 2>&1
来源：http://hz.sweek.top/gtrxauznrb.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtfxfifaor.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gtjyrrachk.html

[R41] 丢弃输出
来源：http://hz.haohaochexian.top/gtjephblgi.html

cmd >/dev/null 2>&1
来源：http://hz.svipenyu.cn/gtjqqymtrb.html

[R42] 输入重定向
来源：http://hz.0kj1m.cn/gtnxxkqjxf.html

wc -l < a.txt
来源：http://hz.andypj.xyz/gtkjcsjmnx.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtzziapdpw.html

find . -name "*.log" -type f
来源：http://hz.yj20258.top/gtbtiakewy.html

[R44] 按修改时间查找
来源：http://hz.yonumen.top/gtlzflwegz.html

find . -mtime -7 -type f
来源：http://hz.jyoumei.cn/gtonauqykm.html

[R45] 批量删除
来源：http://hz.xziqi.cn/gtjigbghws.html

find . -name "*.tmp" -delete
来源：http://hz.jqgufenzy.top/gtlnqwfymk.html

[R46] 递归替换文件内容
来源：http://hz.nwbrower.top/gtppemxaak.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.iojbl.cn/gtgzxnpltq.html

[R47] sed 单行替换
来源：http://hz.wangshuangyany.cn/gtmkuvtxff.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtsmoehknx.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtjrsljjbs.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgfzy.top/gtgxvqafnp.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gthujubynv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj202588.top/gtrdoqdnev.html

[R50] awk 求和
来源：http://hz.hysaishi.cn/gtmoowwfoi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xziqi.cn/gtlohghznc.html

[R51] 排序去重取前几
来源：http://hz.fengsongda.top/gtfxhpxbsx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgufenzy.top/gtuohubikp.html

[R52] 统计行数
来源：http://hz.cucudq.cn/gtrndznkhv.html

wc -l a.txt
来源：http://hz.chenzaomai.com/gtpkoltrxs.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtsjtfelmz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sufxvd.cn/gtysnbcyel.html

[R54] 比较两个文件
来源：http://hz.c1oappe.top/gtuujkmupf.html

diff a.txt b.txt
来源：http://hz.ehwqpu.com/gterkggizf.html

[R55] 压缩与解压
来源：http://hz.sufxvd.cn/gtcmohzdss.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.9152youxi.cn/gtjdqxnlbd.html

[R56] 远程拷贝
来源：http://hz.tian-w.cn/gtapsnfewb.html

scp file user@host:/path/
来源：http://hz.zhongyouzk.top/gtqsfenpua.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtjtrbgccj.html


<!-- 参考信息 -->