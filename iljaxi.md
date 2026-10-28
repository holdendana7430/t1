代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ehwqpu.com/gtpjctjczu.html

[Q11] 一次插入多行
来源：http://hz.wangshuangyany.cn/gtkdaslshb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cashguo.top/gtguvzmgux.html

[Q12] 插入后取自增 ID
来源：http://hz.zhijiandao.cn/gtlshoqcct.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gtbsqbezfn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xylfe.cn/gtqqtoyqmr.html

[Q13] 忽略重复插入
来源：http://hz.jqgfzy.top/gtjkhygsom.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cucudq.cn/gthwtlvblf.html

[Q14] 存在则更新（upsert）
来源：http://hz.jqgfzy.top/gtxnbayshn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangtech.top/gtrwstlolh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gtohrytbjb.html

[Q15] 查询全部
来源：http://hz.yanxiufei.cn/gtcaouzkti.html

SELECT * FROM users;
来源：http://hz.hywenlv.cn/gtwkytgasl.html

[Q16] 查询指定列
来源：http://hz.shangyingyoupin.top/gtbcphwnvk.html

SELECT id, name FROM users;
来源：http://hz.yonumen.top/gtihcuwhid.html

[Q17] 条件查询
来源：http://hz.gogol.net.cn/gtmowhuhte.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangshuangyany.cn/gttehrxqfj.html

[Q18] 模糊匹配
来源：http://hz.tanke756.top/gtyqxyxjyk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ppjwa.cn/gtopmzclnk.html

[Q19] 范围查询
来源：http://hz.svipenyu.cn/gtithmqgzm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gtttucpnmc.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtcbsurhcj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.aibaodan.cn/gtixjdhuly.html

[Q21] 空值判断
来源：http://hz.yanxiufei.cn/gtxyjoyxqc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yangfankeji.com/gtoozuloru.html

[Q22] 排序
来源：http://hz.pengpengdd.cyou/gtyrowqeno.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yueranfly.top/gtdagdgccu.html

[Q23] 分页
来源：http://hz.zycfv.cn/gtqrhsvokw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinghuilouyu.cn/gthaunpabv.html

[Q24] 去重
来源：http://hz.bjfxy.top/gtzpejmsho.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgufenzy.top/gtzxlbhnnf.html

[Q25] 只取前 N 条
来源：http://hz.316326.xyz/gtvbmcuojv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sufxvd.cn/gttfrwpvjc.html

[Q26] 计数
来源：http://hz.xingfuxueyuan.xyz/gtzgviqnmb.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj202588.top/gtvzxlxfyl.html

[Q27] 条件计数
来源：http://hz.sxryk.cn/gthdzpjvkt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtjtcixidv.html

[Q28] 求和与平均
来源：http://hz.iojbl.cn/gtmbpsuxlb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gtfwrwxsxf.html

[Q29] 最大最小值
来源：http://hz.nanxinkj.top/gtgngksexv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258888.top/gtnkqbpsyz.html

[Q30] 分组统计
来源：http://hz.daria6918.cn/gtwkabtpsf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gthhklwmqp.html

[Q31] 分组后过滤
来源：http://hz.hnqzz.top/gtqvhpcncx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangtech.top/gtjigibllz.html

[Q32] 分组拼接字符串
来源：http://hz.xylfe.cn/gtbrhwpgyr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtsfussjqo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigfzy.top/gthujitlli.html

[Q33] 多列分组
来源：http://hz.jinghuilouyu.cn/gtyrkyistv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yonumen.top/gtleimhouu.html

[Q34] 每组取第一条
来源：http://hz.jinqigfzy.top/gtdtwqyrlv.html

