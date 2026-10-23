代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rhojuqga.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3akfcyetl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aaqmeglg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jnhuyhmm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3sxakwzao.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iikklxkm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hibwqyfy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hlofhnfo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wvwzsaqs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yatxfbbm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ywcstqcx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yocmuuna.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ccdfpgmv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fzwlrrtb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ffqgnood.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vlliooas.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ruwnhexk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ehsfnybr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pdxqhkgn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hfxnztbg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jelnpkzd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rysadugx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3hggverjk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gnunnspr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3drbybsrs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3anwnjwmk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3irfctkzt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3prbjnjvy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dmptebsl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bfyoobnw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3poexxpty.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rovkrqmr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3osydbtew.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3namkfvjm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3esfpkfid.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3yohbkrsv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xcrizzzk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fkndvyyi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pkvrsuaz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3efgaumxs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3sxekmsmj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bzvupzzd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cjsjwotw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3bkbhgfwf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fuekeyky.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fuzrnahz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hyhplbxf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3vdwgyzzr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cgqopolt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bfuyttcg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uutervmz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vrjtugzq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yzolgkwz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3brgjzjaz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cgwrwwys.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xftnpuro.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hmzxevoi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nywadqbi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hjlhpuyu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xyrjftrc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fjiqbott.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dtlyewmk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zcnrzryt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ynfgyeti.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3imwsvftb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3yprbeler.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3awtsprxf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3athdfxsw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pheqadyt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3bwhjhevv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3tmlsxrzr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nybciukh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3eaykcglu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3helszhxa.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3mqtpzdln.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3slmavppc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xlddmnht.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cnedguef.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jjyfyrwm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3nxlljrxj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zcpcvffq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3iyyfijwc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bgrdqohk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jmodrtlr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3iwprwwsh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mmqvwckq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cqmwifxp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3cbabatso.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3dqiszgdp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3fbstghin.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ziknfgww.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hdnerprb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3oyczwwyd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3epkhlijf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3maailxlm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3flskdzuf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rjxtcpln.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xddpejru.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3leggyiza.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uqawtrwi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3lnndlslp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cjsmbchx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tiunkdoz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wcqenlrn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jzkbtrcx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3swpxldqs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ovkgdmol.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bcnlomqc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ykkuvgkt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3glgmjcpv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kfwkpzng.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gfixqdmz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pfrpdqia.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aqddbyrk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dqvzualj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eblwmtwo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lpcxdvdd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eotutslr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jocngggs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bafhijan.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hhulkwxj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ecgtlfim.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mfktoqyn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3edywgark.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mntuvskq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nqvosfkp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vigyegex.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3yorcjcuj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uartinmd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jksgyzpo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qvmbsesg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fmmvwouc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pjucjdgq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xdjzrhqp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3spydnbtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofcmpqex.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yxspmjjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcfvoabu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3zwjgcewo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3uqezzfvo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3dewtyqwc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vsgjtamy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3cmapifap.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3illqycpy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3oxzqgibh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xpanvlzp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3npajkbsj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ymlqyicf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wsirolrf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3szvxjnse.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aejykfzj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3evzinzpq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3fxdogwlh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3aqekomms.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xtvsldcy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qtxajkcc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ibgnlyom.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3cfprzhxi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jamykeug.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ayyjqaxb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ghwaoajv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3oinvpoiu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wxzabxth.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fvejnjoj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sdkuzgwa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3amdnpxzn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qqxsmbka.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ileftjqy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hgxyfykb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gdnmglak.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qyorllfi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vdmoayqe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ukxxarea.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tgnarmrg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fsumowea.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cttyuwpm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fosgqcgw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jsgghpvt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ygapkvrv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3egwhnwev.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pxbxrsdv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ygofoczp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ljvodikh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yrvmuzuk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvfxuixp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3imgmkkhr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ezdttonw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lituvkuk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3eefoamyi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3azulptsp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3omxwkriu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nufxtnhz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ykvevuvz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nayfkfyr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3oqzqifqt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3dtrzzlmk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3htamedes.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hfxhodhp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3htjaoevc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bedyqihk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qbhzhzjx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qwpferdj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ljtrenak.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pgyujtyb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lruvdzrn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3njlzcidi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fspkbdut.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3myemmeur.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3lyypuqbw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rnewbahj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ppdnqdjc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ynxrgrwv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ozihbpqq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3awmtkpsj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3krijndpv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xdhpxewt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3phcemaya.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kamwcbdr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xkzkyjxk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rsregixy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vmlanwyy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ioiqstoo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hncmrppx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3iyqyeubs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3guxadxjg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jerrfpvq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cnuuyzab.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3etskkeof.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3smndhdcu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3yforsrph.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mkzvuxtd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bhprfuth.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3hmiatvkw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mfftyulu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mbznontk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3nrrvqbay.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ixjiqfed.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tytgnuqn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uralvret.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nirjkmvf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dnmpyplv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pzchrlyi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kcinwwxc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qjaljjad.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3tnfcagwz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wwlnnkxg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jnsadhlv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ugcrfjsa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gyhyezhv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3pgzbikev.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3niqfiprs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ltitpmvo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hhlelgmf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wjkeemdz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3phmjrnsi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jatccqxv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zqewngee.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcbivwws.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jrhvqvyn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xabwqsse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3eepptdwk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lxpzjeau.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ureetlnx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mgqgdoam.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uiitjqyz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3koeekwpn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3orrmnwcj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ydlfxacx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wmqlwnqg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3oupymlcg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3bgpisjzt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3njtaamfo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zdczjofk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qyftkzgg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3idtyiqmh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3eezxqvex.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vemnituu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wvzlssgc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hfcrmatm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pduccoha.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3opvhvtzu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mbdlfvim.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rpktphza.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mvdtstyl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xxpdyyzm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3dxrnpqqk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dpocarnz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nfmtdwqg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jxtekedu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3eyehmvmc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xamwcfbp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3znjmbizj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jvhtcjtc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rbnybrgy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pvvhzjjj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zxvqtfhf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dpoiyklj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3frwyutug.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmniebqg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gcxzknmy.html


<!-- 参考信息 -->