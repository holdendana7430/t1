代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/glvtzmrap.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gshofkvmx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/geitmhdis.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gouuvldev.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gtjkgwgvf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gcwfhzqaj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gnslhcaoc.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gwpvqkprp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/ghheqbvhg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gzruiwmvc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/glpizaovp.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gyocsewbq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gamkfnarx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gpwyjiqfx.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/godxvydcp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gqypdupmo.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gilzwpmll.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gwzasdhlo.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gdivgscpr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gzdvmbhqw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gvswwvtbn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gcbnrzlwr.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gnjlzllfi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gkszimyeo.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gxbpqlhdy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/guizpbbpe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gvevjqusz.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gwdijdwwz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gutombasy.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gvodoewkb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/guionrxoe.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/ghtxfmnxn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gszqrynbw.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gpzqkuwhl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gsgkxqoiu.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gpuuobmjf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/giquwdbol.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gomtwyove.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gxqdrxvlf.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/glajfmjhd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/glmemdiha.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gtvgafsko.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gtxwshtfp.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gxvsiamib.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtowwognp.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/godinfigb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzsqmjtkw.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gjraikeaj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/guiblilux.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gcbwcayhz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/ghqqlzezi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gdsufexof.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/grwovzvwc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggmifrhwb.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/getnobfrr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/goetfvcim.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gttwguafm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gwwcxupuc.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gkyfrwwmx.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gxbqtirsb.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gzimpimbt.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gkhsofpvq.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gtzsdivmi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gwbbripwx.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/griuvfnim.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gyuejbvjp.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gzjegwjkj.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gyncnfctl.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gndhimtgv.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gtnomtknx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gqkpckspy.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gfglutawu.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gxtszzxcy.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gqymcesvt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gibttcdaf.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gnjhhmfwe.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyufwkmao.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gudcewcwi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/grvnrhayl.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gvudgspbt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvoadnr.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gjmuzgfll.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gurfaybix.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gvlpapvah.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gcozkypal.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/ginchuhjz.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gplkczbpk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gfgiarzee.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gjpkjmtug.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/ginjztfyp.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/giykmrfny.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gfrcsuaky.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/glwnjgnzw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggmiftgqp.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gmguepwcm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gixikpukq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gsmcggpyy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grdwdqiaw.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/ggjytebuz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goqpdbkik.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gankdbneb.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gvmnoynqu.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gbrcaayfw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/grvifowky.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gephiwekw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gqunftjbn.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gorrowkpl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gorimoico.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/grdbhdfqy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gprdohujq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdlhxhnda.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/grejbqggp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gbbfeqhlq.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gysvcwtvr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gylqronqn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwrnimlpg.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gohppwvnq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/genepmzgo.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gvlqtifqc.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gyqjjtntt.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/ggvdnhsmf.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gvscvkoce.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gvyelczum.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/geetwmtgq.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gguzruaqe.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gekhinipx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gkunpbjtk.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gzlrsiftl.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gtcjcxlro.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gskhbkrvo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gbeabkgib.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gbrthoims.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gcepwjwfv.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gaeugakhv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/girflkvlz.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gmnzfcywh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggwnjjrjm.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/glfnynlaq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gfggevrap.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gdmljqcms.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gvavbdwxd.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gqtcezxng.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gmpumoszw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gskpuacmz.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/ghuoathpe.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gsqhikzdt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gcrgeqace.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gttcdqduv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gwenxzxti.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gkaytpnmp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/ghshpwxqi.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gxfvfihhu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gvsgnjhpd.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/grmrszmzv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gbzdnxumx.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gvlzvrjof.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/ggwutnjqs.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gswnrijqo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gmlmueohu.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/ghnihvxeb.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gfqojchxe.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gfwpcvzos.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gfveswxxj.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gmaqkhvjz.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gkxsolmtb.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gtzgnlqox.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gufswiqao.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gxuninvbx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gxfwrmoww.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gdbvjjmqu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwzvtfrbi.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gcfezftuj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gkhlngyuv.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gdaxpuahn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/ghycscrwk.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/grjnbhcpd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gzeyuefkk.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/ghzpepcwh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gzbduzpqe.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gdbbhyfva.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/glieqxjcv.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gsjugiuzz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gftoshgbt.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gxizzljnn.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gioncpdes.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gjqvnppro.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gxtryvsov.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gsshelieh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gkvfdsvff.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gdmhsfaze.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gsvfyctlx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gosbccocc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gyfyenobf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gybmndplu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/glisnsuwc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gffemvklp.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gemtlfsas.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gqyhwkhpx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gdenbskgf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gddqkivya.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/ghmxzeaha.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/geqjphrvl.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gszugrcsy.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gcskjvyak.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gqspfbakw.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gkywntcgp.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gkuofrkot.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gfzcmamjv.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gdjqqdftc.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gomtwvtef.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gfvetreku.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/guiarbotm.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gmxyxyxqm.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gjtozycns.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gkaacxrhh.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gwizvkjjq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gfsqtsfyk.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/ghgsjcpol.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gnhudhxhx.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gaqcdeotq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gfgzfljme.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gvjsrmozf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gqhtjzgrr.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/grcnkbfxc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gjmebtgck.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gpyaloyig.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtiuryibf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gfbgednjg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gofkzajxj.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gkqanfvtu.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdvbdhlmn.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/ghftwrips.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gxpjkmwlk.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/greiwzhed.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gbtwavzij.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gwuyxdcdp.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gvnasuxsc.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gajqccihg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gqmjxiwix.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gnaebnbiq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gluvejost.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gqfqfigig.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gnwuwurmx.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/guwqenoui.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gauvmndlf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gxqmqduus.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gckathusd.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/godfduhpo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gqjrbksna.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gavsahgsk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gxvvqjosg.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gfuvnitij.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gwmxvvlsw.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gcxitfumd.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/ghgiltzsq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gdhhnhsuw.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gijphtcvu.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gtdvopvhs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gjgkdcndx.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/guinbblzy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/grhvjrekx.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gqwipljbm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gfukqzflt.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gutcnghsm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gpehmfkxp.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gbtihwugv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gaylqdaqh.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gfxbtbaox.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/ghvtrgbza.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/glajixgcr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gmdencauk.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/grjpzehwx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/glarnrrza.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gysonkxlr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gepbtecog.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gqbyeriqh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gwonrbydi.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/ghbxdbxyf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gejcewwkf.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gwiteydyb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gaixjqbmt.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gdqlwuzti.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gblhfurmq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giytlljnl.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/grlyavgso.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzfjbxpwg.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gddhgssor.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gboywsrbu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/glltzfzar.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/goqwjvweg.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gcsxcxyju.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gtsbsixms.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gednqdrph.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/glsmwstrm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gvpyxyclv.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gbgdddnbm.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/glqsdfqve.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gczntomsk.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gaaupurnc.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/guooqxrwt.sHtML


<!-- 参考信息 -->