SELECT * FROM (
来源：http://hz.vqdsnc.cn/gtvcvukott.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xinyue.icu/gtihlvpgui.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtpmtnmhcu.html

[Q35] 内连接
来源：http://hz.cucudq.cn/gtewxrqsgn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.mhx1999.top/gtuxpacmyh.html

[Q36] 左连接
来源：http://hz.vqdsnc.cn/gtsrslqmbe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtnxkwcvka.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtyjvkjlcf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtktrmhnzr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jianghu66.top/gtcdnjvlfw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yangfankeji.com/gtiqfhxwvi.html

[Q39] 自连接（查上下级）
来源：http://hz.shangyingyoupin.top/gtbqkhthho.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cheryme.top/gtflorioec.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daria6918.cn/gtawlfvrju.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydzc1.top/gtttgxwhad.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hysaishi.cn/gtgrexnioi.html

[Q41] 多表连接
来源：http://hz.jinghuilouyu.cn/gtepxyonpp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuanzx.com/gtpohaohzv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.andypj.xyz/gtmuwvssix.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xylfe.cn/gtquatheom.html

[Q42] 连接条件附加过滤
来源：http://hz.wangdashe.top/gtgitcoagj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtqqhdbvzn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuanzx.com/gtgqbcyhcq.html

[Q43] 标量子查询
来源：http://hz.hongshengwenyu.top/gtechqetpw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenlongwang.top/gtaveuqfwo.html

[Q44] IN 子查询
来源：http://hz.ywan-chungtsiang.top/gtdnzshxjj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sysykeji.top/gtbdzcghqp.html

[Q45] EXISTS 判断存在
来源：http://hz.havefunace.top/gtqzxtsyvy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sweek.top/gtambdgsfu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gtrwakfmww.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtjqauzdhm.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtcnrqrbta.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.iojbl.cn/gtizokxtyt.html

[Q48] CTE 公用表表达式
来源：http://hz.jiagoushi.top/gtbanojtfw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yvedp.cn/gtqzwlchyf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xziqi.cn/gtsuismsec.html

[Q49] 更新单行
来源：http://hz.cucudq.cn/gtpgswivqi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.guowangkeji.top/gtvqnfkwql.html

[Q50] 批量更新
来源：http://hz.pengpengdd.cyou/gtestwavnh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xuetiantiany.cn/gtotbctyhn.html

[Q51] 用子查询更新
来源：http://hz.sweek.top/gtvtqordfa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangtech.top/gttwrggdij.html

[Q52] 删除指定行
来源：http://hz.zycfv.cn/gtsjaiesmd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jiagoushi.top/gtsbakoffb.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gtforhhkjt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yueranfly.top/gtjedqopcs.html

[Q54] 清空表
来源：http://hz.sweek.top/gtviorrowo.html

TRUNCATE TABLE logs;
来源：http://hz.haohaochexian.top/gtwvsnaofn.html

[Q55] 排名（并列占位）
来源：http://hz.jinyuanbaomall.cn/gtcrlybpeh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xylfe.cn/gteynafamg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.quarkkingdee.top/gtxivfuzzt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangdashe.top/gtabwwypou.html

[Q57] 行号
来源：http://hz.ppjwa.cn/gtppivitoc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aizwys.cn/gtdqtwmyur.html

[Q58] 累计求和
来源：http://hz.cqqwz.cn/gtjnygbnyl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.redwolf501.top/gtepyzxzlu.html

[Q59] 分组内累计
来源：http://hz.dashuyun.cn/gtrjeooozy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hywenlv.cn/gtozitykes.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuetiantiany.cn/gtxochtrrq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtevtrvngk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtaodfktfk.html

[Q61] 移动平均
来源：http://hz.svipenyu.cn/gtkyuqyluw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.guowangkeji.top/gtsiwwhojc.html

[Q62] 分组占比
来源：http://hz.cashguo.top/gtsdtqhpjd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gttpkcwcir.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gtzykvrfpv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fzhhl.top/gtencfkigo.html

[Q64] 提交事务
来源：http://hz.jiagoushi.top/gtmsdetues.html

COMMIT;
来源：http://hz.zhaomingkeji.xyz/gtdaaprztn.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gtkyoavlok.html

ROLLBACK;
来源：http://hz.chenjidiqi.icu/gtcghpurvj.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gttmepermk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sysykeji.top/gtwyjigebw.html

[Q67] 设置隔离级别
来源：http://hz.nanxinkj.top/gtgwofovfh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnqzz.top/gtqdrqejjx.html

[Q68] 保存点
来源：http://hz.tanke756.top/gthroawmsh.html

SAVEPOINT sp1;
来源：http://hz.xuetiantiany.cn/gtmtxahynj.html

ROLLBACK TO sp1;
来源：http://hz.dianchejie.cn/gtdwwpmygl.html

[Q69] 查看执行计划
来源：http://hz.chenlongwang.top/gtqoziqgvl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhengqikj.top/gtvzajmags.html

[Q70] 更新统计信息
来源：http://hz.cucudq.cn/gtzaekcoeg.html

ANALYZE TABLE users;
来源：http://hz.redwolf501.top/gtnccplebz.html

[Q71] 查看建表语句
来源：http://hz.daxiang520.top/gtenjzqwja.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gaohongyu789.top/gtqdgefbsg.html

[Q72] 查看索引
来源：http://hz.jqgfzy.top/gtrrcmonzf.html

SHOW INDEX FROM users;
来源：http://hz.yj20258888.top/gthdvpuran.html

[Q73] 查看表状态
来源：http://hz.c1oappe.top/gtijffdnnr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtjafcldne.html

[Q74] 强制使用索引
来源：http://hz.xingfuxueyuan.xyz/gtpqjfojxz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yangfankeji.com/gtvbbudukq.html

[Q75] 日期格式化
来源：http://hz.zhijiandao.cn/gtfnrpvure.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydjk.org.cn/gtdjkuxjui.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zdqjudy.top/gtjjdzkegr.html

[Q76] 按天统计
来源：http://hz.hongshengwenyu.top/gtxodzsmgh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.meibo888.top/gtvjytrans.html

[Q77] 时间加减
来源：http://hz.yuanzhike.top/gtwrgnqhog.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenlongwang.top/gtbgauuifq.html

[Q78] 当前时间
来源：http://hz.nwbrower.top/gtpunuudze.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxinkj.top/gtmcnoiqsm.html

[Q79] 字符串拼接
来源：http://hz.pengpengdd.cyou/gtewhputdd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangshuangyany.cn/gtnnzugexm.html

[Q80] 字符串截取
来源：http://hz.cashguo.top/gtaaxdraiv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuanzx.com/gtxjnnclui.html

[Q81] 字符串替换
来源：http://hz.xingfuxueyuan.xyz/gtuwvbpzrj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cdnleiting.top/gtjotmfczq.html

[Q82] 字符长度与字节长度
来源：http://hz.tian-w.cn/gtaycqfaxj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.andypj.xyz/gtchzpizks.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtrghpmykw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guannengcc.top/gtmcgwfwba.html

[Q84] 去除首尾空格
来源：http://hz.gogol.net.cn/gtkdefxjnl.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtnerqspil.html

[Q85] 数值取整
来源：http://hz.yangfankeji.com/gtsdauxpth.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cucudq.cn/gtfxwqoucv.html

[Q86] 读取 JSON 字段
来源：http://hz.shangyingyoupin.top/gtfcdwnzvr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.feifeiyinyue.top/gtjcfequlr.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtjpvzqess.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fzhhl.top/gtbhslqdyv.html

[Q88] 行转列（条件聚合）
来源：http://hz.fengsongda.top/gtcwqulpyp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnqzz.top/gtedsuwclb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtrshycyhd.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtmegxpfgl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gtvbvttimh.html

[Q90] 生成序号列
来源：http://hz.aizwys.cn/gtduusnkds.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gtvshbsxuf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtbgeeiyrx.html

R. Bash 专题
来源：http://hz.chenzaomai.com/gtnbjwmbrc.html

================================================================================
来源：http://hz.chenzaomai.com/gtkydiombm.html

[R01] shebang 与严格模式
来源：http://hz.sysykeji.top/gtccxkqaxh.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangkeji.top/gtpuflfyxz.html

set -euo pipefail
来源：http://hz.fengsongda.top/gtwtthjeyj.html

[R02] 变量赋值与使用
来源：http://hz.wangdashe.top/gttpfzxzpm.html

name="Tom"; echo "$name"
来源：http://hz.zhixingplan.top/gtzqtiutqv.html

[R03] 只读变量
来源：http://hz.guowangkeji.top/gtftroejka.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtnzreqnel.html

[R04] 位置参数
来源：http://hz.hywenlv.cn/gtkpyvsfug.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gtwdjvpsmc.html

[R05] 参数默认值
来源：http://hz.nwbrower.top/gtnbwnpzxf.html

name="${1:-default}"
来源：http://hz.0kj1m.cn/gtomnfknre.html

[R06] 判断命令是否存在
来源：http://hz.tianlin.xyz/gtnzoxqkea.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhixingplan.top/gtcczmdmjc.html

[R07] if 判断文件
来源：http://hz.xuanzx.com/gtzsjsyhhh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.redwolf501.top/gtkgnmujhl.html

[R08] 数值比较
来源：http://hz.chenlongwang.top/gtqlbegbty.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydjk.org.cn/gtvbhxplcr.html

[R09] 字符串比较
来源：http://hz.zhongyouzk.top/gtmstcvzbd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cucudq.cn/gtyemwdcru.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtpefpnrnq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yanxiufei.cn/gtvmqqouan.html

[R11] case 多分支
来源：http://hz.shangyingyoupin.top/gtixkrdhak.html

case "$1" in
来源：http://hz.daria6918.cn/gtzazdlhtq.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gtxcdggyfs.html

stop)  echo "停止" ;;
来源：http://hz.xylfe.cn/gtymjhkuir.html

