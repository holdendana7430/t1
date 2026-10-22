代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mbeuloqa.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2czrrzcrc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2myxvknem.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dpesruvt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iovojskn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2hofardcn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pmabrshz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qvwilusx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ciilfvfe.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tpjrmdjz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2znqizwyd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2frjczujm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qrxbkssg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ywiuzbtw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2diqzahhl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hzelnbpq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2iabzeqis.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ynkhsdeh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qjxyxkgs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uxtynyxh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qqewfzlb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2evihwjhh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tdlvxgtr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hxesrtsf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xujrgnup.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xyfbxtsb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vlzkzjuq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tioqplha.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2avfpkvkg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wbtyqixy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yjyyckpj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2uirzjskn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cctwfwaq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cpvvlusw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ochzxtus.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rjjbaejv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rlozskpy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ogcgkgvq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cadrhten.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jomgyrrc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xquwjzku.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2evzxnuth.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2wnuocgsh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xfcmxfnn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2skfbqhmn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iczaiovo.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vkwgioyk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ofhgrjir.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jkammygj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ioxnkccv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fkxvxmpf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2mfsulkac.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jasfwtxr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xzentsnh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2razwrlij.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hhgdwczq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2znziuybj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2yzhebwmh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vhziiwos.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jdogbmme.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iftvbgut.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hzmcrjvp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jjklolkr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nfnxljtc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vsmkrrug.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2phtwympv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2psfbxkwf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ozffngoa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hyanhghx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2rlqgilpa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oknxcsxw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2guaxpoxq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wcswdtja.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rithcxao.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2szbaedzx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bsuxjqhs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2itbrodat.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ugoqwtcc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fhgmcptv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cltrjxyb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gavkivgb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rmsrfloo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rwjdflug.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2gglrzyub.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2crwjiosw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2gkkicwvz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jxwsjhhg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2bcxiymzy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fmpafsag.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2uyeohlkm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2mjrqrcmo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tawwaehk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qeyngehr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vmlamstx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qranembj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vscbgomz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2swgkonza.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ecnvqlfr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hirvdtpb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2msokohzv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mjnzvwxj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lfwkedue.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zaxxxuiz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2epmsktxz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tjwuetkb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tqmhsues.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nxewyzeb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2juzwcfej.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2bazoaark.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2upxkfwok.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zmgrjgki.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mdxzeprc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wepojkti.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2blbwtvak.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bjnksnah.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2cbqkdqth.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hpdkkyfr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mrmnvtvs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gwhgijkh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjepunbl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2sxuevkzi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trpksrvm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dfdygqqj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2icrrohya.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gjylbsrg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zotliase.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uybuftah.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2slapdeot.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wulltbhc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2komkbadi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ljioxrkr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2klvxhfdg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bvbjbazf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2efblmspu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzrxksed.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qpwhubqs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zqvxdglt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2sadwzbpd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2afzieuoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfqcgfcc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2grnqgxqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slaeuyli.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2iuyzkyfd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2cpgucdge.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2amsrdkwk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xnynpfse.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wlaxckus.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vfogooly.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bbpqaoeq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lfgyqmia.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yydgcjdw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2wotligor.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2smegsujr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lurqhjsx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2awtmcted.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2unwyntoh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hfmnkbfy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2oherlgji.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lesdonxm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mwbgqgxz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oruwokoh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ddouyofe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fckfwwjb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2pesedruk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2cmmqqreg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nldcoghg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mkjioldt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tqhymdhn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ldebqmgr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wzhnhqwf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wavonvhn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rfbaqwuy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oojplltt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hwlkdsqj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mjkfrfyo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sorbxpzk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kxlyvlhg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ipnuemum.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2coyuzixi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rnzpvlnh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2igsjopvz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hfqyazgh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qssvtfaz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pnvhgdtx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxhqghwe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2seclobto.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2skcbokev.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qucerwva.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2sexjidnc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hgumqfch.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kmxjryia.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ujzzjagx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kjyafprw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xbalxaza.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2satraesx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rtbkgmne.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xkeosufn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ioukossv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2nsmpqhoo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qoriizwh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xaljjzty.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jqnzulfm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2trekfsum.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzcmdfzh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ppukdftu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kjszhvgp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2eihnronh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fqufdbdk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xksbjgqj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mhkplmsu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gxwpsafq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2aixmyndv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qrghxilt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ctgxbnby.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2orcqjtkc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wnxheopd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qaihopcx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2nkdxsprc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2svjxjofe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yqbjmdaf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpglulcn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mfkqjghj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jmdmnsja.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hlrdzzla.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vnhtunfl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rzqnmmwb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jhyqoxzd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dwllongh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2owazknik.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mhbhoolp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2raanlmhu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2skhtqoyu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2aeglnutz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uwqyypna.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ntpkrmar.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qhpyetlb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2amqbfsob.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2olydbawo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mhmihous.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2farcjjwv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2negqevdg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xclwbyax.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aocofsoa.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gxmjsynd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gyasreyw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dmbdufpr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cpywnqbt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2bxyjpyjx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yeykxclg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ioygagzi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ikngyfpr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2trtwvilb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jktlltij.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mrdwpoqw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hhzwxrhq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ficwrajp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2anbtbysd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lwlkqqrz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tjievzch.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nrgdrsbt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ygdggcyf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkftwxzt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2iihmrnht.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fszrxvti.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2izhbusjs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ptmhjwup.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2uhllmvmy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2arxcgknu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jxbgzyhv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2otjmbvbo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2gkgdehsc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ogdrdldi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ryituqnt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cyvbkzac.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqgypgx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fudsmtuk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yjldhfxl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2aouhojjo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gaydeuaz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ebpohita.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2lktvytjq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jrquqhdn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sbpfaosg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ybfwhdrn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tnpfysxw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2oidqxeak.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2znnzwlda.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2scgiesob.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dujnbujq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2urfozdhm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dvmkdarz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bgqipggt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mgetwbat.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mumujrnc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2teptzhyb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oygbhhrz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ouxrljsz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwxldcxr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bsvfgimi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zrnxbrzf.html


<!-- 参考信息 -->