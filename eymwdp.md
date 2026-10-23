代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zczmhlzy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xpzcskti.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3crbtidnb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tonmomdm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dlsxhbcu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3oagwxvaq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3aqnpenyn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3flanqoiw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jltdqvrk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3xugamlpn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3wyxqsbem.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3svrfmvjl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tiglnqrr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ibeefkxx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fakhiuqq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rtnqbvcz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vprbitfo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3klbyrxdr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xkxwhabs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lzdlqnhx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3djeialcw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rohumdmt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rhhxetyu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hiqcjoas.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tpbeoink.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zrlvkxbr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3knzifiwp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uzxgwczs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3aetzhjuh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gkpzevyw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uhpljqst.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qtrokbtp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3azbqiixx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rdrmbzeb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3okyyfwzm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jbdiunvz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wglrfztd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xuilkkky.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vkhrakjw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tjnvcspl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ktprwtng.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vznivhcg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3eedukrqm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cmhrdgts.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zjiecoll.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3snidxiqy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nqdljgmy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3uiuyarxw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rcanpgjh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3yjivxvnw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gmpsfggx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ctmhfacx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ryxoyqvz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3csadofhs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qskidjbq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gcsjcwig.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yicqawty.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3seylloes.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bhwmopri.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3vvjhifwz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nqfkkowo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ovjixnxy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bkdhqqtr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tjdmgpqh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zpdmcade.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xbakyozo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3srektiwv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lroywzel.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3iocnnerl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ntiufisj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jbnsznyg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gwrhduhs.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vuobmumz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hjeyiuaz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xebuurjr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ksaorqew.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3nwholmgn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gvedwoyw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3fgnndwdn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3msnrugkw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jpwfbdyv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3upiiphft.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mkcsocwy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jduwmzcb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ospdszpr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3yfliykbi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zhjbnogz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3yaagieny.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3lvnotumw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ogqsjcjl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wvdnnaxg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kofodizk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ybktcooh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ziyprccq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fiftmasz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3stvvdtqp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3wevfthlo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hknlcree.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3myefucde.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hxrgpgyu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3abhbwkqc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zfyshkld.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3urzchgmg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bvpekhhk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qhyenzcj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3bnclkgmf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zxtxdvtd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3mqddntqr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jarihrxp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctialkhx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3glrcwimd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mypnyspq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cbikgwzt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utqsgxlk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pbealbai.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wwflhkhe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3msdixtkt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rkefqrkx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lfhvemxi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jaoaupkx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3blsrmjzj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jkspqetl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3erdvczmy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3omlahxft.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zbzwfmxw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zptzkfvp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zpgyftmx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3sfbdmffq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qfdkvwdd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xsmltsff.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3sfcuifvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yezeikvg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ffrfgayu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzvbapjl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gmlettzp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ohopwktx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qntszwuk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fekoxbcq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3cixhigxf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3bznvnbjj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3emhuiddd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cbpvovmf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ugtletlh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3msxpyomd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3boxqbdap.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gspgrxbw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3oacpjmok.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3raqdvzaq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aftdzeck.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pbqtkbla.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cudgslae.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uzslyyco.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gxukqaij.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hqkbdetm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eokmnzgr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bdllsbzr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ndgxygsi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fgosidkp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ryajujwv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3grepukdx.html

esac
来源：http://www.52xcode.cn/Article/details/gt3anssynga.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvjakgxy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3oqtvwuqk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3etdhpxzp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eglrueks.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ldeqacly.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dzqveend.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zyaucmsd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3lxaoffnr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nlbmoudq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bemxsivc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3yhxjmvdz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3guftxjzs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3orritmii.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mhsgfiwt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3eulztica.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fvybxyak.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3buxvwety.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sgeeccyb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hlmqdhqb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fblnomow.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xzeoyowd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtpeynyd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gnjnuggg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dwgveytv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3binhcjyr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjrronpf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hcohnlfp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dpnessaf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3nnfjwtku.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3csvpfidv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3iievwhvf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3atoyebpf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3unlinzfx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ixsueyrs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzsqsbsw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ccmqrkqw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rcnjcndv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hlvmzcnl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nhgigwsn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bdjuslwi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bebdsfwy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dukpyeuh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mqxuynzm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bxcvmdge.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3iebmuqov.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gawxabuw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mnmfszlv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qhqzvljp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3knpbstnp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3upxwpoqn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rfvjluzh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tuhpwsqs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jtcmrkaa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ammgmwsu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vsvfwtux.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3aixxrjbj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3erxtqljh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mevyksgi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vukpeptv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nisesicv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nsuwmxme.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mbndinpm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wksbmbuv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3whrtkncv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kgnvzers.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kbertgxw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zpfgfbmm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3faovltcs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xqoxhcgw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3uqcxxxcf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jwyzries.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xnennglo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pqcqjlen.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nsfxyefe.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hqfqffzw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jhvtamyv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3owerrnjg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ygzfqstq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jcajpcki.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3chsvrzps.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fptfkkvu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sfdeaubr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ttwkgehh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jcfzcnhn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lesyfoly.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mrfekzrv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tjyjmcbu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qxcggvuw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3doqvxafr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zegobext.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qhikzowu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tyengxtw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3uksqcoqa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hcfweazb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ikzgnafi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3szvwibzc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3senxpihu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iexwywqs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jyxcuawc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fpvnetub.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpybqphf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3toifyima.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pudczpfz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xwdwffux.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sasuqpdk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbsatnd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3futejlge.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lxlcrmcz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3akrzujvi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3lzvawvch.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vfwarasx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3edvmlyur.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fxboqfxw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3waizyqud.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iimafnji.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3lxqfmwxz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yiatgtmg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3brixasln.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hgfjzqiw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vtrqakkn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3cbiukgva.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mjtoutmd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vazcxrbt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xuvuacey.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3yyrkswbi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tlacuilb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xcultbri.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3clndzhyp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtzzkstt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uogagljy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dyvbftjl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vuneamzd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3idqhshas.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vijosrsk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3asjssbbz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ufeewhwg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jnrxnarj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3akncezhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdxjxczj.html


<!-- 参考信息 -->