代发 wailian999

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2nrfemszk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xcjwzwxv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2tvheyqci.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ayxrzbhl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2woqmprxg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nuarpnkm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2fwmbvgbp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nbepufio.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ukhdnnlr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kxkveozx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2cidrzytt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sceuaqsr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2veslvuxd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uezutzzb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2cvqkfsdv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2wpixbsrq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2onecxzpm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2rybrmfdk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zqdjvdvk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2nfctimlh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2pakbfjrv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2hioiesjp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kstmbkpd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jnheowzu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tyhbkaih.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2adxmxbdt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nugufmqy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2abjuudzj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xiyjgetr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ovoiwdxw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lqmrunef.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hbiyhcom.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2grvswiyf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2udkflpai.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qbudslcq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rlvsbgbl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jerjgakb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2theuxpqj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cfngwjfa.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2baxaamtf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kmzxbhts.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rdxtwuci.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qoyxagpk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yvrvmtta.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2eiqvnvdo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mxhqjfyg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bsblplux.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xnmxbrka.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2myhrazme.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ixdvcufj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2chlfqpcs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ntpwiobf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rbpnqiff.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2cptntnap.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ftzklqia.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nxxwwymh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2psxojzsq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wxzhohte.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xlfiuvhh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2uxaqzyaq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jrozxkbc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2wjihnvre.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2xeeaptki.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kvzuznaa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2omhywsmv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bywfvmkd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fnfcxzel.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jmypsblw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2wjbyygvg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2nchyrwxf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ygzeyzha.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wzvyhbcz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2glwhtnsg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2laxqxkoe.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nenxhehx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jtmnwgxr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pntmdufx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2npirjgdk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2thuhgqlv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gmwdczjn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2snjfvdkg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2nqagiqvn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xiuexnqu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ioaukpqm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzmklhwe.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2skdzouqa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2tpqcrzoc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zcbxthrw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2medzklai.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vawctunt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tfmazklb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2iledpdrg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ejtvwtwh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vlxbhzek.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2evkulyec.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2yrzquhnq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2svsrjppi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hyhmfygz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2gyqifhee.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gtozhnzp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2arohwgfg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zatsfiif.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2upwmgvtv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2raxtgvoi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tjtptkri.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2snapowti.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2myubgwaq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrsyefmu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2cookysvm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xjxjmfxu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2teajzgyr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pkdtihmf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gjgdcwvk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yrdvbfzk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2autngwom.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ehhxjzqt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gcbmdmqn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2veahomit.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2oefphjnw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2orixdsst.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ymhpbvpa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bttnppar.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2phphxfva.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2arovtizr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2eccjhqol.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yicnexuz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bbrbgvuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxvviats.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vvpapkrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqrmgdvo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wkasadvh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pvdziijw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xztsmqhg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xbmusgpz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lffnfgcg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2yfrjfiwr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ettumfwi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqkvnlum.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2levniibf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2znrsbmuj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2cprpakfc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2zhrywgog.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hlrmglls.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2atihbiie.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2stfeiitx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jarwjkxd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2khanuklu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nxjtzswz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jaulctyx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qmqqwlzd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fggdctct.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lzztrvti.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2cswwgotg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cnrnxeer.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uewmupxf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mfigpsve.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xgkekcfv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmzjruqp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2dczzfuww.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hhdzdmva.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wvbzntfd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2oouuqlnj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tjyesyyp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xjdkzgii.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2awvqlbzb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2hixzcywi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2emgnxajj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2srriclii.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dkdlvnue.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2swqupnuk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dzmjglpf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vvvpidlp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hwntqsrw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gwroucrn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2anpgybpg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lxopvawr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zwnyrnse.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oozttxyf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xlmfyvog.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xmsartxl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zyfrqomu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qfwreexa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bfxawgox.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2soiuspgl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lqjqplid.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2agwjdlne.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2yspcqyan.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ljhwsmde.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xwjjrcoi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2urxsaxbo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cawlkntx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kcbpvtpo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dlqocsld.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aellyxaf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jvnpjrzi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xyxhizef.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kezltlqr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dkpsdpkl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtfcfxyp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fzjevpag.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pgmgjuzg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2slgonmcz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bbszaqgj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xaevqabb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mpmopjig.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2onlljqjy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qzrgelrs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wxdyndni.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xegxqtnn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ewifajhx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hymfvfkd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vlmqfbwd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nukrdsjq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2edltkfpq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2gbemowil.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ypxjabrg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uwajsssy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wdmuqobc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2inbnxjar.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bkdmgowd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hoqgrzom.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gnicsewf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2dlvirbwl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yoxxeutr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xqivfhou.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2juijlkyd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xgnoaete.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jocydxxo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mwnnoydq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xfsejrln.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wnougcuc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cjjnzjfv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nscjiakn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fczfwrgc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pnothhji.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pqjglyiq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ctkacgmo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vmoaqkvx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gwbworqe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jrizmdnf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rkgjykbf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnljbqsx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zllhhlra.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kyishwxm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2aclfmjel.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nsbgqnjw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xpltstga.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2pfyndyvj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2asdzyixj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vgjvzwly.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ofutiwys.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ugxmxdzk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2idgdzipy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sfsrsvgs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pddexwyh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2guwehswx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lqbvtohn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkkrmxct.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qqsfmuer.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xjfdjzsb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hmyyewwy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cmeoytiq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gdlzswds.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pvwidmmy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yqmgwggr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gspeekin.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hwwyuznv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fdkaofsn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2nvavjqxl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hbthyceo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2mwdcflxu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2liabbwrm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2glaoypfk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kbuqfbar.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2owuqwchg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zhczuvjm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hywnzxty.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ivsgcdcz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uplcqyfk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2omxnzvgj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xexcuuda.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bdwcyepv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rnxicqrd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qveftmqq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tpbecxrp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wwyqawka.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2iebygbcv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ppspbtyh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2sxoskewg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2sfanlnte.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2nawfgcgz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ywsmfbrp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vqxafhde.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mhkvdmcz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wzpobsnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kitgrcvu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2oyubujem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2narhwtxz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oahjyuqy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2uizkedwr.html


<!-- 参考信息 -->