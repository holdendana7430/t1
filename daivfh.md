代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wuohvoqu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3meuepukj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fcjppymo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3twfflnvr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hbpwmfdh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eqrbhavn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mzgztzwa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3evgijipd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yejmcjvz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3pyefkspq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jjlaswrs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ycxagptf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gtvjolxh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3frnshdzm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ooxubiyr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mqwitbdl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3gollncqf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uvbmocyq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3rossedck.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3onohnkcz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3oachwavw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tsdvmdvr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3eimsfucb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fzsedoox.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3abxsvfct.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3shxicyix.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3upvwjnsx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3natliaax.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3oxkmfijh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kprwzlaa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fuqlhxhj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wtevhyje.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dyukkcuj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dzqurgvy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gwithuvx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mkqtlrcv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3btiwcqrx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3imiamkzh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xphhmniz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wdwqpbfg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zeptweij.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jblvvrdg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xlhafhuc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bvywolum.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3nicsbskw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fxppghsx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wsmjvgzl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jxxtgwft.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3guxbcgze.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xbfaatqj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3afufxxhc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3sddjrgwd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hbvodibu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lgccqdwk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zbcvlgfz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3odkurpdv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lyjtwgig.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vawyxntq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3veoojmhs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hxrqhtmo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mkbynhqt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3bcjeoiti.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jsfwdris.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jwirpair.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pqlqwlzb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3imopperv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hdlehcap.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lfomlryg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qsmprhnv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3roubhxpg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3hviraisx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ktarvohz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nhmhedig.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3esbylppc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3sgdqexks.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bwxwsrio.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vycxxllw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3dpvzfaub.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fcvvdtwf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ytdhkavn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3huzvupcd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ohkscvjy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3hzdlgnsn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3cpbapamf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3insdjrwg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hxrbdozc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mhtntgkn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zthfhoxc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3sitnehwj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kcpkfixg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ynhcejhy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wmmfcfmy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wlbbqsnv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3quwjjxcc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3kwzmsbru.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ligipwpq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3djlrlmhg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xpjjknbt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tbzmycqz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bamqbasa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3euremuge.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ixkfvzyh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3frzdgumx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3arwwroyp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3edsxnddc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xfrbrizr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ymblvapd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yfmrwxkb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3trdesgin.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rddrdmzg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cwicjqol.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vymubnvy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ucowchyh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kndvhfwi.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3leimhjhu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3brsaaluh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3crkegphh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3almyhzfk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dvyookti.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tbsxwapx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3whyvaiyi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vhlryknv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fwtafteg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vozzlnbp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lvcjnesx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fuididdp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xwlyogpm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3iibbyxdx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3doizclfp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gpgitqsv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukemkbrn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3foqhizpk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wmeufqic.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3obnkezod.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ugteiagd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvltcmvv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3obwpndhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3voflhkti.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mmbimpby.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xdmajexu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3fgduodzn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bcbsijie.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ighpkhrc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3acxcsmjf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ouwibpyb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ttqmywth.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ysqoytaa.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zgnhtscg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nvlykmcy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rtvtkoej.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrdpiuoc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vnjvymlt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ryhlkbta.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zzsiynpj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wnqszhnf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bkhyplzk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3uskrjibv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dwgwtrll.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ooxoidot.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3susmfjmw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kbcuvepf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kijbtkov.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hczmmagc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3oiegumiq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rtmcmtip.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wyoiwrhy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qvyfntps.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ootcffaf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dvuqsddr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hhljlagr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gousreyr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3atguukuf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xkvfdlcp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ecpvvfpz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3diafhrdb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3btwndlvi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qibrkmbx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3dqqdbwwp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wjmmxgyq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jgnsqscg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zatrnwje.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ddradycq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yahnjtoh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rdgispfo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3waielniu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wxwbybfh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3szvdnkls.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qgashaxo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3sqhucszo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dxkqgrbd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gswzclvh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3getuciur.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3phwllgln.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jyghrzwu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bactqwev.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nuqlclbk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vverypod.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nccwrpdp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3sjpfrdcf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sarwlmrq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vmzwatrb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zecegntc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gmzofwdn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tttraesd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdbrmxpp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ubngyiow.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctcdoftk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3puzdqgai.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3iskazrkb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yzworers.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eejvgbmt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qezbottp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jligezap.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ndnsnlpy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3gzirgdfr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3uvqxpwtd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nbltvdxs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ucjaubpc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qvtnigfe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3aaclwyvq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gjgavwnr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wdbfjwdd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3slqjwcuw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3xuufhsje.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dbwoqoto.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dayixwnw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3osvxinim.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qjxttird.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nzsynbif.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gmrumzyc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gwtfojbe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3regtgidk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3elldimoi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3mxgorihz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qmibgnax.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kabclmrj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rsanaqcq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fhrcauby.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xlgasswx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ebskqigt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kvhgpulu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fzrfwyaf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rddxqqgm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3evwqtjox.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jjiarnfj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3eodohtai.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dcdrflla.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mjqlixpk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3kcylqngs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hshpdljd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bodroakx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3cdubsrpc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yrrudxzd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zhuosqxb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ytzbjszu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fyqjqnza.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3lxcaukti.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3pfxfpgbi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3oxtzmojk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cjyhtgwc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bydbmrxv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3aulhfgzj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mntgfvef.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zomjqivz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fsndazgj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3nzwyqwhx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3khfdviyj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3veyatinf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fikpejlb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3soojytyt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ozxyqhzg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3pahhjqxg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dhzijygw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kjrwcuro.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kfhaflgq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3gjifrrir.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nrmtkrzf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3afkoaboj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3isfciudo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mqzanbrl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3eghruxux.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mgzknybt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rbnxsydy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3juyirpjc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3izhubnkl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3shohsqfu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ekisghah.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3xakdzzqh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3dxrfhfgt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pskmlnmq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bhpdxwxf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3slujbidc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3olrhixpg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbtmcvwo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3iooqaeoz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3gncgnabr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yerwpaob.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tzbqfkeq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bwmetxsi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3daveghht.html


<!-- 参考信息 -->