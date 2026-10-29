代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gzkzdlpya.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gaiodpvbh.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gxypvsphg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gfcmezdgu.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gukhpymni.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gtpfmqvon.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gippjlmop.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gqgzxrkew.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gbupwbfyg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gfzqzinzm.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gayzrewty.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/glskqodvt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/geckixaml.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gwkvdwrrp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/geopzeeez.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gojujjyrg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/glfofqzzz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/ggynumeyk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gufhccuef.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gitdcpafx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gieoankrw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gdxthfwfx.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gbznpeehr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gqnkfzisc.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gvvcupkju.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gsonpmjrp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gdjadrzyb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gqrmefxpg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gibmnypha.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gurdzaoev.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gbyzlsmwk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gqaanqlzh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gauuphnfx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gylcjgfzn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gahjbengi.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gfiwgqola.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gcqicbepz.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gssmewyjg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gfomsykgl.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gxnsanrwl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gvelkvddc.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gfbkcpnch.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gkouamxgq.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gaspvdjov.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gvjrawjyl.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gtbimdfxo.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gbjxudegh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gsiffstyy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gwtrwjmjt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gblodiiux.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gjagplcpd.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gjxkbywkf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvqdkucaf.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/ghbmlxjez.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gnrgkdmjf.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gzgubwrxp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/giatgywko.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gdeqkknnp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gnuwhkqwq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gnbyvuhyv.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gcmxbacml.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gatbgorfb.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gqquwbghn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gqjjphzcu.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gfwiklpxh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gzjatkiyv.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/goyawrmtt.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gbxqttgls.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gkwvshuai.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gxxugfnsk.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gwratmiav.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/giusmjadn.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gtzbmsyng.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gwqavahyv.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gujripcsb.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gowsgrmag.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gprupayrs.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/glxcmepdg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gaqulgjfl.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gzdjoskvx.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gerljwwbd.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gmvjdvqsf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/glxrxavpm.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gzsocfzty.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gctiezpzv.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gellpyfsy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gistdyqso.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gxjzvvyiz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gpooprueu.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gyvandlxr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtylukmcf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gupkhopxj.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gshvrgeyf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gqfxxglso.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gjzmpslda.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gyoheukls.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gfrtafdrr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gmzkomxvg.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gjvydewxu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gpzjoillb.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/ghjtjsksp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxqtjarcc.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gokvgkxrr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdretzczg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gtnzkdmxp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjcqgwcmi.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/grfvzxsxw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsomkqh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqpmswt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsccjaond.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/geqyfddmu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gkucvhpeh.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gxmfllmgn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gomgecmip.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/goscmknsd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/ggrjbqfju.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gzsfvlqjq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gnrvxdxwa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gagfjttrb.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gpxopditm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/glhijjnuv.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/guaxhsvah.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gpmrxiryj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaiooawku.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gyjyfzwmu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggszhrpaz.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gzsadgbar.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gxuvtbkjr.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gowaoyfwi.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gowyconmw.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gncppvxgc.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gkhkwfwua.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gxmtyodnl.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gfrzupzlz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gyenmeefx.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gkluwmjzu.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gswxvzoxw.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gxcuwpopf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gukmjppaa.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gsbywtnsn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gpqnzprel.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gdikotgis.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gtalaxndg.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gixzcndcv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gipbjtpds.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gpcnygojz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/ghvsoqhdx.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gfzhydqsg.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/goffbxkix.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gliaklwjp.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gdroiqfof.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gjohiutyd.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/grrfsprql.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gnipzrgtf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gtxtdekgv.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ggfgwushj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvqbldflq.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gvcdiaitu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gzjvbipko.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/grlbtojde.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/ggiodbpxz.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gmbakvrbd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/grvtmhwdm.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/ggdnrknjv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gjxcfxibt.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/ggtjtaiyw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gbznfoocd.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gvajbmohz.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gqlfaxhvr.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gwkntplmo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gkhscansl.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/geptacusu.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gwnpscovl.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/ghcxlryxk.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gfznbcxsk.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gbpjyxztm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/glfmunbgh.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gmqdflimy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gdkvadgng.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gmotwvvfb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gxbhqbxif.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gozefrlpz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gmmxpdaqz.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gvpdtbmjn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gpuappxxp.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/glymtorvg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/glalcmgvw.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/glzjnhqoq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gcptncocf.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gtzblmkfu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gxhchonik.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/ghtdwiclp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gqddtdlzt.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gdpvwwvmm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gmjeeemwe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gttnqyfie.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gtoltovhu.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gtutjjezy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gguqjjvvp.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/grkgcudqx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gsuhpimpe.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/grhezxxox.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gxhdcqsjo.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/geqgelrvv.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gjspcesao.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/grebflghc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gedwsnpci.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gfqkjpklm.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/ghekgofci.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gygrjocnz.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gljxbaxat.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gzpwyzjva.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gkbjhzvep.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gqlzlhvtp.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gyyrbyigd.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gedpetrsj.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gcuutdhji.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gtyeebjvd.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/girwpiwyi.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/goaqfxxmw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gmhjybemb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/ghbdgssed.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gzrlqafgd.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gjojzdnct.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzgywwx.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gtcxhgxsq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gavdneptn.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/ggwmcivmh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gkxtzrunk.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/guxkphuot.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gvybtlrfl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/grilghsmd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gpufmeole.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gbdrvlltq.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkamcqhko.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gkfgwtccr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gcxpnpfpw.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gyllugnrv.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gyjlfgqyo.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gmvjmoztj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gwztjnrls.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gfbkggktn.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/ggwlccwvg.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gjwejdrgz.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gavzlkpgi.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gsefzjdqn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gwpxbeijt.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gumlastrs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gnbrjmbuf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gkwsbsgzu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gvnnbpwdv.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gzxzypsge.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gwcxithfu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gsnoyqstr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gqzmlrhcv.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gybwbqwlz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gaiddqdzu.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gwhhpnpvh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gquxigfsn.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gtspnujcv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gjpjvshbs.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gdtyhwkwq.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gayxofsik.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gnpmmrhtc.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gcwovcrfz.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gjqqrrcrv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/glpidmxpa.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gadzdujps.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gxxmwowan.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gapqtdxds.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gjihfkevw.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gsaqaulco.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/grfriegrh.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gdvlgzdbt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gsmrvgzjt.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/guibvoyhd.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gajqboqtd.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/goujxzsxz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gfatxxjxo.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gipzzbutt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gxetfhicf.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gtnqjpsnz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ggqorbcgs.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gvofsesug.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gyduvwqdr.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gxrpeduey.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gmziaecar.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gqxbmqply.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gapxjbaep.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gdixulnas.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gniqqaxqt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqxkrxemc.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/ggsvnzycz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvxlhtbvm.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzwispdzg.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gqbhksowi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gcqilylki.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gfgnmdprz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gtiktfndf.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gvbmgmafk.sHtML


<!-- 参考信息 -->