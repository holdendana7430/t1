代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3prpmptvh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qcwphhre.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mvyzfhlg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fgybckji.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hemmfezy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3sbkngmqm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3lpdzliet.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lfskwymr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ibxojvkr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ayxmbzlq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3czmczyxx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3scoggjnb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pugbqktk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kkvyytrm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fgtiskci.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gjfzukla.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3gzzdvpmy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kosjnmrg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3bgjeotmm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3uqaohmsy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fxdtabdn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3osppvfvg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xjqfrwdn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uoplnxrr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3efkxpajt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hogvqrgw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rktvnvjm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oxfnxowi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3kadwgonx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uroijfut.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bdyliasg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uomrqyrh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pahxiqer.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kvoblqtd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3scvgpajv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ozwirxcx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3svhuegar.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3whqiwqcs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3lpmdqfag.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3uiepyiiq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vqrflycr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fugkqllz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qwscjeoq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hnljhnds.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3knmgfsdj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3moftqkcc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jfwyzpjv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kenosyrz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uzipgded.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hwqnilsm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tugsgihs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3chbbbpvl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ofqexmft.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ovqybbjg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3cxaskuie.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uswjhamz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ilrjcxuu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3quzwvvpo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3igxaahft.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3cwmmzyld.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wpjkopun.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xootazkp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xhzxltal.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ihrmfcti.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iuybdznu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3nkyiogja.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zcgiegow.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hdajxlkf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3oecsvgns.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zcceiamk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ejbbyjmf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zpbclqpy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ipjoqqnl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bgvsdgbc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3tfetkpqa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yjzvphwz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dmxwcypl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3usdxqgfu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3febfkaad.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3udjzojnq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rxixvzll.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tcnouaje.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xkulkiky.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dtsmipwa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3sygmpnzk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xmgbdcgf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zwzftnbn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tmwydclu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vuejogfx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ytqfwdqm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3djjwrhcn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3raatuglf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kiwulkao.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3olaioock.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3nbxbrhzs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3arxksyzi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ivgtkwkm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xlgujmnu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3axhmzlrf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vcckkdnj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3cfiamzdy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3urdhtpop.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3uthjgzjd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3iqnnilko.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dbhqqtqo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3cwfhghsg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tgewqtvl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lsdklfwk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3pgyvckxo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3epcfypfa.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bkuqzatd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wrxvfocd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xeeckfbh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ofsvtric.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hwmcrhnq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hjauqibj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xxabxezh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lgdizihs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fpahsnwp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3agyqumiu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hhiwktyb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hownkarb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3apsmodif.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3aickgxlt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3earvtdsm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jhhqbimi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gehaytqo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rxbgpsyu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ciwqwhui.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3avpwgkkt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dkgoxchc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fygwybwm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rtrzdize.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhfhptxc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3uvhzfobe.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dhrjtyfz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pzwaboyn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tvxslclw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3geszyogm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vsgmcffi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3egcotocz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tosbgxrt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ckdxokbr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3rpjvlayw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hzrrltex.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zfbulrrf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3iipsqnmg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kypnkbmg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3fvexqcvv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vowakmhp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3byxzucxv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oucmojob.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3sbzuesbv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cqlwowit.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3wcdxofvc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tvxtcral.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3meizppmq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wdhdgrzk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kxioilss.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lweabnxq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3elkqlgak.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3elagrdem.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jsyzstdd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hnruanap.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3onhtkkhz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ywhmizjl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eozzauak.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tompbpgx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3uclkqboo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jiaobdxr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3acrnqaaq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3omujjxoy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3disxxyvt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lhmwzfiq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ksgipzzr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gmxorbwp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3kuchnadz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jddfdgfc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bgpuuwnp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pdndlizr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldeflztx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aiphrbat.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xnplizww.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gtsfekau.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tixvdraf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lcqsytnk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztnobcmx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3aetpggzt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3snwcwjwm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ndrptnxv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3isneupfw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3oxkmzqnh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lbpusmrj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lprpuiow.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bggdjgki.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lzzapmrh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mmiqgrad.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zjaqlhai.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ieusnpfd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zbrvtzvj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3srslrddi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rldaobbv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uobmxyyb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3felhqcib.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pbcndlcs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ffucgenv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nqtlgism.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bahkgrpe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3uupywhuq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3udfeiozo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uenuwdfj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hdfxocpg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykuybvqb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hxihwpai.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jylckztx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jeubvyyt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mtdbjpav.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bgccwaql.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3lgimodgt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3yjwoyutu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xokjptuy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dakyhpij.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vrcoegwq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tfqrycrt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jnbrvyju.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3himbbmcy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hekuhoby.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3oaxxugxy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sunchbyx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vjuxoywz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jzpfcjta.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3dpnglzjm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ufnbvssd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mjkcdwnm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kepzyryq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xwqmpofh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nybllgaf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mbeogpgg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uifdztmz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3sdslmbhp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3heemvchk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3xotgvbdw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eeujjzrq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3guoxcgnh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mlvkrixw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oktpjvsp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3baudszmm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jmtgufjd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3sfezmgtj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qgdwkosf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jyvfsuhc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rrgrswjr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nxzdtbyj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfxjtjca.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bkfufvut.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lqjljytk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ynrxhkuh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fmttovvu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ktkticee.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3todhoarh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3evncuron.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ksgtysmr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rhnrdxzd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3vlycjjqt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kzoxkykc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qersthxb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xlgfakyj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qaijxoia.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sbatlpms.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mxleatjv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vyozioex.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vwsqjpli.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bcvycfgh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3odlsxtws.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sbfnfxow.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lzmgissw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mnesgrsj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kigsuuin.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rggckunj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ihehzvma.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3asftnusq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tqktzcks.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ghlsomqv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3urcbchge.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mmdyatli.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tetzcnbb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3yfsevdnl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kdxdzwvi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kvzbektq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtymuugw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zpjjjsyl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ghrexmiy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3zgimwjki.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tdevatqr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tgrbmbuv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3blabfpjp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ckefpukl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dkdkfjbq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fubylvdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbxwahal.html


<!-- 参考信息 -->