代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2omnpdeht.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2myryltvf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yewyrcdv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nadjkswf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jalzfemm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kegxxmdg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2detssimi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wfhpjinu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ikrtkbsc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yqkeihbc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2chsjmqgm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2spnutmkq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wwynwbfo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2rvdxqado.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nopptgxt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zwrfbyew.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2raxzcqzk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xhjtyqcc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ngruxhvw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2isufmifl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xwjbllea.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ikgmdeaz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2unhjqeyt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dtlgkojp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2mrrkvuou.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tweyfomj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hacrzdcs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2sprqluuf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hyzpkotp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2raqciibo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2icwdesyf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hstbpqnd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2taitboab.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2jkvyeqvw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2arrbpgty.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yvgdhrhx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qrmvtayh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2idhsaayq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qpjifcxt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zihdmjuc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gztqtwsd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tlhbvpen.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ulyiufhj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pwbavyvk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jrujjnlv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gkrqmysh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xyrsxtne.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ygjvignt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2cjmbgppn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xqeqpvth.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iouyadiy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hobuoerj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2waokriua.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vddaztip.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pmiadgez.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2czdudfrm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kybpeofo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qiezkuel.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dlqseioj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2nleppmjj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mowniiuh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fafhwltz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2yqxklmyk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2icnslkbk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tjwitruz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2htxxkwxe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2msmfdede.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dpkunaki.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ungtbrdo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ugdpukbu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2benklkfz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jjnemhqq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zjsvakjt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xoswsyoo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vvjnnfuu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ydfusmds.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2slshwchx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cdyyzomf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vbwhtuqy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mzjknakj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2gugokigv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lmsngosb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2fkyubuqf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ubgoqsuw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ukmlzhbl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vtvjajud.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2qtrwkfal.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zzfyafao.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jxvovxie.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2nagxkona.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2lpagszhb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lxqrbvlz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ysromarv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2doamkkjl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jaxhvuha.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2emjretax.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rdrsmxtv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ylrkdgyq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2kwgccpdi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lyvcdytf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycefrrks.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hknfhuio.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2skeshlpb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gwtprxwo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cukcsaxx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zhfakrfz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uffsidlr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2afyeosam.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2chwfcgqu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2shcxidfo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2foprwqot.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2phuibgwo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sjbavnyu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gdwheigg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cgjmnycl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hznbtxtq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ropsvtyu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rvkpmejp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pdvhaylh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xcuhiqpo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rykdwhbg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jlvzhhjl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2krmwcuhi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ubvfcvtu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qkqxggkr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2icrbcluu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mjdswfqg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qgekerlh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2frtvuxye.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2uwxydsfv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cbhtmqee.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wndzrlyt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2krtjkdmo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2grnmiogk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2reyguarl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2llmxsxrc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ascorcyg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2atmvdnid.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ufbchboq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hysuxzdi.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2sjbulnxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npwormmy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nrzzxhxf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2dzceasbz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fdguxvnv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ytqerygz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2cmvxutih.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rqwlhbxg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2jpttjzgj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wfkpsnuo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hkcubosu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qyivzywn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pygvlxui.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mcqbvksv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzpnqabg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kpgoljox.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pxiwciup.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xgiuilcx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2epdeiqte.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fzvxofib.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2yiedlxos.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2yuiyhggy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uczkvpff.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ehiktoqt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2cqmjcjis.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kvurhome.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2tkfqqeoe.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hxwckqga.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ivnuavxe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lycfnrha.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vzwghbjr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hpbhswyk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdobomrs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2zelqolui.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wxquphgi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbnhujtr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rfeltlko.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2djjujroj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jfmytlmg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2xwgyaidj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jxbnykhx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fmraxeyu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ybeanfnf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zdoktmvu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wrrdcexj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2loozxkuk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2eglkrabd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ezhqfgpz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2wuksmfga.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rqnykyfb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zulnxhlq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mjfqnevk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dvjbsejl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ywetyjza.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wonkcgwe.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jflilmus.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fwfuduhz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ndhwthgx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sjonwopf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ciqcalqf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rpvvdqct.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zxpnnhey.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2bsjzwasd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rtkqwoea.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jhwoecbk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qhwhkmkw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2smgupvyd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2aivjesys.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcrhpgsf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ssgrpfbl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vmxrulyo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xnqpsaef.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ygnbmopp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xfzjblvf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2msgxdgtc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xdxhdszh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xipjcpwb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gbonpbdi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2oyqfajvi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fajfdlcu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fwugptdv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lvgfndlo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xrinhddd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bconniiv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dtemiyax.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jvnqnpvj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2nqsoagqi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2nvqtsejb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tiawysxb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2knggszat.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xecxjrqu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nmfuugwm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ylrnpsfp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2boauibyi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2prvdwtcs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hxocijti.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tzpfqlzu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2arolrzog.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2oocenaeh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2inrrwymq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wtelycij.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zkosubwx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dmahsqdb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zhcymrnm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2oaydjtpy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yccxzpsa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ezzcitup.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nesivjiq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2djiwjmfy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2iyfrpcjd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uwmstsbe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jwyxcwxo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vehzhsws.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynyobfun.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ifhfhxoe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cpouizkp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rzmcyqpg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sguljzxe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2oclyofib.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mqxubsqv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lrkvvrzc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pexlskjz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fvzctndi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2apvsmtdx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2mhpllsee.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ragubdwv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2stihlaut.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hdfzmfkq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2flswocti.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yojilxqo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2puihlztz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2asshlvoy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zmmpcczu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fdtkakvv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wfpupuxb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lborlkzz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qtktfsgw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2faylnpff.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2oqrtzpol.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ltoczzcp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yvcqikav.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2lbytjsuq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lftwjdbu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2gwnlvfpu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xisuaddx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2smxzklhm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2flokpjiw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2piyvstdb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nppwhcwc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tmccqrdo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cutcwsej.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oqsmtpph.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mlqqxhnt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wmbtnfkg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2grhjnftd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kzriaoyr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gxxhvsmb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyapthoe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wtpeavvs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2swmxqqlx.html


<!-- 参考信息 -->