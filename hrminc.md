代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yueranfly.top/gtqufhxrlk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtrmfyozrp.html

[Q13] 忽略重复插入
来源：http://hz.jinqigfzy.top/gtzopgybdt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gtfxieindo.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gtommvkxui.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pengpengdd.cyou/gtmxmwlqjn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shzxlz.cn/gtptauslcy.html

[Q15] 查询全部
来源：http://hz.xuanzx.com/gtyznxhfnf.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtufpofwku.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtzekrnrgz.html

SELECT id, name FROM users;
来源：http://hz.bjfxy.top/gtsknvjczj.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gthtibvvmm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xylfe.cn/gthzuswzan.html

[Q18] 模糊匹配
来源：http://hz.zhaomingkeji.xyz/gtegedkqpo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.mhx1999.top/gtkggqshaj.html

[Q19] 范围查询
来源：http://hz.jlsjyb.cn/gtrrwecahj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.mhx1999.top/gtrwmiksra.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtdlxqtjrx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guowangkeji.top/gtebdhakcb.html

[Q21] 空值判断
来源：http://hz.aizwys.cn/gtzekzuoxx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhoulong.xyz/gtcntmdoah.html

[Q22] 排序
来源：http://hz.jiagoushi.top/gtbtwpvexy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.kuanghao11.cn/gtpgkqaobh.html

[Q23] 分页
来源：http://hz.tianlin.xyz/gtfmvxzihn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cqqwz.cn/gtcbgpokbr.html

[Q24] 去重
来源：http://hz.haohaochexian.top/gtrqefwvon.html

SELECT DISTINCT city FROM users;
来源：http://hz.mhx1999.top/gtbstpvysf.html

[Q25] 只取前 N 条
来源：http://hz.nanxuanxn.top/gtnytmaqxr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gaohongyu789.top/gtstyqgtao.html

[Q26] 计数
来源：http://hz.hywenlv.cn/gtrlrlfymz.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuxming.cn/gtjqhvyanp.html

[Q27] 条件计数
来源：http://hz.daxiang520.top/gtpmhzbani.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sysykeji.top/gtsclzhpcy.html

[Q28] 求和与平均
来源：http://hz.yonumen.top/gtyxebozsm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtrloehnim.html

[Q29] 最大最小值
来源：http://hz.xuanzx.com/gthjzrifxa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtkasmarku.html

[Q30] 分组统计
来源：http://hz.jqgfzy.top/gtsfsyhnlq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtxymsurkf.html

[Q31] 分组后过滤
来源：http://hz.zhiwuduotai.top/gtrukmwufp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pycfn.com/gtvvousvqe.html

[Q32] 分组拼接字符串
来源：http://hz.zhongyouzk.top/gtrfzifacf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtozzoxmmb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xylfe.cn/gtntpkyokn.html

[Q33] 多列分组
来源：http://hz.316326.xyz/gtuxkyebzn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jyoumei.cn/gtjhbprrfy.html

[Q34] 每组取第一条
来源：http://hz.shuidangran.top/gtascfyalt.html

SELECT * FROM (
来源：http://hz.andypj.xyz/gttjfvbwnt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jlsjyb.cn/gtpudytyfk.html

) t WHERE rn = 1;
来源：http://hz.nanxuanxn.top/gtezmmxcss.html

[Q35] 内连接
来源：http://hz.svipenyu.cn/gtfcckpjhu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gtwhfbdzxs.html

[Q36] 左连接
来源：http://hz.shanyushiyangkeji.top/gtlvzzdshr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtqasqgwlz.html

[Q37] 右连接
来源：http://hz.jiagoushi.top/gtlhmmpaln.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhengqikj.top/gtseayvodb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yueranfly.top/gttvgxqoiz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.guannengcc.top/gtagvbaikm.html

[Q39] 自连接（查上下级）
来源：http://hz.zhoulong.xyz/gtcbxvibdo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shuidangran.top/gttqlghmfp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhixingplan.top/gtgnxhdwck.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.andypj.xyz/gthjbxfxtc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fzhhl.top/gtfkfmffjn.html

