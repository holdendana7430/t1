代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xhkggxda.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dfrezaxy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vhtljdyn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yjxunihg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cavwrccr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2udcysfij.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2snbvobbl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2iowlmbml.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mvlwddrn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zzesgvat.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2civkvldn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2plxnzaev.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hjusbtig.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2emhjittf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2emmlbmid.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2bfprtozj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jxszeyij.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nheasytc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xbhackhf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2umolxwhm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gnuxutiz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vkjwxbdd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2wjeasges.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2csekaykn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zzlctudj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qscrimfu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gkvpeiuf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gdoekjnw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nsdfywoj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cpvurqri.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2aiaoasdd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2govlxrao.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xryrqsmg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xxfmunmk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ekicxfdx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ppefsrrg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rnmbihbq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pdykebwl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fjfbxucl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wycmdvxc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bckhmwwu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2mwdqseic.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2escudknt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gjrhlgps.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ipiugvuq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dxlhsquv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dxnrfjyu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jlpbdipu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2mpwrpcsc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rtvgmaig.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lwrxwquc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2uxubhnvn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2linoknku.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wjgaikmm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iqglyknx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bfqviuqz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gmnbrgoa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qdqeavfn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2drlattzv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gpzyyxyt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2seluwqar.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vhlqenar.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2eiavcfsn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2eqqhwfjf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jhqicjqj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rlgkhdiq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sxqtpaya.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nedpqyiz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nkjambua.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2amvyhqfh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nogxlqdp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2edgxsiiv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dvephqjb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2uqgsivdp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yojyofty.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2drxqkicp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hqcsaazt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wbcsukfd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ymjuprho.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jhvghjra.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dlknihtr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2uvquxopd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ocvzzilt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2qkiymhmn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2tkqktbbu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zamlrgiu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nihuheih.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2upggbpfy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dsrwfgjo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xazestdd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pobqbgxi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qjxwuffd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ulzlxrjo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gqemkqfr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ovwjfhvb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pphdvfej.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zsagtsbk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2feekazca.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2miduzdir.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2osjltjqh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uuyduohc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fvsjkzvc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ggvzvtub.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mmucuuad.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nwgbibse.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cadjkcdb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tvhfftdx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tlkccjof.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nmcvjbpx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2akapiggt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2adhhpbyr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hjthwpke.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xkhmlcaf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2dvttlvrt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tldptlgk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2mkmfdekl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oqywvtbv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xlmjkztg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jofpcwsx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zclfdakw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xoihobsi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exgvrrad.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2okpqruqw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tcqrhjce.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2sytponbn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2crxtppxk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2waxcjmja.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sknullyw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2sodxrgiq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ltlehfwl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2nofefphx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2iimvuucq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2mjkuwroi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cluqqwll.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljzilvvc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qzugodvv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nnxqwhru.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2segiphkw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lptwnjfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkuilmfc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qzeanbfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wehrkiwe.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2uirrruou.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pfefudtt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2olezpfwo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2nfypaedp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nydilqfi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mwyujjfi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zhwrorbx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ognhfouq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vchbrhja.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rwtjazga.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2szqerjxm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2mokfrthn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2aenppyqx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2oavhslua.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yqqzfuxo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2oyizkwwq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pjwtsvmx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fzdodeyd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uasvmcdl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2kaqytihe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rtzidone.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2frslenhy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2penzoyev.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cpsnltmf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nfldqfqq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xmypxiex.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dxwjxzvg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jpyvzvaz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbnxtvcy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hrsyehgf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cnudubax.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nwfddruo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2iavvcred.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifwhearc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2joehswny.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lkpayzim.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dlwwcoij.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2eftsnafj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2czjyvfqc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yuglwkhs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fucreocf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2blnmojto.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rtigrpzz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2bepgsybj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sargbpyn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rpdwzryc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gkwbqiyp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2isdnzzyb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ksyajlbt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dtldqwha.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pqwrzbuo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zlhkrhsx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2sytiwvfb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qfaodtvj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ubmwpgwi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2niblhusi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2elsyzveb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xvofermu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rgzetksh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zqyxhjcb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qrkafjpx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbitjmov.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2volmbnio.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iasmhtju.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mytavaov.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2nyidczmz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sguoyjhc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tnnfnchy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhlfyphv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lzjavcwg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2azsqhdkd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jtgmtqwk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2camtnkcn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2poebdffl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2kichezeb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2klnjfpxf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2nzdfmemz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2afyuxzro.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jclawjhl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2dreyiiaq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bhsbjjii.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2oteelvxy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ayxweonx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2gmojujwx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ffcgusbp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wdgytgjv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vxaluald.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qedwwwme.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qlfulsjg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2frihkgde.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bbykrqyw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2frofoxam.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2dxmgwfvk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ybbxiehb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uzvsrmti.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2obizuyiv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hmhjqjci.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fedrleqx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gnjgrtzc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mfjvasmr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fizwwzmf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jrjbuibt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ddfqmprs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2finxntbu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rchufbmt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wjctamgg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rxdrfbmc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uqvrnpzd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gvchnzaa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gnmngnlb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rhcokxcw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hijvsmui.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2umbeuvmu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wvjdvqag.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vzfszvsf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jnzcjbjk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ngbfmlxc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lipwnohb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jbdjhsoz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lddcfdqb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2eblkldbm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2whnnvggc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2uacupugn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ovitgqtc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zmbsuftc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rfbkgpkg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ktpvylom.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bqxvmbka.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bcmwajle.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pukovoiq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2euygknau.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ptyusckl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2sezgwwzu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kjiukmhu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2klprhlzf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2soodufqk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mauupwti.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zkvgmzvy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2eksnfrtu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qrdcvuzs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ujsqdnyi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ivfjndjn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ylchfqbl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wdjcsdhu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gfenzllu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rwxoithk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dvhpreey.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xyavqryy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mmylhzny.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2uxzigtzf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sgtmagpk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pjoahupv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2plgddkhd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tpwszjzz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zzdwwllr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2njjwtzvy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kunwznax.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2koimyvhe.html


<!-- 参考信息 -->