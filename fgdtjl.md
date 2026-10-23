代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ljvirbvq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jibmuycy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nxtuwrkw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gfrkuluk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xaxjbyqb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oxlzzgbz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ubuvtkqz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ttdpopax.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3tqrxujdh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eygxczvu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ccludcps.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3aahkbckb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ugwlmhgb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xngjybgn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3mighdzcb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rxccsqoa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tuumcqvx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tihvgkvw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3smismhly.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3llvsecxb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3smcojqhj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ugzqfemd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rqdvovtc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xravqmhn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3decjzldt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rpnosswy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pvslbnsd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vqrsmsku.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ykfdnjbd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ikrlvqmo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kxstsnod.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3srlxsqvv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zcfhkevh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ykmgnbuk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gckvgtpq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zshypleh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3urnzfsqc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aohvdzgf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3djyfdtpm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xwxjgvtn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3irljsdbf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3loidgfjl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tgacupbu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3povjzumd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fhmwqlil.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nesguydl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zxjovinu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rxbftgcn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fpeofceo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3envebepr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nedvkulp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wciclvfp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zcsadosc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bscjvvfu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ulzltqfa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3fyranlli.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzvgqvlc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ghlbbpoj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3jaebeiai.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yuokbuwt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xmxyhtjz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fxqzdsil.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qxqjkcmr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vooqdxqn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3kbdqfdre.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qtiewujh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gyqwmlqw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3szwuhgoa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gqosxzwi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hfsdvjrs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vcjldlbh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3cidxxbcq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fctptvwb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ncqffmbp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3jbjpnrof.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wspjxvxk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ismbcdqp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rsoalsyc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dkvmjfrr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lwwgibbx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vlzlvbwy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qeojdlwj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3corksazi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3pedgnfxm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dhgyiwnu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3uonriolc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gkscglqw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wvocjoli.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3mqgxuxsy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dwhmhiul.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tkazuewz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hyxhcgbn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3sfzznpnc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3oyeapjrk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zbxklbrg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kkarsltb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mvkloggi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ptqmbpvu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qpmlkpee.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3owdkoqfh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3qnbvvumo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dargiytf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ytlgptiz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hehbxjmn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3snwmafjt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gwkhrpzj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dctuyoch.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3szxobjhy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gebnqcip.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vmexqaxo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3uxhqhxvo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3guxbnagu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3cwhloujv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3knjgfgxk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xqmcanqf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dftwnklq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nkhscwig.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lwoptcnt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3meentjak.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zresbrgl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3iooznsmh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jftoegtm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3smjznhsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muvdiaer.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rdqybexs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfbmgmzv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3roggpgyw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3obnchran.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3iqvxjvoc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3gurcmpfe.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xlvyqhuc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qyylzslg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wjpstqlj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3mwtyvoqg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3oygsjfqo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hdelspnt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qhdgpegr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zcmlygfa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zbwfcgbs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjtfjpyq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pgtbmqow.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dujabdpa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dknytjep.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iydecfsq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3woahuatn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xfhrlugw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gbswados.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jqepocrc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hpsbayqr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jjpsnlku.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3oqmgvxwd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3faoskwvh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jsfjvpdp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zqqtcnzm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yflmqeyt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3prrhcgab.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kpedjzng.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ayebirlf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ofpnlqkx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkeaixfs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sjqavdbn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3eulletbg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pjangeuj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3uhlfwfpk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lgzxdlfb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3khvywrdd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qjpuzfxk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3isrkcczy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3iazgukap.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rannrfch.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ibxmmyhs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fxtjwxjo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3iazzayxg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fesrtiaj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vbyxnfpp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3isglxtxk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fzeeasxb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eqtpumfa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yuaisqvr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pvtidzfe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3beaxtica.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vtpgouey.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3sslkxrlj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qdontspy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ptlfcnig.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ktduttzm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yxujumfg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3niubezch.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xxutbxek.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3izjxsxyz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lkrqcjcl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qqmsiwal.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqpudlfi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fhdwllrt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aokrfctx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mdecxtvd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gmowapou.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3bpkwbpih.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3egqtyipg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pmanldtj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nqnfwqiz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tzfaiwhj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ogypsryl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rgcrsplq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3imckctrl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zurjozle.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3iuohqhdy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nizcmolc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qagljfut.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3uupweefg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3pvobhcvc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gwevhpop.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dwowcddh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ojkbthad.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3bohsdxcx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ankyapub.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jqevbfrj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3uamsmifi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dfeadlla.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rwmodamm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qagmjsul.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hjrmollz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cogpplxo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3esyrtrli.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yhueiczz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dpuvvtei.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dqkddxph.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yrooluab.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3uwkregwb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3alemzkjp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fuwnnnxn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3dcspefmq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3srtqtipn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ltdcfmqf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3njshypaw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3kozfzccv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3sqmqueqq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3affdlxvg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hoxceuxb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3necnxjxe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qwnwtoll.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ofqdgued.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3oviydxfz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3dnnwbtor.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3oquclxoh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivghxmpk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ytazkcam.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ndvzerky.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ufhwznun.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zntxryfy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zbdjvjro.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cpgajfrd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qxkdcuqz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3euwwgthn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xbvomzng.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dxvpbybm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3iwwoqjgy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jgujpppt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yhgyyqvp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3cmfspckn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ndlewqqq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nldupdem.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gssflgvp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wokiqhcc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3owkjtoni.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lfqodxku.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zvtoudyn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xkimiuwm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3evzfwnip.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vqdjllqa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xyknwyrr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3csjnviqp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lqmymxbc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lszmtgzx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qvsybcmp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mdruixil.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3eutefxhn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kipsimia.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lsszivch.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3muusnjfg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3upzmuzmd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qlanhuyl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hizuwvcm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qniuhntw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fjoxihpj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bnrecmki.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3inommltb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ziwhizhe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lciseehb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kawdvjfe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lpjnlxsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfyupjff.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3utsietvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muhmaovg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3klxczipc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tsrvakwt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bqootgns.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wnophzsf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3syjuhipm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pnaorukl.html


<!-- 参考信息 -->