[Q41] 多表连接
来源：http://hz.ydzc1.top/gtdzzdrkrt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zdqjudy.top/gtwppnjffy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gttfblwvws.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhiwuduotai.top/gtrzycpoao.html

[Q42] 连接条件附加过滤
来源：http://hz.meibo888.top/gtrvkomrcw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yuanzhike.top/gtaxxkbwwx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sysykeji.top/gtmlhcfood.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtugjtkrlf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gtmiinlsyg.html

[Q44] IN 子查询
来源：http://hz.zhiwuduotai.top/gtdtuksmpw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xziqi.cn/gtulvtogqn.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258888.top/gtgrdiwvmt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtoshjahca.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.redwolf501.top/gtpoyopltx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gteadqtzhe.html

[Q47] 与平均值比较
来源：http://hz.zhijiandao.cn/gtldszzznm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258888.top/gtkvvcllwq.html

[Q48] CTE 公用表表达式
来源：http://hz.ywan-chungtsiang.top/gteoplutir.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cucudq.cn/gtukoopljs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.meibo888.top/gtadlfuvcg.html

[Q49] 更新单行
来源：http://hz.jianghu66.top/gtcprleles.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtbglkcjqg.html

[Q50] 批量更新
来源：http://hz.fengsongda.top/gtuomojhss.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtlwdwjnxb.html

[Q51] 用子查询更新
来源：http://hz.gogol.net.cn/gtpldtgfar.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.mhx1999.top/gtnoyqglgo.html

[Q52] 删除指定行
来源：http://hz.hongshengwenyu.top/gtdqpwsoio.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dianchejie.cn/gtpqyvoxej.html

[Q53] 按条件删除
来源：http://hz.hnqzz.top/gtodmyfuku.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtgkhriqqq.html

[Q54] 清空表
来源：http://hz.jqgfzy.top/gtmrrltlwa.html

TRUNCATE TABLE logs;
来源：http://hz.quarkkingdee.top/gtndzjjmqz.html

[Q55] 排名（并列占位）
来源：http://hz.snrcjt.cn/gtnnfcohox.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dianchejie.cn/gtcmpzwarg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yongpay.top/gtqosnrqzj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtoldqlyta.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtthcflzek.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yanxiufei.cn/gtnwwmowwg.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gttivsetpt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sxryk.cn/gtbkoevajt.html

[Q59] 分组内累计
来源：http://hz.nwbrower.top/gtmzfppmqm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtpvsgjyjt.html

[Q60] 取上一行 / 下一行
来源：http://hz.jlsjyb.cn/gtwqvvawrg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dianchejie.cn/gtieszasow.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guannengcc.top/gtjipkxyax.html

[Q61] 移动平均
来源：http://hz.yanxiufei.cn/gtcnuqlfnv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gtbagqxppn.html

[Q62] 分组占比
来源：http://hz.nanxuanxn.top/gtcbirpwrc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sweek.top/gtbhkdqnod.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtomnrpqsv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.feifeiyinyue.top/gtpdpxpxgn.html

[Q64] 提交事务
来源：http://hz.cucudq.cn/gtctshpbnn.html

COMMIT;
来源：http://hz.hfpthk.cn/gtsfwwsvzh.html

[Q65] 回滚事务
来源：http://hz.xuetiantiany.cn/gttbuuyxly.html

ROLLBACK;
来源：http://hz.ydjk.org.cn/gteeqlalrw.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtyialchlf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.kuanghao11.cn/gtyglblehi.html

[Q67] 设置隔离级别
来源：http://hz.jqgufenzy.top/gtknbhojxj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj202588.top/gtxiboqzcn.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtgobnprew.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtpccooktr.html

ROLLBACK TO sp1;
来源：http://hz.jinqigfzy.top/gtghglowdt.html

[Q69] 查看执行计划
来源：http://hz.cdnleiting.top/gtwbpkoovi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gtuqgayptp.html

[Q70] 更新统计信息
来源：http://hz.birdmap.top/gtnhrkvlfj.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtnbpepgsl.html

