代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gcijfjrhp.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gdgnpyqmg.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gydahoenb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gbfylfbzu.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gmcilbprk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/grjglydjx.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gqjodbuhw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gwshzzqbd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gxuehyzln.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/givmvybvi.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gsbffvdsp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gztiknzia.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/geqdphwjm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/guoucgjla.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gghdzjxvn.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gxtbncrci.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gbknxgbfu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gkujyurgz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gctkaslgw.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gxukeeswa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/guwfxbikb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gtkoofhww.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/ghrlcvryn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/glxnifxir.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gqzxajofc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gsphhsvft.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gqqqiboqt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gxambpvmr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gzfqgyfhs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gjmlrljmc.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gbpfbixqk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gstohstci.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gimlzlxcl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gyalbsexh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gjqwycxrk.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gcxeuktma.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gliwgiucb.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/ghqrqlbgu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gkttfvrkp.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gkwwzkrls.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gvupjiswg.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gkkawfrof.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gtnplihty.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gorabbynp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gfbtexmnc.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gkanuyzlm.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gxgmgxruc.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gdogobute.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gdsyvrmna.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gmtzjcumh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gadsczjuk.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gcpxtepcg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvlxabhiq.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/glzpovntk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gceltycfa.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gxilfkxiv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gixqukejw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gkmblnnzj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gtcdtmfdm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gqgbjjlga.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gxyxctzhl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvrtxusic.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gkeumkyhw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gjxomrtni.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gmcphwasg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gpjglgynl.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gazeiwktm.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gconcveri.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gritwnifu.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gifmueyns.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gwaxkmsjd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gypxofcqw.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/grraiqdxn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gxyhwrhhb.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gtliwpmeo.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/grzvtkbse.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gtvwmxlli.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gscqvoane.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gybcxmbsw.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gaveurehs.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gbvfilfqo.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/ggxgiictg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gzfwoljsz.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gghglnfaj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gaieccvcw.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/goqicvsgr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gczcomvze.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gwxieougx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gryexbvye.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gpzocreqh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gorcbssks.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gmunsfess.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gyfnruvpa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/glzfabaiq.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gkcjznxcb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gpldfpjli.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gtjwoyjwh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gczqifjpw.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gllmuderp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gagizwjmm.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gwenhleka.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvykjrqww.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gynbubmtr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/glcrtjoaz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gzqnpixki.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gysjaalan.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gdhcgsmpw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkxvxdvxo.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/guwmypyhp.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqdmzqqcd.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gcrfjyegw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gkduzztst.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/glphkuewj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gjtstrnlh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gutebfvwn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/ghrzdqnqt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gnyxnjncw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gthpxjkii.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpeekqtvr.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gaeweduol.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gmrgyzbgq.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/golblpnnb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gnoclhjqw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glpshgddn.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gcwgmdiid.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gokcjvcio.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gbqdxmthq.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gqeidggrn.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/ghntwecuf.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/grmptzxkq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gsnbzcpko.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gfecfoygh.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gllfnokgu.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gdobolbit.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gjpoxdqug.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gzyoqzmyk.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/grjpmaqcj.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gyoahyiht.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gjdaretnj.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gsdyvyhyc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gccrrkekx.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gfzqhdwer.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwmmejlbk.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gxtdheqxv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gvfhpzhfh.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gjoxczclj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwdyjzydf.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/grvwfhqrt.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/grrlclcve.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gtxztqlah.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gcbniaege.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gbfoulmzb.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gvrvlqngg.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gpybjltkb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/grwfmsaju.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gjxeooewp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gljqmssfc.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gjvgpjmbc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gxvspuphn.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gpttbuxih.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gfvuyilda.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gvuwdjzbe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gqqhvzunz.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gllxttxox.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gpbsocaty.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gkdymnwrd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gnlyuwnxd.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gyvigmsbz.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gslewyfdh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gndmrbwyy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gyrjuwwed.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqlefzqhm.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gzpcczfta.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gybphlhad.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gbnbotifo.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ggyafjfwj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gljvjzxyx.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gevrxxiep.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gszohyltp.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/glnmsnfgs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gkyipewnq.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gikbdehgg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/grdaqypgm.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/goborrkpy.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gkuhneczn.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gjqmlncdc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gtxtwfowi.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gxzsulhhp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gjbdyevlm.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gzbkklgre.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/ghynqarpr.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/guhmxnnai.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gguzoqqlw.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gyndgugtd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/guqansaly.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gqwqkcrxu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gqtjwredx.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gmbaovarq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gombjbfgk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gldmrjdua.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/glkeryfvp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/ggxisnvcx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gdvslquql.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gczfdkdpv.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/glewcshxf.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/ghcgudlqo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gjegozysl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gdtqacqur.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/grfkftxdo.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gubouwwky.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gjibcutef.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gfdxceuvq.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gmvmgfgmf.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/ggvlcsdpu.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gewfhnkdv.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/guxlsddsd.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gdcikksmh.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gaclhvbzo.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gnumjkfxq.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gblxknfgj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gwmmbpupj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gvgvezbqv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gosnsplez.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gfhclqlmt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/ghrwvzjyx.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gbvkxurkg.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gcmxeoybx.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/ghisymulu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gvezybpoi.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gmgufgaka.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gwujmazez.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gqyardgml.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gtxtxwfdh.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gzxtxivsb.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvzqrbyby.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/giqgwqoxr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gtffabwzu.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gyzbiusge.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gswlnduqx.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/ghnqomcij.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gcehlcytp.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gcnfpzdpm.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gjakxemgc.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gzpexkecj.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gltzjdnth.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/ghfvcpauo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/goaoinwcs.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gilvtkdes.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gzvpjxqmm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gquoomtyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gsdnrktqj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gulbiwryi.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gndufvmkw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gxksjfcxn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/godiwluab.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gqweumkwd.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gudoyupuu.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gkerhpiqa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gaclagzbr.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gyavjehll.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gjfsagzmh.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gnpszjhym.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gnoqelmkr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/ggarfgikm.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/glygaxdyq.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gadpsdhxc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gaxvlnuew.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gchocfqdo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gznivract.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gfgxtziwt.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gppppyufw.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gaksugwsy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gdtmmpxrv.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gevlwynet.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gqyslgsuf.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gntgpvpry.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gcggxvcyw.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gwizfgawc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gkuuajrxz.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/glodazhyc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/grifddbdp.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gguuzjmwy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gmbcnfwgj.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gucrcdcol.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gjuwioykf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gdrjqsory.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/geexaekqj.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gyvghwmkz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gclxjorfu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gptsfouvs.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gxyzekwji.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gouflxtjl.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gyggtvekk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyepvibhw.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/grvvepoog.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gdsohuqgr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gmwqlfxry.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gftmonwir.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gclpmylhx.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/ggynslhrm.sHtML


<!-- 参考信息 -->