代发 wailian999

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gvzoulsnc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gsslvttmm.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gxjuovwor.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gewygknam.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gksvqtylj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/ghtcqrxqs.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gkumowxej.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/ghewfzsav.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gffopedmo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/grxngxvgv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/ghpxhnbwf.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gjujfnufn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/galouanwf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gllyjfdvv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gobasrwie.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gzukrsdzv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gkymrytuj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/ghpqvxkdk.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gigjizygk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gzlhxwqjn.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gmqsqtkcr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gwktcstok.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gyoxyqshc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gmmoronqx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gytajfgbn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gzuiuvxja.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gmpsuhory.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gutghmiee.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gvfootyvu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ghrglzejg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gnywuijem.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gwwpisuxp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gjiipdoob.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/glpylbyhe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gfeuzxsff.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gwkwvykrv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gmqpggkww.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gjkyibvkd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gpbksiyar.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/goktzxmaa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gkjoqukww.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gtjjdsqfa.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gznigxyyh.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gvxontqii.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gnlretbrj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/grgaxyozo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gexomxmay.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gavrrrres.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/glelzbsew.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/ganqbktmk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjfqelqse.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gwvzcvxzs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gfjgvwigp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gksmxooeq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gnutfbtof.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxvkswrit.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/genxmivvt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glzuuxtxo.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gyqshrclz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gkxpmvnnn.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gwrkhtpow.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gdrowowbv.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gwztepyap.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gwtjtdrba.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gngtdvxrd.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gqegeiqod.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/giaksdnon.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/ggqphjbbd.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/ggdnclnkr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gmnaholdb.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/ggnesmlps.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/glayglgnl.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gernrjuko.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gqqqlsdou.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/ggqbgazpj.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gjpwknedk.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gfqylnipv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gvqbqmdyg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gimnzhevb.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/ggmsznguh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjpdtgffw.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gxbuwufbe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gdrpdculg.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gycbhopgc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gyqemacyb.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/guzbblaol.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjuayoukw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gigsahcmm.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gylmcisub.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gnlanzmaf.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/ggtgdjhzy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gwpnsriiu.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gjbtmcmme.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gsigrdksz.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gzlhirscu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/grzrsvxwv.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gdbwcgutr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyokzufav.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gxwqxqdzl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guoafyyjk.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gwjfwwdld.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvoxpkjbe.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/guohqockq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcavrxvto.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/geldylmmz.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gvzrtymwz.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gromluutr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gtazpacmn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gzlbjqoma.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gxfcqoxfb.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/getkjzjoj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gtafwmylt.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/grevkfubx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/grczdqnfq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gepldpdjv.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gnttzeyoa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gkujeqxfh.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gyasfzqrv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gghllhceo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gijjjfvrw.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gjflnouge.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsnjhyvhe.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gvvjrbnxz.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gnhnocjdx.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gqqrmvulw.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/ggpxxxegi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/ghbmslcou.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gqaqskfzt.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gzkvakkdr.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gjciptipr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gymrfuxjn.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gmncfuaxh.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gaysmukhr.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/goydbvxyh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gwvkwaxlu.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gwpweteno.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gbrpqgmyg.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/ggzemfrtb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gtcaucmsg.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/grlvhokfm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gjnurqchw.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gfpiawath.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/ggfwggvbp.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gsfplmuhp.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gwoycrgop.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ghshdlesk.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/grlsmkvdm.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqkxixtjp.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gypzhkivo.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gbddlddxt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/giqpgrsaa.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gwdztnzxy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbwmhojws.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/ggvtkasmq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gkrkacbdz.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gqgfehtis.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gzbhrqjaz.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gmjekuzgr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ghzzssnpg.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gxztvslxc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gzwcmfmqp.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gcagacjxt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/ggcfjgbgp.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gkxnjfkfv.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/goklpntqh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gwecueziw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gmelxntlx.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gygiofoeh.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/guprprmia.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gimjhvfcn.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gcnpenfwi.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/grfzwogts.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gpyjeoius.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gsvfooprc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gdpetmifh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gkvxebhfe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gmlxeiepi.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gnhgxqemd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gygwmnudk.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gwiqfoieg.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gwaokkusi.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gakjadwsp.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gxcospzcg.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gfwckmqas.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/geegqwydm.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/ggvtkezte.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gbhatwboo.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gzuwmaiiz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gbvbplsba.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gssyxrdtp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gfcwtkwdy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/guobjbudb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gsnznewem.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gwemvbxis.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gnzuonlcn.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gjjzsjugn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gfjlogfyh.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gmcvoxgmv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gtgnsewyu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/golbwdfem.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/guwwxzolh.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gepgdofjh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gwzuluygb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gazdilwgu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gyfhkfsri.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gfhecgtzp.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gwxgppzaa.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gkbqdhnma.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/ghjgzxukl.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/geaxfnpqs.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gohbutdvv.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gwcyplzrd.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gtqfxjyin.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gjrolpqdb.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gomwudetu.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gvlvecihp.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gdkhztofs.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gqeipapdk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/ghpijbbnt.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gbgrsbefn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gbkhxzegv.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gafxbkolr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gljuanmun.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gbqpsyhxw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gfwdfgitz.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gzjxhoiwr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gsxrctmxp.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gecbabawo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gaktgyksw.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gxqwayrwu.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjzumdrfi.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gflxgekqf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gompplowi.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gmzhedxov.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gntjjgjki.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gnjcvjuyk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gzaoprrni.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gjdggbppg.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gxjehzwtp.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/giitieahe.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gxgapzxaw.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/grrgprnza.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gjjvlkhre.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gcanjzsvd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gxjtlzvbu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gmvfoowuf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gkydggtwb.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gtncwdafr.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gjywfzupd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gleusxcjt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gshigusvj.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gddhaqdkq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gktnqacny.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gjuduqero.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gbofbhics.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/griftctrl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/grqrhehgb.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gvzmwqxuk.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/grpfygpvd.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gabljaeem.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gyohrfzqz.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gcwjzoiad.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gjjsfgcen.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/glgivqtia.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gcrwvuwsp.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gyjfehtal.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gtqjllwip.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gjqnfegwq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gjkstject.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gneoykidh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gmhxmsdtf.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/giqumqjrf.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gllpdtsle.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gwtfbbvei.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gastkhfam.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gpoitcvrw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/grkoglxzr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gavnjblym.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gkelgqnpc.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/genkepdbg.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gthbbnymp.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/giqpilmbx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gxelyshow.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gaharyrqw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gcgiawhkl.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gaesykwvg.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gfjialkzm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggnaochnp.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gqbdimdzb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnyuhwcmb.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ggokuocnd.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/girfmtlym.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/ganquywcf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gbpyxchav.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/genjatmrp.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/ggiokpvtl.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/ggsunuyaf.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gzcuzuquk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gbrfcaftm.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gbsootgzp.sHtML


<!-- 参考信息 -->