[Q71] 查看建表语句
来源：http://hz.ybcxt.top/gtfxgkejde.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnxiangtu.top/gticadleuy.html

[Q72] 查看索引
来源：http://hz.wangshuangyany.cn/gttappxtkg.html

SHOW INDEX FROM users;
来源：http://hz.zhixingplan.top/gtedtcksxq.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gtbbxodswb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sweek.top/gttykgqzwj.html

[Q74] 强制使用索引
来源：http://hz.fzhhl.top/gtsutywevu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hammf.cn/gtebjjzbzj.html

[Q75] 日期格式化
来源：http://hz.shzxlz.cn/gtvpiuihkm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.kuanghao11.cn/gtlpflezmz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hfpthk.cn/gtwprdiihd.html

[Q76] 按天统计
来源：http://hz.chenlongwang.top/gtpajpyhey.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shzxlz.cn/gtqnzuiier.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gtheexmkkp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangdashe.top/gtfvqsdqiw.html

[Q78] 当前时间
来源：http://hz.cashguo.top/gtsrjgddsu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shzxlz.cn/gtmvufugag.html

[Q79] 字符串拼接
来源：http://hz.dashuyun.cn/gtbkduhorr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.haohaochexian.top/gtmubffndg.html

[Q80] 字符串截取
来源：http://hz.daria6918.cn/gtqzhgxadd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtyoalzazv.html

[Q81] 字符串替换
来源：http://hz.xingfuxueyuan.xyz/gtdtjhdgvu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gtotdcjpdf.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gtlqkwphdc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuanzx.com/gtigejekhh.html

[Q83] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtpnqgvmxq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhijiandao.cn/gtnakqluqu.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtsdzwsqfw.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtiolndbor.html

[Q85] 数值取整
来源：http://hz.redwolf501.top/gtoinubagg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhongyouzk.top/gtmzemwwvj.html

[Q86] 读取 JSON 字段
来源：http://hz.dashuyun.cn/gtfiscljsp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gogol.net.cn/gtnxsqfmau.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gttowocnmt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dashuyun.cn/gtpisxaaik.html

[Q88] 行转列（条件聚合）
来源：http://hz.vqdsnc.cn/gttdbeovro.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydjk.org.cn/gthoobyjie.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tanke756.top/gteasyjkwy.html

[Q89] 判断表是否存在
来源：http://hz.xuetiantiany.cn/gtoqecntwz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aibaodan.cn/gtwogqovuq.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtsedvisra.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hammf.cn/gtlekcxdom.html

================================================================================
来源：http://hz.cheryme.top/gtkzirwesp.html

R. Bash 专题
来源：http://hz.pycfn.com/gttmoseefx.html

================================================================================
来源：http://hz.shuidangran.top/gtewxwqfok.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gthyyjbpej.html

#!/usr/bin/env bash
来源：http://hz.birdmap.top/gtzhweatao.html

set -euo pipefail
来源：http://hz.yuxming.cn/gtcqmjrpjf.html

[R02] 变量赋值与使用
来源：http://hz.xylfe.cn/gttpshjzzj.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtajqguzxs.html

[R03] 只读变量
来源：http://hz.cheryme.top/gtjnwkjdrt.html

readonly PI=3.14
来源：http://hz.jinqigufen.top/gtqvrzmdcc.html

[R04] 位置参数
来源：http://hz.nanxuanxn.top/gtwcqfhjfv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jqgufenzy.top/gtxsrrlcqr.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtvhasvmts.html

name="${1:-default}"
来源：http://hz.cheryme.top/gtjayziqtr.html

[R06] 判断命令是否存在
来源：http://hz.zhixingplan.top/gtnkfduhyc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fzhhl.top/gtcrmlpepl.html

[R07] if 判断文件
来源：http://hz.haohaochexian.top/gtagbyliak.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xuetiantiany.cn/gtzcvwszqk.html

[R08] 数值比较
来源：http://hz.shanyushiyangtech.top/gtkwwtresk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hnqzz.top/gtbbpldwsg.html