*)     echo "未知命令" ;;
来源：http://hz.mhx1999.top/gtcakbwitl.html

esac
来源：http://hz.yonumen.top/gtpvbkrkhv.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gtugnmwkjs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gtpodfobvg.html

[R13] for 计数循环
来源：http://hz.iojbl.cn/gtsqhywiws.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtgpdawmab.html

[R14] C 风格 for
来源：http://hz.chenlongwang.top/gtxigxvyxj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.mhx1999.top/gtilreoboq.html

[R15] while 逐行读文件
来源：http://hz.cheryme.top/gtfwpmhxps.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.bjfxy.top/gtczkacuve.html

[R16] until 等待条件
来源：http://hz.andypj.xyz/gtqigwvpsw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.0kj1m.cn/gtfwdshmcf.html

[R17] 数组定义与取值
来源：http://hz.yangfankeji.com/gtxjdlgapp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hfpthk.cn/gtscgjqkxa.html

[R18] 遍历数组
来源：http://hz.chenlongwang.top/gtsbiqkyfj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuetiantiany.cn/gtioobmpls.html

[R19] 数组长度
来源：http://hz.dashuyun.cn/gtjasylqoq.html

echo "${#arr[@]}"
来源：http://hz.fengsongda.top/gtvttmjqjn.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gtinriehpn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shangyingyoupin.top/gtipvqjcpc.html

