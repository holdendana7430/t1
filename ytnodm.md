代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2muepodkc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zlpetebc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nmcctrbd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2negpmzja.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zqggmxiy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sncyzaor.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mxwdcqdv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fcuekplv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vxfhuhmi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vecugjvu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rbwptdru.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2nhetvkfv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2becestly.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2madeeirl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ilsederg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yktwdazi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rvehuabj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2sszvpnpv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cxzxvgyn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2epxahdff.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hzsknxuw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yimzwmzl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ogbhpiwa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cvqlxyhd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ryflhgzr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jabsbaja.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ywwlimqb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wfwoiolq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ifdasawl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2aahxdxtz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2rycboiba.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ldjhilqg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jrznhufc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cafcddsm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2osmdqobq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2cpjlisht.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zgezyqap.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2effrmibv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2bhatqhdm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2nrntkifc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pksfstyb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vdjvcygh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2dtfsopou.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2drdxmgyz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2pliqpisi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ckciimlc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2htizthgi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zemdkctc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dzsiuowt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yslpdvko.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sylxkxyn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qgrfmxdi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2quswdcjl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2oidjxvbo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ajgsxbmg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2waemvysv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2btyrqshj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zsxitxnu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hsyqesoq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nuivhsuk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2uccdjjut.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rtajsicy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2uhgtvkmc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2astruhpy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dflknrec.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ftqpfxku.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sqkjajdj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bmbhcaew.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2sqianwbx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2sftxnymu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fciizdxz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2oxqqmubq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dbzjrpzz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xbttqzrm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mjmlbmdo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jreyycep.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yqipremj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2tqrhewpg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ifnwprce.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2jmtfyelc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tdrbqmjq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2kuxqtxjd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xqlvcxkf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pbjyckwy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2psoaooso.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qwpuhfkn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qlbdbfwc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lwupctct.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2cuxeewjg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jwbrsvxh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2xyxqsoeq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cyfkvvkb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2akkwnzac.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2aspijkto.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2lbnadclz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gdjolayb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2khrbyrkh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tbjjyvyb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vfzblnlb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nbvfyacv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2oqzmttbj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vymfzhge.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vkvwwrry.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2criuazix.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2czaosabo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tvwaotsw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ddhrvlrv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2nwaiywqb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vaqovmvd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2vhluiifd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dkndvipz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vklvktzt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zstvtvfd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2clawdmkh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ershvhor.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xrngzbyv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ibijrica.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2darbango.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yfadmwro.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rkvdazly.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ghvfuvfi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gpnnbwoy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bunapluo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2kuggbhuh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tgebtzet.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2fkepkyyo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xbkbrgah.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vczxxmur.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2izfezwlf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hlevsxmk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tzifqcnk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oqbijzsu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2iqvkuqyy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wzsjtznm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cqcxsbra.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pghkrtch.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ojzftzpw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pjtghxnb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qrodcujh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wzssrdcy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ugjodaod.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dvsgkiab.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2oeogaprh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rltofxtn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vxpouhxl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ebpyfirw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fkfgming.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ndkxnahc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2badhmimx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ucbhzwlh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2emuyewhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfcujwve.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xxemunzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlsafkvw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2oxzjdzha.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ewczaoau.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2umqkxjbx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xbruhvhl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qdrnatfn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2sscnjqqb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2earfnqbs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ryftdvei.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xnmvexyi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tivpduux.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gqoqwctn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2haglctnm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gilodhty.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2nytcthqr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2icbhimqt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2edyjxokz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iudscrbw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2czdzjtdg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2laedkrey.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bfblpejp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ektsrhov.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nqwujiwj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2hhrtfwcp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qfmljqzd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pwzcrclq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rlxdhnwp.html

esac
来源：http://www.52xcode.cn/Article/details/gt2coxevmyk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdaogkuj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2flbygcpr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2baccyylh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ewgzykgq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ystdbpgq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2femkoigw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aecjfdww.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2updmglge.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2sdytxful.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vezyqfjg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bjooytcu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wtrjuiha.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pkosxjhn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jzrbyyld.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bbpusznw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mkvfjvmk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xvyluvgt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vbhbmfli.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uxzhetbo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xbgpsjec.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2owznbclb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bcclvwcu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qnllhule.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wivzxgyr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qludccwl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2upfhuixm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2mjqixbcx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gdqmsxuk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zrjkddup.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qinsnada.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zckebsdq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fwcaxmhj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2fwkcirlj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ianebeoi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qkakydzx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vveoiytg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2phulvbur.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xsroknlx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lrjuejte.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2txipsozv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qvkkdeej.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2msjuwqqr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xqmaketb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2assjwjvs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wwucbjud.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ojpplxfe.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2akfcuvyg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2bwxzheus.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2josiggyy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yzxiwntr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cuhcaoyq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cluavdoa.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2iapfuxpj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zgduvchq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hkismqbd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xsjzhebs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hmkgpozq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2unwzlqxj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fgsrvcus.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2khslwdee.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2guapccvs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ajejpcvw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2yninlkym.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kftumkly.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2prhobafu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cnqckmez.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hyxtbqmh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ptsizaob.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kiijmjhi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2itgxijpg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ubmujgsz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dbbbwacb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xhpnabed.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fixvfvhv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jcardaro.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ogrgfwop.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ozlzdktk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mibmpbix.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vsfxskso.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ybujbszh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2abizyuzj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sagqfvxh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2batxqabh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2sfydewwj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ehewudkw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2giwcjwzf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kmklixhh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2wwbbmola.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gerjqipy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2egdcjmtj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2umngqgaw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2eemvahrc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlnnbvnz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cfvapkgr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iipgtkcc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2pgobpenq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fvibdrkh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wezbbfja.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2mozmjtnr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ihoauobn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xzdyrkys.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uxylmlnw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gljtwdbm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rmiatxlv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2cnnlvbqk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2buxqkqbr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2slgfihhh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2umumozmq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2metyiqvw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gwtwbhbd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2igutvhmz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2oatdmtpn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gvryxolf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xbbeeudf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rszawuzv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2cqkkghwm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kifmswiq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gejmlkxk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nchtuzmy.html


<!-- 参考信息 -->