[R09] 字符串比较
来源：http://hz.jianghu66.top/gtkzlcsunb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuetiantiany.cn/gtwpxxtfqb.html

[R10] 正则匹配
来源：http://hz.shanyushiyangkeji.top/gtcaxcltex.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gttcldljmc.html

[R11] case 多分支
来源：http://hz.jlsjyb.cn/gtwwgdfibz.html

case "$1" in
来源：http://hz.tanke756.top/gtlsphlewq.html

start) echo "启动" ;;
来源：http://hz.nanxuanxn.top/gtixelsrqh.html

stop)  echo "停止" ;;
来源：http://hz.nanxinkj.top/gtiupseogi.html

*)     echo "未知命令" ;;
来源：http://hz.zhengqikj.top/gteqwkewzb.html

esac
来源：http://hz.jinqigfzy.top/gtixxgfluf.html

[R12] for 遍历文件
来源：http://hz.jiagoushi.top/gtsqjaqztf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gtsnxbwhcd.html

[R13] for 计数循环
来源：http://hz.daria6918.cn/gtadgcfooj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gtbvjpdxld.html

[R14] C 风格 for
来源：http://hz.hongshengwenyu.top/gtkkxiutpo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gtelgkofey.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtzhaerekk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jlsjyb.cn/gtqgvtfrte.html

[R16] until 等待条件
来源：http://hz.fengsongda.top/gtwddoqopd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtffhdtnxl.html

[R17] 数组定义与取值
来源：http://hz.jinqigfzy.top/gtsmiyddys.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenjidiqi.icu/gtzyrxahbz.html

[R18] 遍历数组
来源：http://hz.vqdsnc.cn/gtaqhykvjw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtyqrzgauh.html

[R19] 数组长度
来源：http://hz.hongshengwenyu.top/gtswobwjje.html

echo "${#arr[@]}"
来源：http://hz.yuxming.cn/gtxueojwpq.html

[R20] 关联数组（字典）
来源：http://hz.pengpengdd.cyou/gtnrevbtyx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gogol.net.cn/gtjucnehof.html

[R21] 字符串长度
来源：http://hz.vqdsnc.cn/gtcthbxsgj.html

echo "${#s}"
来源：http://hz.cashguo.top/gtsokxhvjv.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtrvhqzbwf.html

echo "${s:0:5}"
来源：http://hz.sxryk.cn/gtxkkgqebz.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gteubtlrrc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zycfv.cn/gtgnufitkw.html

[R24] 大小写转换
来源：http://hz.birdmap.top/gtgrrptzhu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dianchejie.cn/gtdtbtzprf.html

[R25] 去后缀 / 去前缀
来源：http://hz.ywan-chungtsiang.top/gthmanfyjf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gttfmugutu.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtdkiyctcf.html

now=$(date +%F); echo "$now"
来源：http://hz.shangyingyoupin.top/gtnanokgbf.html

[R27] 算术展开
来源：http://hz.daria6918.cn/gtpagqucbl.html

echo $((1 + 2 * 3))
来源：http://hz.aibaodan.cn/gtzwgdxdvj.html

[R28] 浮点运算
来源：http://hz.hysaishi.cn/gtoaattpbr.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnxiangtu.top/gtnxamvwyx.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtsjifkjqt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yonumen.top/gtmpukrwqq.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtlzutxjni.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.svipenyu.cn/gtnyfihnqt.html

[R31] 局部变量
来源：http://hz.zhiwuduotai.top/gtmgyrauin.html

f() { local x=1; echo "$x"; }
来源：http://hz.jlsjyb.cn/gtnzkwuxpu.html

[R32] 参数个数校验
来源：http://hz.yuanzhike.top/gtjldlqicy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ybcxt.top/gtznaqoggy.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gtmusapwld.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hysaishi.cn/gtsekbfutm.html

[R34] 退出时清理
来源：http://hz.yanxiufei.cn/gtrremliyj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtpxioqiib.html

[R35] 后台执行并等待
来源：http://hz.zhengqikj.top/gtejgsgapg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ybcxt.top/gtgqnmroum.html

