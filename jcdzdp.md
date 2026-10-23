代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ttlwcxrf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mcmunkci.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ncixyhzi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lxzjcxxf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jsalpcvj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bramslkl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ogopdmgc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3yustixjc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vqsogoss.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fylvbwub.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hgcglxlc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xsbipnvg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3urlstazr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3udkupmjf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tgysnthz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rsxefeba.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gxezoyqb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3erroapme.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gayewcpu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gdpzrrnh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3cpqydvll.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3fdjxwghq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xnrgrdek.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3oqzmxovz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ghfamjgo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3plwdcmyu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3uojlltvu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3odxcfouy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lmpzjmmb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zuxvehyn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mfgyoomq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vdfubslf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3lcwoclcg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pcnssktf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3azjtkrci.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3uxqgctuq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hmmooiet.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mxyreyqb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ferkznei.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3piqvayfi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qbqmgvjr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3nrknvhhl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zwjgplyy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3uauuhgnb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3yzaeeuil.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ubrrcjit.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3baqbbrgc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jqnilomd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jxjeuvxn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rejruynp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vlveyfsv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hupaktni.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dqoutjhf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3prunsayg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xvxkubxi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3whcpviik.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sfsxvsyu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3onakzccq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3orqffubv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3uputnagq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bcyhpuau.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ngxpoeyl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fnrywpwu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3cvosnipa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3boedsnga.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3iaaydxbq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ammwyhkl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3orkjyunf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3sftbtywj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rmyusjog.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3zcxjhyin.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uouduixr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kvdiauhx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kkfiozpc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3eznxwqmt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zzylehbu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ojefnpoa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3nljbgqjb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vlqyagmh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3knqlpxea.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dxnvpmqf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3umnbmiah.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3gpwamzck.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tfrikbfl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wsthqkcv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gsyqztmf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yhhafwgx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mtszsgot.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bzqqgovr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3flhdzzgh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tggdajhs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3yrsassci.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wdrryrct.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3eutuiqje.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bzesdvxs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qltpedof.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sqcmhlzo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3egugguna.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oliktuhf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3swdxiige.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gzurfxgc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3eophdksh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3anrmnodl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rdpfxvsp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfrbqjit.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ngzyepmv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3llnotvgy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3aflevlwj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eqxpqcna.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vwypvlvk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3puqzwkau.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vyaajftq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3mrljdbxy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nxcacuip.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ixpgzenw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fpdoniao.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bcwnrprb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3slkzkjtt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lylrkhma.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dskcckpu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dazmvgtr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tapzxfpx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ofwcoydr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tiebaxux.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3sutikxuo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vmpnduht.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ogfqezmj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ztwlqbys.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ljzgptlt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qcvnoopx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3isninzcl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xrqpznuk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3udpxsbgf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wmrwlyac.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3shuqgkmu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bqdqcqoc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lpoazyao.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3itcrijwy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kjuzurnn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wuhpfvyf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3utqbqdzz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vfjdwzlc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3whsdxdpv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jaeesdky.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ihxwkrcq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bysokdmp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lokvbygt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaafpnlg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hixtoedb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oyxfpatg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hhmcavny.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3dbtqaudq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3vcgfonej.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dxxvkyyt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ndckfnkd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3bsxarijz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hkwijnzw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgwuzlra.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3fzlbmqmo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pkdttcam.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vowewpae.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zfyrugxy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3srkrdumi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3iiiiskcc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lwqnjzrf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yyqpufll.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sxccsgva.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sqigikdk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tmkdncwp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vyhathoc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vovrhfay.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tvyhfuas.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gopvxsmw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hobwenfk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yzblmozp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zumljogh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3uuzephke.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jkitbioj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gvognlfv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vcopadfo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bcblqnmp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wwrdyxsw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tbjjasmt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yhlubdpe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tbaxkimn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pemlkehg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ywquymzh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ughozsga.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxpcsbbv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qvcfjbmk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rtkrcges.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3flghrzcu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3umbxftyh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xbtwgmli.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ytptardp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dtkmiyzc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3suwcwufc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fzjxxxfd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3bxkutmca.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vbjnpnwg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dyjbikrl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gcnmawwm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3aizunlie.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3aatyclka.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3optsrcdb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3byyktysk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qxbxehcy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hetdugap.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rycmyntz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pbinexqc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3riciljtp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jgjdcsjc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3knqlbypr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tdulzjca.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cuskiaok.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jcjzmzqb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3egltuodk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3awozuqfl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jatfutbj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ofmclztd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3elzfrwnb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ezzgcayo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gfpfostb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ipcxhyid.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3rpzwpnfw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3bclbqwuq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ypqqqoir.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3owcdyvxy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hbqenbon.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3eujvnhgm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ztolhnlt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qqbaqqvk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lpeshtjp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ycnxnqtz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vlfwvukd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ksuwtyys.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pzlkvwpt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xbcgdgmj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3nnmkwxsq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3eyaiukov.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ybwalhur.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mpueyhhc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3sayqnfwc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vktfsjne.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3knntmfzn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ijxlgmrj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cujqolkt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3eogujudq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kqvuypfg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jmgehatc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3suvppdlj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3iofwgedq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dvtbgqgv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pcqirtbh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tgomdccl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tfxynslb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pjlqbluh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ggxphvqd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3srhqxiix.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3njfurrvu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dkbeffmx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rdjvyxzi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3htaodovb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ieamauji.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kzshnhbz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ltwuncgh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hbvipwrv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3sorhizlu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xjdjgyvc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzmgxmvj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jywvsceq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wdcwdhgr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3oheqphpg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pnekpixv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ojoannih.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xgzfvztx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3bgedatsh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzhupavg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tqrkcfpx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dsvzxqyz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3quuxxvtu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sixuuqhe.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mjulriqg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ztmyugnu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3oyvgjarc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zaxchfaj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nyigtbra.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tuhmemdj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wdpqajcr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bdlxysre.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dqrnbvdn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3izlyxkdk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ggdilqsq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3eonaovuh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3foahqemm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bpqpfpoz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bejzmstb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gtsposyb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sfnspzwy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qawalmsn.html


<!-- 参考信息 -->