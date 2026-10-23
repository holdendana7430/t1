代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yhgwrcvt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3eqoigowa.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fneffabe.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wnuzjfjy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dqbtazgw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jercnmla.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bupdodbl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dqkblkky.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3geesrcdw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zbapcaoi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nzdihets.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hyqlysjn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezzbzqgn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ioccjesg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yabejldd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3eutgawwb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bqjqwurv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3acebechh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xmgawjxh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zruproya.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3iablhwhu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fcbrocxf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3dfhhtjug.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3nlreznkn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3fvkxcvxx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3iiiugemy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3muxtxurb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wklovhli.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rqrttljn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iaunwlvh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3knyxsggd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bksdsfyc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ktvbswjw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qmkukzbv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vcvivqsu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3czttxhvw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3efszkigp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hhthkwgr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kukujfug.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wrkacxrr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3psobdgyl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ocnjudny.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xqcdyrlb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3skcgisxt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dnrdjxoh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qgjpyxqw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3moacmina.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bchumdqa.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xkpowavs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3udosooet.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jzdsrexu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vgdhcuqu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mbkveomz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vjzoodnk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wgbythhs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uwfwhkbr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rgghtdth.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3rgaxkwzx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ktcsgnbm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jgyysywf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bghyhyee.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wadtjhcz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cziaoiox.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xxupqtwb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vkrenibd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mtikiayw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tphcxlts.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rhucwnwx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kksmqdat.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3dftljhuj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3zfiwctfw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pisozlld.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zrmpcpqi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xucucacn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qgvpgwka.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ciepfwtl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhnuwrls.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3haszqzyh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ybujqeme.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qzndjloj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tvybadxg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gwitnncr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3svttbqai.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qzmxtmrb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3dmtqwtbj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ldqoirzg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ttqbmyrh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xtuxvkwb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hxfwnujj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3pblvmomi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3nhjtojfb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3akqeslcg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bqwtdzbe.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3wugeprad.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ngzotxqj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vdctzslk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ifdabqin.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3htsvoqwu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fjamtqgr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3axjvqqzi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vdaslaci.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mjxmeilb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ukkctwek.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3npipksri.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3pzratvof.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ndxzaauy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vloacsdp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bsdfmipp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qgtwichf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3krjjdpsr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3zkpfhcps.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hufoilrd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pxixyeyj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rekxeduy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lrpiimxs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kiovuloo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ooblxeuu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xfomwfjd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nrnolzub.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wrdrldva.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ogsqinex.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qcvppcoi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xinmrstg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3myhzzcgs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vuitiyvz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xqzvcxyg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3monitibi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xmmyzfti.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vuezekzc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgeyjyik.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nzkupklv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fxhphzyb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gjqbpcvm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rvxspfhw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jstszgtf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ieuhfbng.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3itkzbeyy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3msbsegrw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3trwxvkim.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ffwvsyrt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lqhzzbix.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3nqvrfgbe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxwdwoow.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pwrzfjdv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3givvsjbp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zvrvstja.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3tjfrhfgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zirtznji.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xvikyyyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aoqqhpjk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rtpyeduw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yjrzpczq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3aktycjmz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wrnbhkdb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3aemxdbpt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3grjlvpyk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lupilokq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lgbnhhug.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3grxmuejv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tjtfqjcw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gpunstcv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ltsrxway.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kekdlhaj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pyhzwuki.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dvsdbbpi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3izirnmtg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ebsjllpc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3owzeedpz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jmsyoqoc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ppkfjqhp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vlpvjfqm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3thiadbjl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yajaalps.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nvteisop.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gofgyaqj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kxswgzih.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xjaeiosg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mtltbyte.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qdjebvim.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ymrobbza.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3axtujfoy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3eqofqgto.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3iczvdsen.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cvlacdwf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cmnfkxin.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wlgwaqnd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fexdaeht.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rmqsmlul.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gnvxgexy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tevdceey.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3giqjtnjd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zvgoxibx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xtmpssae.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3diuuwowb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dkatjllb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3snddyodp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3qlsczamz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bbxmsaeh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3uncfuevy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kgexulva.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nfspfhkv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yvwdvsah.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3kgiaefuh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ijncxjry.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xrnvaihd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3tuyblqld.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mfjwznqy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3uakpjqss.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mxnhiyhm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lnidjftv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ekjfvokr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3glhrtxgn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rbsudmtt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dlsxjugy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fdcbqrcj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lkaefivg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3cejnlcbs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gudcupey.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryxehmgs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3nwttzgch.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jsluhsrl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ysqngfcr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gbkvumpv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vjxvgvqg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3puoynzhe.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rdbhqfbi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3vxldwmyd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xzoovwyv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qdkjxqwa.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bourfffx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fyrhaezk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tcppzulj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hytnbvpf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3gvmcvldx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mwgqkfdb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rzjjdpdx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nafsdetj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ymehddek.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pcqefmvv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3inwletql.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jswdlonk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3dehdipbt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dzyunixl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3oqpkxlmz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3efnztoph.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qetmfyrl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gfdhdjov.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3poeqmkge.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dicpqcih.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jrddkjet.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxrfwnai.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3znusizwu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ngoqcnxd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3yeicpibk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3otoyiixk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bvnxrhgx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3nmnvcmgl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ztzibbta.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3lbwebckn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3smhpfmwg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jvwyettc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3sulooqre.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jdtvsnvq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jgshuxeb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dzdbcymq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yfzjzgxs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ocoofvkf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lxhkinlj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fsnbmref.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xyuvgfcd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qexhbeol.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rtqbdpqm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fksgglze.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fqxxafjb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gbxtamgd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ezxrceqi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3klvgchfk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ntznzpas.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3dbkqsioh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rhpfzeay.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tclambod.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3eyslbxfw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3neahbaar.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3oilwdvzn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3sdirxgdl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3epqzqwln.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3amtwzorz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3iinkhhbe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nczsmqvq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zfpflwmj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rnnsyoyx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3rkuyeaxx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3uakpctxj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ssynqotx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3trmtvthq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vepeezdi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3irsfqkdz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fqcfoihy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qqqmptmr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dfwbhqil.html


<!-- 参考信息 -->