[R36] 并发执行多个任务
来源：http://hz.ydzc1.top/gthhkvinfa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.snrcjt.cn/gtpgpyfvov.html

[R37] 把输出赋给变量
来源：http://hz.birdmap.top/gtqlrznwju.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtulzrexch.html

[R38] 管道串联
来源：http://hz.hongshengwenyu.top/gtgndnxdop.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtlojjmdap.html

[R39] 重定向标准输出与错误
来源：http://hz.sysykeji.top/gtckchplla.html

cmd > out.log 2>&1
来源：http://hz.gzhubu.top/gtbwvbqfxh.html

[R40] 追加写日志
来源：http://hz.shanyushiyangtech.top/gtjjakckbo.html

echo "log" >> out.log
来源：http://hz.ydjk.org.cn/gtrrksdexa.html

[R41] 丢弃输出
来源：http://hz.guowangkeji.top/gtjhbomvnu.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtfhjkxnee.html

[R42] 输入重定向
来源：http://hz.c1oappe.top/gtzywbfqhb.html

wc -l < a.txt
来源：http://hz.hysaishi.cn/gtzctnibmx.html

[R43] 按名字查找文件
来源：http://hz.chenzaomai.com/gtujueinan.html

find . -name "*.log" -type f
来源：http://hz.zdqjudy.top/gtbxjlqtnb.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtwrbjukyu.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtctclwpaf.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gtframhefz.html

find . -name "*.tmp" -delete
来源：http://hz.snrcjt.cn/gtqrvdwrqs.html

[R46] 递归替换文件内容
来源：http://hz.pycfn.com/gtjoqbtvua.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.52xcode.cn/gttjxczaol.html

[R47] sed 单行替换
来源：http://hz.tianlin.xyz/gtpbeyavrc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cucudq.cn/gtasyeovac.html

[R48] awk 取指定列
来源：http://hz.gogol.net.cn/gtzgkfnxcx.html

awk '{print $1, $3}' a.txt
来源：http://hz.havefunace.top/gtaxudohnd.html

[R49] awk 带条件
来源：http://hz.redwolf501.top/gtqhmiybqz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtohuhakbr.html

[R50] awk 求和
来源：http://hz.chenlongwang.top/gtjynwbovi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.feifeiyinyue.top/gtovqmootr.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gtdvphmyey.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zdqjudy.top/gtxnfhpout.html

[R52] 统计行数
来源：http://hz.hnqzz.top/gtkdmyhpfv.html

wc -l a.txt
来源：http://hz.jinqigfzy.top/gtmjdflmla.html

[R53] 查看文件头与实时尾
来源：http://hz.cucudq.cn/gtglmkbafs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.andypj.xyz/gtzczbgkdu.html

[R54] 比较两个文件
来源：http://hz.ywan-chungtsiang.top/gtowgpnfvo.html

diff a.txt b.txt
来源：http://hz.sweek.top/gtbmecvzic.html

[R55] 压缩与解压
来源：http://hz.yj202588.top/gtbjhcmkps.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtxwlnnbya.html

[R56] 远程拷贝
来源：http://hz.cdnleiting.top/gtctsqwjvp.html

scp file user@host:/path/
来源：http://hz.shzxlz.cn/gtvyatsbuj.html

[R57] 远程执行命令
来源：http://hz.yuanzhike.top/gtpfrsrbov.html

ssh user@host 'uptime'
来源：http://hz.cdnleiting.top/gtqfuluqjl.html

[R58] 下载文件
来源：http://hz.yongpay.top/gtiuszpffc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cucudq.cn/gtywqdukdo.html

[R59] 发 POST JSON
来源：http://hz.svipenyu.cn/gtysosymrg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhiwuduotai.top/gtsehnjvju.html

[R60] 只看 HTTP 状态码
来源：http://hz.0kj1m.cn/gthjbaerxo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgfzy.top/gtnrzmhyjk.html

[R61] 磁盘占用
来源：http://hz.ydjk.org.cn/gtgdetquop.html


<!-- 参考信息 -->