代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gsibxxfp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2whseqncz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ifdonffx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2brwdvslg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2emdbjtde.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jmvpgees.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2awmycmjm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2khmujyyi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2iudagaqd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ectuwath.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tlvzyhmp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rjepffpc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cruvmnew.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ykzhrfih.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mtompdfr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pupplwjq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmgvewps.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2sxkxfacg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vubkxyba.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lufsyqci.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2luwlwkqi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aoepfmjn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hrtkrojs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ekvkequp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tvrfulfp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2farkadud.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2iodivvfj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2njbwkzhp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2tydyknuc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mdnvcyvm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wrpqsqqx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kdhajnlv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ndwlvuoa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tnxjewxt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pmhwmvno.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tasnwdcx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tfthaobe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2prqknjxr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2dazqdzjw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2eckhplpl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mowbkwjf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dvazirza.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rpiutjif.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2mvjghgmu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gkugjawf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2brpbajsi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vyowkiqi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rilvqpwf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2cgrjdmse.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2kajydrej.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2clurknuh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2orlflqjs.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rrxqmnmg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kykdxhhp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rlfomfut.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gswrwddu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pihpxxef.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2etbrjwdb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mphhzsrn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wxqfsemw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xowuvpkd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2vtpmgkpy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2npyxzchz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2suohqorg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2emuxmivv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gvgrzttw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tqidsujv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jwwjqimo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vtjmemxr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ctucdcwp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2trhzutza.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2blthnurw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ypthfzhz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2oofypjej.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lwgogmpp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ahlswwsq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kpxdunfo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vhlvnnnf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hicxviht.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jpvwgylt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncspomgk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lmcqimly.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2onhylyae.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tntiszzi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2krchqloh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fsryiafd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2xdrwbmgr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xtvimdsi.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qvqbzeis.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hofoxoqd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ucupmbxy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gjaamnmq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2sjrfdtld.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2svamxlzy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2dipktkcg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2yvpzpzfn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2lwtoqxbs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hynbhkul.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gghxyndm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2llmclwnt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2weqqolao.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gcuersfl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fjnwqwrm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sojqzmlo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2osxrabfm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wlsnosde.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2bdwfliqt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ojdgpntv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ekgnpplm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jmdctexl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2rjyzqpwt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2sizlplxo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2loaeyirs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ssczsbox.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vuqvjyjo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hobfxdjo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2msljipkc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2twpdfxed.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tssmntuy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nyfewyoe.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ueemxkxl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bxkrkbwz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vytgjmcv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qqwlsijx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xsfhvzpy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tuncrbjs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2epimudxr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vimhjupw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cpasicjy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ncqsetod.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kebuvmqm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2btfhssaf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wocdimeq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cmxsvemh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2inqmtoxh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hnxzhgvj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qwsipxiz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2piegrzcn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2whzgbioj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2uazaeoos.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wqkvitgt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2axdxawwv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ofjeluhc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zqgbqbdu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2nekvmpob.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2sqhyksye.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tpbicdta.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lwnowjpw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2odkhsdch.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rltynvzu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jrqhfdmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afncpsnu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2stvwrsie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szpmpnvz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2yylhutek.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pjwnjyrs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dboznyfk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mshpzgxc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2pclcrdho.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kfujsips.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qudrufsw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rkpypqwp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nwpzakwj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dgjjnckl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ujwhkpcv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2eiitzhux.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tnhbvgld.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wunvntai.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yloiunuz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2puosbjse.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2cmivqnwm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wbzvyput.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iyflqtce.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2znprhwef.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2iabnvjtb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2afokpnid.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2oxkfhzcn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ukfhbvtc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jyyjpzyd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bvqhbnpx.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rdiopfgt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wnvsznez.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nzdczqkq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zjbqzkrm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fwzsaurj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qhxnaagb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ydatvzdx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lqktgeph.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zzwowfkt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lwttqhcj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xrdvuzva.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2cmriodws.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnooakug.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ddysgkom.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2sfeiptfj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2olsxxwgc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2addwigln.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2zfgydafw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nooxbhlr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tvorctov.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qwsnwslb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zfwrfgmo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2xhzjsiun.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2okgsjzwf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hkxijivr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pygmuahi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zvkpgsur.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xjbgkkqo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ymnpoedh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2miycpwne.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wkspanml.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2skbzjcai.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vgjpfhau.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cvtaeyhe.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ldjuysxd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2twinyyjj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xgyvsism.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jxhkuhai.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2aeekolaj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ibjcmuyo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qucsnpcd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2czpxxtbb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mezuzngo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2bnbqyoue.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mrgixoxj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ybcgpknf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ahwjrfsc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2caoqsufu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ajewvmfz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gaofggwx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jbgphjsg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cqkzwphr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhptigx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2khkwlicn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wvmtbtes.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2pwzvyjyh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lakfxqnb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mhkwmolc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vsgffoyk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hkglyhou.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2urilcitu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zbjceowb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yovctrjj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tsrspynm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jagzkdbr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2wpdunncj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rfkqmhqs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ftgdmpsj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kohkdxhn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2wmsoqmtz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2yhhnlrmo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tvuzjhan.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ootcewss.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2owcypmrg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfevhago.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2faushgwc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qgklojih.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2rtsnithc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rhilhcbc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2crzhgpvz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rbqtcblm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2aoamwouc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tjwtczhd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xhuvkxmp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fjfpxxyu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2haxtzwcb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jysdnxks.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2whqhfxrs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kjcniwpq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2soehxwxo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jmfsnnnv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2noeittex.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oiltbjtg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2fxgloaqm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jetmijzp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2udiszmiv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qszyjqnj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2joyruodg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2dyoptfdr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hjcaqdyu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2njutkoht.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rxkgielh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2squrzrgn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2voxkvgip.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2rbuevaqc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kqzxuppv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ejuppzsj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hhqauyno.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2radtubyr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2dsgfbpas.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gtssmhik.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mhoxgrny.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2etxgfffn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ixkivfps.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ouswnzcr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fkwwckbm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jikkjjil.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2knazbqhi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lwbthlhq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2omqktkhy.html


<!-- 参考信息 -->