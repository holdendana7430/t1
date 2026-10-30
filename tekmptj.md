代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuhlabwy.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/geiljxvxj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gisgmqlpk.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gtuiobtbh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdbkfhcwb.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfilgfwi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gmdakcprl.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gymmgjwbr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/glkkllhsu.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjptizued.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gempsxdoa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgfujjsh.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gmdlqqzdh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgpopbaf.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhpkpcrp.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gzuuolrka.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gztmqafxf.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gepaccrfu.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/glorfazcy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gzgrwyqzf.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gbnuuwumk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gplnodbif.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepeeeobs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttlcplah.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gixvxmbpd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/goryorduv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlpodsqv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gctiogicq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcbfmvlx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxclbdse.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohhvwhgv.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxziwras.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gwkxfaqwu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gfqgunwko.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gghrcnngj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggdvphzdb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/genixiibd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gmsxnpxtg.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/ggjzzadcv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/glplzxghp.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gpgrkvtbi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgawfyra.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemmhrddj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbnotjks.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/garfunoqy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpenegstg.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grpwujyhq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gggpmuvyy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/ghprdxqjg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwiunonm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gywoqqdda.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gebqcphql.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gvkimgzrq.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gzmjkpswe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysmzrimd.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gdzblvjwd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoredmbg.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gnflklmwa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/giwnjagmg.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjzjijlds.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdesrfvlk.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gnhjjibai.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/ggguzijfh.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdposqbx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmilmcadu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gapvovhbl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwxtsffa.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmicujbj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxcwljxsc.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwqafgho.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gjklqcfoc.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gknpifvuq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gqmpzcajw.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/govzxlkva.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gcipbkhtu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqgzjojze.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtmhmiyg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgxkozwk.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gerpfjyqe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorffkjob.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikppujhl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhyonlms.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/govaagguo.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqegxvxvn.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gbgqxfytk.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvksgbwkv.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbvcornmj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gucctoddl.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gahyghbnb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gcvvpwhvh.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmfwjoqr.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjcytgum.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/grqcezmcv.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gdqgiamtl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/grffybkrh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtrvqnpf.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/geinqdspk.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/glfpkktmb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuvrzkua.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgxpqagh.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfpwwfkvv.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gunakafre.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiiiibsj.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gubxiojbg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gzauhsqdd.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoxplctn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gimgybnpb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/ggprohfsg.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gbperojqc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsvadbvc.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpsfzwhn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpvnusjb.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gmfneeysw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvhozblt.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfmpoqnt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhhkutle.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtyfkmqb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwplxkft.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gghjftlep.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/galbvndvq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gaenflnya.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzmqkbkg.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gledopsyq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkvmwbhx.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gkmljsktq.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhiemaea.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeluaknd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/grhgcymmb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnxkcgfs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxtomwxo.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzdpijeup.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjbzjkxg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/glrqnjlxu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyqdmaql.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudriiljr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdwzyhtq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gsvuapnrz.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gapjtfyrh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/giuasyhou.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmfhacvei.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqtixkids.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaquuhib.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvumndgn.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gfjlcfftc.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gwwgwdysj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/godoshijg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvkhswal.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmzbuieqb.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/grwprkgvk.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyxsmmxr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gxabvaunh.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/ganygahjx.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduiiphwq.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gquifezuj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcetzmrpu.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/goxptmeid.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gmnycrwhd.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/ggntwkyal.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/goayakfca.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gpmkazzqg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gkjdhqqtt.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzgdnhfw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gtdnaxlfv.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gpclgwiav.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gprkkgwov.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gvrjfgccm.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxyyyzgqm.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaaexcca.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdskkala.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbghldqte.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglpjuuwr.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqknkazh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gssosohdc.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnukshzp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwnpozrrw.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gobqlgtny.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpilpgtbp.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmhzyexq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzkqrkpcn.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gxvtyzxtt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqjtrexk.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gcyhfjxvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfhnqbdj.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhbnvger.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gueqpsepv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuygqmta.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtkkoyufn.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbicwfvj.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmrumwbn.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gamxnvmol.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkldpoubi.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqubvcxj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwecutvll.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujipiqzh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/giwrrdgcu.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gihzfqrxu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/guysgdxsx.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaweevxj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gyjzmzigh.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gtxvqabaz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gqgjajuqt.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtahhfexv.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gelgufbjz.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmbgfopn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjgmeblx.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlifxuhf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gpftedqkn.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gstdbyufr.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbywebbe.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gosyuokyr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsrnfcmp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxbnjccy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/grztswwle.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/ghulavllg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/giwofnhkx.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gsotwycxl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnemlanh.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxluatxh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gllhumkxm.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/glfqnuiwf.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gntjcofzd.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gegkhjtiw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqljwnaqp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghydscsjw.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnyabxun.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gifvxnxgq.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjygmfkc.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gnrfbrqfm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gowfwnsgy.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzohiskh.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/geeebllla.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnocnpzhm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/givagkpvo.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gagqoppvi.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gffptjlkm.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gcsrsxhff.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gffhpxdcl.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojvtjewk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gphqrwxaf.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gunkdzhfw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewyusgdw.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gypramvzf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnvogryih.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gnwvokjwb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gucgxdbmm.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gpjhgcoxy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpbucwkq.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gvkpxsttl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/giidgjvrs.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxssasqh.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrjyzydv.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gomegavap.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdzzcwux.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvetbpdwd.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwgkpadj.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckwjfjor.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyphzefb.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/galsylmbd.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gyvouuddh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnhwurwn.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gwdtfzwse.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtgouncmk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gtjzigtmj.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gwadlukyz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuucmwzo.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gefpylufe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwusmfolz.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/golewxnoa.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/geldehpjz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjlshehr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gueywaypl.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gctzfmahm.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gmuyxkzcv.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmounifm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gjjiuqgfl.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gsfoedufq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gakmwqhwp.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/glsruhqwa.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyqqwkmt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcnzlbyh.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gcacyokbh.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gvtzyaqog.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghxnbhlhu.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfaucmnu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvlaxjuq.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvabubzw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gamdvlfvy.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grhorbmub.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/ghtvqajhi.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gqprnzqbu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhobnrlw.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynpseiny.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlcuqaps.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggffwqocw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxvnrbvz.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzffijeuv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gdfgusdfs.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtpbbtzu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gevxtqrbz.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gapyjuetf.sHtML


<!-- 参考信息 -->