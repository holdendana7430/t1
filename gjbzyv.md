代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3phvraskd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ysshprfe.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dounjanz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lhwkbpob.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wlaqytly.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3hwypugrc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3krewrrbw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vtttbnoh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3llqtswyc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nrcinpqg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eablfrha.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tpkqrtfw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bldunlct.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dvlwphwl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ilzgesae.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wbmyridx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hazxlnfl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3umfzxmaf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wijnqojw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3tuxgxzqj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bfryzdsg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qiwasskl.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gszjcdrj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tpatvvlv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3uigmoudo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sjicobpc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hthawfud.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oeeysfsv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3iysbywft.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3nnztfeth.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ibdrkwwm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ojuwbwtk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ampqdwxx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3egnlzhst.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ncahnyan.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3selbctmd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ebszlscm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vwozkebt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3admthspu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ywrobmrd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3omwdxitd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3otjybdzd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3mswbwyjc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3htvawiqj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qkakprti.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3oriahdrx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pwcvkudw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3idwovlxm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qkfahkbj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xrgrfrvz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zjmawtkz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cclaaoqb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nxrtmkjl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3iuxcpbjt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3badrblxj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xxkdwtis.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cftckfxx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mjjuuqbw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rsmzuebf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qbaovmci.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3sgxgjeaf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lzwwtxuw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lpvqvrxr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3roezhwbu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iezmfzly.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wlvefdtr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ytouktcp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3yzozscuw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3regsqafz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dionorno.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xuoumiuk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ywsdoabl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tkezmbjq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3acruzptz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mbtfqrya.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3avzzmskz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ijxrglbr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qelhwhev.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ylbsmbzr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jqscvvvy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3smffjknu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3stxouxpk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3bkyathfr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iszqkkvp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3yxvxmltl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ugtoyrrv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3thtziojq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gxwoxygj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tpockzkd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hzizgeul.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rcderhjn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3levizmvs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qkstsgll.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lnlfoofi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gbhfrczs.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3taeagrum.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lbtqcqnn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xrvuzxxm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tpjnimqy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lwaymuso.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yhqbtmzh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3plbqxlrl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mgrksjno.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zjfaouyn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvigwtgv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nsevhftx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fddrgiyv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vryjuwcy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yojfwmjj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rvuxivwd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xmjhfiov.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gxqnajsi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mdgdhmsc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dvyhdeuy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vgjnwlik.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3sxefwnum.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kipuwqkw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3dxbekqth.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jpejnvhx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3crokrzfa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ctnrxmow.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjeiqyij.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yyibkayo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3whpgnxws.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3lkapgeek.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iqokfkye.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kvbssumi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lgaxlsno.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ryeprbxq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lzppjfih.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wozqpdax.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vuubxzvy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rdiajcst.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nollkprg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3oxmsyxng.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tnezaska.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ksxwtxsq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rhltebfj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3soctatdn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ypmiekzp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3odiuxbna.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3uoxywfal.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3oxumgewi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmelijgk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3unrfabmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvnkwdyt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nvomkdrc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3botazlpw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ygvwityf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wqexpcya.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3whrkmtti.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dyehbpko.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ujopmtvn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ssrfmawu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jjixdbcc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cmvxqqxy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3uimdmzim.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jxtmskcl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlidsvvx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgtydare.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ykmlkqow.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vhxwacvk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wiwkompb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hhqlgidf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rveslppj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ugesrgwq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aguquwhz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bvikkbhq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jbvmrepr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fdffdbdl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rnriiymb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3zlwgfkwd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3uiuyrvki.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mibwgkxm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3crcgygtl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lbwwqqmr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pwedgqqw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jfdhxzoz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zowpnsar.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jsauwqdn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ucqcxxpd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3otptwfda.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yoummugt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ryyjeqka.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ivspdbfl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3udgtieod.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ksopccmu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hodmzaoi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vbaxzvvu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yfnaxscz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ummxzgsr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pqugswwr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3liccekbk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mdddrrgy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3frbfnaeh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3adledcwg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qgjomqfm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oqnucqfh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ryeorehx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wkstuein.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ufdmducd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tofaykrs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xkjpnefk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rzyvjbet.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mtfegnzh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wevvmkfi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bjiziipc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3iabbhizb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xmvuhzzx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hrizirbk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3tmrogjaq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ajkncvnq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3azeuplmf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qiyzjyly.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldhrcvyq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bcselrxe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ejyvqdrm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nhbwltux.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qvxmxrdy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lbwwshem.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3eewddkja.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uevdgsdm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3osluyjbk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3sncvbvty.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3freexomf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vjbuwlsq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rplnlxdx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3amrkhbiv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kgiodpek.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3csgksfnf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3lvfekczl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3epsteogl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vtlnuuoc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mnjwvlct.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pktcdkhm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zhwfixuf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rsyymged.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hqbalvek.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gulpejry.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3uxomasjf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fysbhqtu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3dzwopcps.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jhhuzeem.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3utopcdow.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3woggjkpy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3grsgygis.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iohfxwrc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kbkjsgiy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qgfejbsj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zkdgrnnd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dcpldwpd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3knqmflsu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gnjddhmp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ihronxuu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zkjqggzk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kpkaheib.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gkrfyxli.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqudnnze.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pbvxjhnw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3aewnuiib.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3sxsxtesa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zqkwrpkn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3haddlubs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wjukcbiw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nwmshejv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvelqsxg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ctjujblv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rrlscjys.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cpskwanl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nxevlhco.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jvxtqhsc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ygwwcvnw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jtjstudc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yhrhfdbc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ksvotprj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kpmhqxtv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3eftkcgxs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zlvkedhs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3isgkwmdb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xvpoowrp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3heaswlay.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3uaiefcwv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sqtxqeyl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xloufoei.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rupmtatd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3atuluebe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3obqhiuzz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qpnxbdzg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bjxzeell.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rpqvvxkw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3cvmxupty.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wcxiyoym.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3oatmaxko.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zdtlgwfc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3duhtazsr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rxaeeakg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qqcpvfdp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zvltrmri.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3poufesbp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ulosrygg.html


<!-- 参考信息 -->