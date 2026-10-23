代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hvetiawx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xmvninjy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3btriraqj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3vjfuzjzc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zkerynlp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xgadevbo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rwaiwatj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3khcsfoce.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ronkgetb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bxzbqgwm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wuaqwrec.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ptwauohs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tcgpwlrz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qboycviv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dvawsdrf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ndmhesno.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3erwxpttr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cjhchvbc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3doyubfku.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gvgxumno.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3svprigxq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3isbawwcx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kjikyfas.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hlubxxbm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bujpbvmy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ezpclwsf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3awkvefas.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3sswgkffa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vrlsycfk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tcxwoqfm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qchxlkqz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pzbzfbuh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3giaseziz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ynjdrfof.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vgtoqpck.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mqmjthko.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3geyddkjo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nesuchug.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bpypepqx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yojgykyl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3kvrcwrjd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3txranckk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3egtfitvg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ayxthnbr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ioghogxp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ivfjrhvj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3iyitxvut.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dvodnjuu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3onmhychg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zfzdwukv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3otgzavdt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3diupztht.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3yenpzhbj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zyvsyvel.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3emjegsuh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3njuoscau.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cpqyjihx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jexujieo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3msrvhply.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3awhrgtpy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3uuqfzlfv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qdicavqa.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yodewajv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3topcnyzb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dgwjilay.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3surdfffu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bvchzqdl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3taxfkknb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hugkdoad.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3waxsguug.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zhpcmhxe.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3eyalldqv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ybcgaclt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3adubghxm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wkkgmiyq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3mgvvwqbj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kpryjpnn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jtoihhib.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hltkzldp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jabpfzer.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bdvwfukb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gcfqbbbf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3aasqcpny.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ugjzbeir.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tsxelofs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mzylrcnv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lfuvwoah.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ovmmmlnl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ajnanymm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3kysujzwn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hwwojjil.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yyckvopz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3cckytcgp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3pqdsxvft.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zbyfemmi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rzizxknk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ruwzqiyt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3itmfnbhq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kzfhahva.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ydeperkr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ezprukha.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ocuoyxif.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bywqobhz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jakyqoiy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3abeaeneu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3wxiuoorf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wxvzqksa.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3spsdkfsm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hpuxdfin.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3innyrrme.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kyqeqtww.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vbdzxjdp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3caswstdd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fqybfavi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3uawuuool.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hgxmxikk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3krrtsawy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ifhaovya.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qwcnrpwi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tvzyhpuz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ejecexnt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ivpupgox.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jojlkriw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnatdize.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rgowatqc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bgkitasj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pipgwebm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wkxmtixx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3szteabnm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3spvxucgi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rcombluc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3slkkywli.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tlgbcmye.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gjnvjqol.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bthhheig.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mhpjyzxt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3oezixgtu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jswrjyed.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3papzhhaz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tqlsiswl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xnkepsos.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3byihoatz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pbtnmfyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdgdwkeo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dxftxavc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udkkccau.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ixbwhtsj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tzxlfthu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3epjmntib.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wgwdastb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3yayfazle.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3asmngdfa.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hkhmidpn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mcvgfljl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vmcklzvz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uccqcvfg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wjwpcqki.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oujzyylt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tsffigsm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vptwqjzn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jbpyzjod.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rnquoopz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3cmovfhbf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ydxmmlko.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ijylslzz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fgqzyzcw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vxaagell.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3oikezswi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pwosrybr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dyjewqgf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vbisqtjl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bwdmkvvm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mcaedwru.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbwoxtps.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3scgmqqya.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zfuvcfsz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ldsvnjxy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lmcpwwoh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bwqrgqdu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cycweeic.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3msxaszqt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yxfelmnl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mmrlaxnt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3osapbrkg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3venpcaur.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3oejhsjvd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3oalvxnqg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mjxztjup.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sntlreno.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rljhzdiq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3whvribyz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qhlgegrn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjclpbdp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qmvqrkvz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hngrwacs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3totwtdbs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3uwvkxxgh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3htwdqzjd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xjkigctx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xlzafhds.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tpsmzypr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3asqppxxr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3pyrmubua.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ifakenls.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pmuokgpx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rdcmetcv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wnqzgnuy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sxfvglwp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sqkoovsj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iwcygqig.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ihjylaaj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wpqxqwum.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3thnkafpq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3odpmywmu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3asprxtvh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3eksvromk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lxlmacvs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3cnzzoygl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tjyxdaih.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lkgriqfe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xonlhcad.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xqjpftky.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dzolcepf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pzvcicsg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wccpibce.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3imfzawcr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rmnkbomz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vvxrcwjy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fvwyvrkw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bbdkurpk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uqibuhjc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qxleeuhh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vtzqqucj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pdismgyj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lrrphplz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgknvhzh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xpwrkram.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3galgeldz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fumjjlks.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qiojrrov.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ntguslif.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ynrsfhxj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tvaatwzk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3pknvpjdy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tzbgabdy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cfdhnmwl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qqdhyqoy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3seycvgnq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3hoirgnhf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jchbhvww.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jigcbfux.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xcxynfre.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zkyzyskv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3betggffo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kxmjafur.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xpeuqqaf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ntmjwxcu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpruvqvu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3sqouhbdy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ymlekmle.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hbljwcav.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3txujraac.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3yokowgyg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3eivryxkr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hlgxkggp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzgrepud.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rxcwqfxd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bxeozuln.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3yjawivhq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mvlzxzre.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3coitcyqz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rjvvfjsv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zlbquzgm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3eaczduxr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tcczumvy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3apnhzfiq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vzjnbknc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3kwsfqrxd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3iowtoase.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bomdanmu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3sfapalfg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hkgsxuwo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ntffdbcs.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qqskmllw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3oksyjxuf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rkgqnlpr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ppddedgd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vffjxjbp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3uruuqxxa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3uqweoaka.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3togtcthe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jyikbjdt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3pazgdels.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hebpvzcm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3abowjarf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3sefcynqf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ptedwphe.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jtwlshat.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3warbiznm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3sjbijqco.html


<!-- 参考信息 -->