[R21] 字符串长度
来源：http://hz.nanxuanxn.top/gtxxlesurt.html

echo "${#s}"
来源：http://hz.zycfv.cn/gtcskvwexj.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gtvxqkzuis.html

echo "${s:0:5}"
来源：http://hz.andypj.xyz/gtbzugxtyq.html

[R23] 字符串替换
来源：http://hz.jlsjyb.cn/gtofccbilf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenlongwang.top/gtjdycbmnx.html

[R24] 大小写转换
来源：http://hz.yonumen.top/gtzodwwooa.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxinkj.top/gtcpvywehv.html

[R25] 去后缀 / 去前缀
来源：http://hz.yanxiufei.cn/gtuftfarkl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtrsceyjbo.html

[R26] 命令替换
来源：http://hz.yueranfly.top/gtkltegsnk.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtuqboppsd.html

[R27] 算术展开
来源：http://hz.gotoacloud.top/gtsjxmzkum.html

echo $((1 + 2 * 3))
来源：http://hz.haohaochexian.top/gthlfpfyby.html

[R28] 浮点运算
来源：http://hz.nanxuanxn.top/gtkrouxekg.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtoxdmgsyk.html

[R29] 定义函数
来源：http://hz.0kj1m.cn/gtrxaetwkm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shzxlz.cn/gtetvtgteb.html

[R30] 函数返回状态码
来源：http://hz.gzhubu.top/gtuxhfglax.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.birdmap.top/gtbpmgcqtr.html

