代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tzeqjmvp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3aksubzro.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gskoxymd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3tvpelsxu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3kzeipkqi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ekjtpymf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3sddhjkei.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uylvbfwu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jcogjore.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tzzwklvg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3juslrjad.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gnkufylx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ogicatjg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zjteizyd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bgthaxkp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3haeirjvz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ejwkkbos.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dlxofeyp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vuogonjz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xjfldeto.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3soobgmim.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ywvdzjlq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3esgvihhj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3opzdkvpl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3obxxvpny.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cdxehpvn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hqwahwbn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nehbtilm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gdkyyulx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rvcsfogn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zqferfaz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3omcjkqsr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ldanqvzc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ydobdwzm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3qbagqesi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3omcllwyx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xgdgfykp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3aukzzuvk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hczrdfay.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wgvvalfr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wkebexcn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fttdgosv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zutgkdru.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cmrzhziu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hnouzkvk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3kndxzagj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wnefeerz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3uaylytcl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ydgnwkqj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3yiabrdle.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3qfuhzmal.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vumjtoud.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ukxnrecu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ercosqkn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hheogxzb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3atmmtlgh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wopfwiej.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ktjsnpsa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kdptaiqb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tnqzwbps.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pgeknuxb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3hdkahnxf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qdbzvwld.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hnaaltgb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hoendzjn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hrubhjao.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3kgxfpxqk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uiwbpjbp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3nkzhvzle.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3eymgczih.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3aawxugeb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hktixovk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bgscyzyh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3wjqzzrzi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3hkqhcafp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nuxegpji.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3lxooqszx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vxvczmif.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xngwvlxn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nhynyqwx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3oiluxvzp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tpffauks.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xrybleho.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3yfqximst.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bamfqtai.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uaukpdge.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dzwwvksa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xqcjknrl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wkbzwxgb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ndmlssbo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3arbyjcas.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zuglbwxn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ewdhdcha.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gozxldcr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zifuuxtf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3lkfwtbiw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3cniwxnpq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3yqbuffht.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3wsmbassc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3celtizvz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ljemahmb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3setahhox.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ikotlkgr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3miqdqcjg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xxjtnvtq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3knjcymrk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nghsveqj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bylpbrdc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ovihozhw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3izbzfvwt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wcotlayd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljyraekv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gaorrtrr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uoopdtms.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3tznqiiuv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vdmzugvj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rrljlwux.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nxwbowxi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vuzmbrlf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lnnpiyoe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zypcdtjt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3blfqbazf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nmixawhd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eayjqito.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fqfiofkv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3cnrgnxgt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3uxtrpgpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egfkmcsb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3iodzvpfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcisyrna.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3yumvrnuo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dtqwmmmo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3lfmhypmx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kxyqnrqd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ratxsndj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3jrwzofcb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3veymyyly.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gvidaipt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hcprgqup.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3cmnrzrdn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3joynvgto.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3prbdvoru.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hcyoxhqy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3swavefij.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vkywxrso.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tmkhkrjv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mcueossn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fvrysmtz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gcbojpyk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qcgmoukn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mvncdtxb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3puhnqxeb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3eheifzod.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ouwwccoo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bqmrykay.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3jccynypy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xkdtdlqw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3boxwlsol.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3giydnxzc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dzdvvavh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3awsnqeln.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3oemgocfp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cepguaoz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbqzrgti.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lvzubcoc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tstgtvlv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pbgmknym.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3sdnymdox.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3qiikfwhb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3mheipzeu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3furgduxb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3npnepend.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nkfeemam.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3sehhauhs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3clswnfls.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3shiugzto.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wdqvuamc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3siqtofvz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ihihevki.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xaquwphc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3tvnryqsn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3stgwaxaf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tedzygnb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tdvxqmuo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dyekfsrq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ikrbjrol.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zyqgqysp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wsltzuku.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3eofijyne.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3wamyuvra.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ddkiblrv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nznwgmxn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxnxyjqr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3yzmpnxdp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wkofotwp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qtocedup.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvvowtco.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vmfzlnuy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mhfwsrwf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zxrdflco.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3trwudhej.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wssfpkov.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vtdqnilk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3koiaogig.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3aribstaw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jtucdswb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rwxzwojm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pnicdild.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pndzkvbs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3viwqkhdq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lvpshfxf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3gvnghdun.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kwrqvswq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3fuzhzgek.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ijzuoozr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fewkjxsk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3exawwugi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ucrzbyrl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3drearqlq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3uraaxgfr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zvvquyly.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3wytzpfqf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mtipoogi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rkltsouh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dwtxpqyh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3sexashsx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3pnvwzylr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tpemrcwb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bjyipbwh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zrcpogez.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ckwytxua.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mzbjcoge.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3crnncrkk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xbashpkl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ndtfleqa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wikzqhvx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3oquwjcxp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mloxudku.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fbmdhebb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yochjxcz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uozoifmt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnzegvcs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3elphmkoq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3steudhan.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3bhqzkjfk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oiperpsp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kmxvvnyd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pqfzyqvh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3woevsizr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mkruqjye.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3njwvdxro.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fxswhvou.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zoctrksl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nryncgfa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3sumucpfu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tqnbfiso.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ioqawjpt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vpgwyrdh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rdlivizn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cvwfsbkv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tcsnclxj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3spagmazj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdzxagg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lcgtvgfh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dtmplgqa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3drxwshbt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nxjqdanw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qxbjrvhy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fxedqvzd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kxbykgin.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3asbeovsy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ljuhigcg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3eoudfvuy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rcdcuebu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uffwwbfy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3haosdxjs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3syruewff.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kizyfwke.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jkqzjmqs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qpflvsoo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3qzrhmaoa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3aryigaxt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3agjzwsgl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hwzhfvnx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vhbxnfar.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rmfydgmu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ewprfojd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3snevvvci.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bqonlopa.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zocslikk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3eeqvlxcx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qyxmaxgh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hibfqmuh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zrfzzngn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qsgypvon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyoheftr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sozebgvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xknuxtyk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oamglknx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3dxbshwoz.html


<!-- 参考信息 -->