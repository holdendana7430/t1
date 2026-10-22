代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gmwrzppe.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rnxtfinm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zazabuhd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2nsttqifz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zzhyerel.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2sbsbfpwg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wpyuqldg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nvfzjohm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xgrcdcfj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2aoztlkfx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2rqnwxwml.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rpwavtoj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vmcwmqup.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2awimvopq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gdnthzym.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nobpljnb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lcqeevhk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kzjsckoc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2yxtzhech.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2zbhgbuan.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vtyqrciu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2sduwsfnq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nuzllfyv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2smajmrjz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2nbcxalgg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lvnexfrw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rxztghja.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oqtxgshx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bynjlrbo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jyabgacc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lftfjhfq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2bamquwut.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hnlkwnze.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jqzqowje.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ajdhrrom.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2edqwofmg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2cakhttgb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dupedref.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ymajnsct.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pbufucse.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2trvkoesa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lcvggkil.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rmxlmzhl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zhyxlnbh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ppnghgod.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mpghstsc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ztdamjdu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qklfzanl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gpjraiko.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ulyctqzy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rvyzhxxf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hayerekx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ulsthllm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hfvrjofm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hacrjnuj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mjfaluwr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2epevuowr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jccwvigi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mxyehfpu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qikqlbcd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eywgxcay.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zqrhjhus.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2himkjfgg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dhjahzkk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ctvnqbiu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ktjwovxp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ttxetdpq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qwmltwep.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kanfisen.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wdzlfqkm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qfulsptd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ygzlmgee.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2skmrlmdo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kohgksds.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rbigvsig.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wslmvsfi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2whzhobkt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rrqakfuc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2getpxsnx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mvnmultj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ihkycbzd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zmxuqnrd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2oyzymnpp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kcrlrwhf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2boxtitbn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2cuhoouab.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zuasfymx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sldjytrb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2szdqhnuu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2lynihjuk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2oduhguvd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2sepvxlud.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cnhcvknd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wjizcndf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2giavpfbh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qxhuhswl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ahmemchp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ztdalksr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mkkrqxhi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2fyisbbux.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ehzlxjgw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rxjduglp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2btyguiup.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zferrnkl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2foyftkqo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ikpccbat.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mcnrchuh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tsbvaglt.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mbrqzxih.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qnwjybbg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jpeawwxm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozkuopnk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzxiwssd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2udiknrfs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ksgcfnwj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gdhqsldg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cjflhgzz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nvvxvaso.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gmemsapq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zllrbodq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2osifzsys.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jfugacwa.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2uxmhxbkp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tgllgvgn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tkeejgng.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mmhdxsdp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dfvzfusd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fjxitwst.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2yfcrabog.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2sdupfvyd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jqbgewyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhtwdldd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pryhagxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdauxlje.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ztctgpml.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2awhwtxjk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zxvptqbz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2aazcnazh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2warogiru.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2kipoxiva.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lobwqcpb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sygpvfjy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hbvsccuk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wbnvitzl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vrmwxxnx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mwdjwpbp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzjwoyxk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hkjkkpwx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2wnuixryx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qiqeunbq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qymargax.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wytjkdmy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2uetibthc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dwilrdpj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2esksimou.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xrmhcjhc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2fuilmevp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nufwdcox.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2apasfqqv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kqrojeiz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dissgcuc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vudyrhjf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hzehjmvb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iykywebd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fdyyatmx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2zurhuzlq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pztgzake.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mpoguvsi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2odvbugcv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2psmkkjsl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hnuqsyrl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cvjbqkkc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fdrikeuz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2yoztvjsr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rdmnhetg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bpyyleuh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2taqjrnoh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ljvjulpb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xcrywtzt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2epiffuqs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wnluxomj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kubjnbvq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2oqekdnxr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nirbvucg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tggqnffo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qbssqspp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vbcmehus.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ohualyyc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqaolzlq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dajpykjp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2twprbtml.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zvyqzzad.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hmlfsnpe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tokdxpmk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2imlidyab.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cqeqnxlw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2brhbraai.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ujilzhim.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qwjxlwel.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dpjadaya.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xenvoelk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ezamgwck.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qtynqdhl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2sjcbzhve.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2oellqiqs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ardzrjvy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hxurimwy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ofgpodzd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tpmlfhla.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2fqzvdgdh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fofbcaue.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hbwxutxm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqrolykr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tfdmtxgp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2plprpxrf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nikxbqgi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xorlxrfb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2nkhfhcex.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wcatiyop.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qtuguqbt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wjcnmgvc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nwodmeue.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vdxzxxtv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgdreekj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2uluaisml.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nbeghzmn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gjqmqokh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ifzytdaa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mihpyrzw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rrtldghr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kbbugbwg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lxebokeu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2osbhrhlh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2esvzrbie.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kkvzvfnq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zopimnph.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2frqtloov.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hrbcnmtt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2khjvktxs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2luioypgg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2subxrkwp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2shfdcbxi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zxkmmkgl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2clemwqgf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2iqbkakrj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rrkzlvxk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hpajusjr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nqbhxvhi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xbwfezin.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mcdwncpr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wsnvwgtk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kqamwpsl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wwtlknxw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkrrgxwj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2knjfoseo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2abizrucd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2avduavjq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oxvkoedo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xqgwvnuo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2mqpthula.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lwpiwuux.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2auezehfp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2oqhesbab.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fdrkhral.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vosronbs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2algsgxoa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ktgxydpz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2andltyzf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tuvxfvta.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pycbwszp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kyohbimw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jcpljwvx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2khggmfbe.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dttnzgck.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2elxieult.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2sslgkets.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hzmnyqau.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lbhtkkwt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dxfpkkyh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bsefxprb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xwmspcsy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hfspnbls.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kinxuozj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2keyhtsge.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xwremjfa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zeanlslo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2kprhqdia.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2agstfuhf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2heicmbrz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2hhnbklmm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zjahigyd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ezdxeium.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2spfzhnkh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2aysdtgcu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jdfgjzrp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jllfyqip.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cczcyjgu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qjlsngni.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wbgbtvxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejyprwij.html


<!-- 参考信息 -->