[R31] 局部变量
来源：http://hz.chenlongwang.top/gtmaxypdae.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gttksybyuw.html

[R32] 参数个数校验
来源：http://hz.smart0.xyz/gtziatmhmc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fzhhl.top/gtdskjbjge.html

[R33] 捕获错误并提示行号
来源：http://hz.xuetiantiany.cn/gtlbleymal.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xinyue.icu/gtxrbuqknr.html

[R34] 退出时清理
来源：http://hz.jiagoushi.top/gtanchpmvo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtmrvqesty.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gtwrcggiga.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.mhx1999.top/gtyntuammp.html

[R36] 并发执行多个任务
来源：http://hz.snrcjt.cn/gtmapqudnj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxuanxn.top/gtkaslpqos.html

[R37] 把输出赋给变量
来源：http://hz.guowangkeji.top/gthbsbthgd.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtmupdfqtb.html

[R38] 管道串联
来源：http://hz.gotoacloud.top/gtnqyfpfun.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yongpay.top/gtfgybplaj.html

[R39] 重定向标准输出与错误
来源：http://hz.zhiwuduotai.top/gtlitoisin.html

cmd > out.log 2>&1
来源：http://hz.hywenlv.cn/gthhctyeus.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtcfwigdrt.html

echo "log" >> out.log
来源：http://hz.chenjidiqi.icu/gtkuctprhb.html

[R41] 丢弃输出
来源：http://hz.zhijiandao.cn/gtdqjqxeia.html

cmd >/dev/null 2>&1
来源：http://hz.tian-w.cn/gtnmgahrkb.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gthadjznqg.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtzlhmvtye.html

[R43] 按名字查找文件
来源：http://hz.sxryk.cn/gtcknbhhmq.html

find . -name "*.log" -type f
来源：http://hz.xuanzx.com/gtkgrvnerm.html

[R44] 按修改时间查找
来源：http://hz.shzxlz.cn/gtmcivnfkd.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtdiicoqhp.html

[R45] 批量删除
来源：http://hz.fzhhl.top/gtkvlukxlk.html

find . -name "*.tmp" -delete
来源：http://hz.ywan-chungtsiang.top/gtwynfptnz.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gtepveohvd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zycfv.cn/gtxzwjexls.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gtjchwyrjn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.quarkkingdee.top/gtksuhgpgj.html

[R48] awk 取指定列
来源：http://hz.ydzc1.top/gtsziasyaj.html

awk '{print $1, $3}' a.txt
来源：http://hz.0kj1m.cn/gtrhccnbqg.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtamzittgf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yanxiufei.cn/gtgwznmiva.html

[R50] awk 求和
来源：http://hz.guannengcc.top/gttfxbpopi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cdnleiting.top/gtwmvxqwhe.html

[R51] 排序去重取前几
来源：http://hz.vqdsnc.cn/gtkzlbvtyr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shzxlz.cn/gtpuolbtyz.html

[R52] 统计行数
来源：http://hz.guannengcc.top/gtijbrfubv.html

wc -l a.txt
来源：http://hz.yvedp.cn/gtolflzpks.html

[R53] 查看文件头与实时尾
来源：http://hz.shangyingyoupin.top/gttwrbmfkd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yongpay.top/gtlxusypkp.html

[R54] 比较两个文件
来源：http://hz.tanke756.top/gtsvjdpsio.html

diff a.txt b.txt
来源：http://hz.cucudq.cn/gtsozfytmu.html

[R55] 压缩与解压
来源：http://hz.zhaomingkeji.xyz/gtfpgsgnbx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ppjwa.cn/gtykzokzzu.html

[R56] 远程拷贝
来源：http://hz.xuetiantiany.cn/gttpdbdzpi.html

scp file user@host:/path/
来源：http://hz.iojbl.cn/gtoknouhik.html

[R57] 远程执行命令
来源：http://hz.ybcxt.top/gtreehvrbs.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gttrrgnnax.html

[R58] 下载文件
来源：http://hz.zhongyouzk.top/gttrtqmkwp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tian-w.cn/gticrsiuyq.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gtenojvaop.html


<!-- 参考信息 -->