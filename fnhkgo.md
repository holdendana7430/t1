代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pvkingkx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fhwtvraj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yxohinsj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3muklbgyh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xnbxemxa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cdftwvci.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dcmylozc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zrxadotn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bqjsismi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ukqiulic.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ysrsektr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3holbgjvp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3egvoiiui.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3irwpzisv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wjoibauk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3yrcjvjoc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rxnmfpnt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xalxuxpq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kuophsid.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mctxwlsd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lpumvmyo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ysofcraf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3oxehgixg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qnjblcov.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3erddntgb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vyziqkai.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3spmhunjm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lzbffckf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3pnghuauy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3amuvkxpq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3jspgtsmv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qwamvlaj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3meyiodwl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tsxecqdq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qxddzoir.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jnarlise.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ytjxkhyg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3yntdqqff.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ixvwevgu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3eisipgze.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3awaulxms.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qeyynsos.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hhzxhmni.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lknzpdga.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qmobioxa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3upropfak.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3sqwsyzgk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ewggzwlg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qdjkqlbx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3inokufez.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fvmrkuhw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ysbtnkuv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xbotqegg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3oevlkcdj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ldpywfgn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vahpzpho.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zbntwrjt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3swjxxlzu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kscsqhky.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3eyhipure.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3akoqaanf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ugrdfthd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3scaosvwf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tqmspbye.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zrqwchfd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3doajmyeb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xxtmskbj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3txfunjuv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3feuofunr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ewunhynh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oqgngcpi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mxmbyyco.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jgemcnfv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jdkkkpzu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gehtzkdu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rgovvtwc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nwxqtjnj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hzcepjyh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bvqlkkud.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gtlwxsao.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lspsycrn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3vvkaeqky.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3hdzujbfm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jojwiexw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gslkkakn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xcilcoyk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mnhtzbei.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3uhpejouc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3udazsovr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jchlmxeo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ycvzbxzi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ilpjurip.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pimubomt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jeqsgfxe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3aqyjejso.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jkthdgdc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bmpnyfmt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3auwtkhdq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zvmvwllq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3yaykfyta.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3odzxvlfc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cycmaqun.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3umzlledx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wgzvwqki.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nyalazpb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fhxfyzsb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ephizbup.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3lanwbirl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ncgjswfr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3lcbzrcxk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3bfvwbxee.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3esgsysja.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kegrxkuc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3uflkkhyq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jlgwwntr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3sfnwgkbt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xbmrpbfg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhdfrbjp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3khkcpdlq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qymxqexk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ywoalzpb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3phngkfpb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zybhlytn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xglouluv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tpduppzq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lciktinh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ilpwisde.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zwokfmhw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3cntuqcln.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qraetrzr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kkvlclpx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3grawpbfm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3kfxvbyvl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jopdommq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pwovpayg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tkrmpczx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hgjxcuuy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wwlenthc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3efquukhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aoprmgre.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jniessrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxxavkat.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3umtvlkgx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3bhcjooxy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3dsahmhka.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xgqrphom.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3mkuwjdnm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ouumrhym.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vcqylwfh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vrenygol.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mlvcvyto.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zcwuuunj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3pvfjdcpu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kkrcyxek.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hfumsmgz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lklxuucg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qkqymily.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3defaokqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gpkzczgy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3otxikmlt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3twasjgec.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rquskfli.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uzutrspb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kwkozizn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3prxrlten.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3qvbzylzc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3haswvwec.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yijxixfy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ahtxdrty.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bpljcdbz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3urluoyfi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3knxgcnep.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3upcyvmrk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3egzptkqy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bomhqyhn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ndycwyhj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3kgqyushf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3veffnmyp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mfchpyft.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rbgmpfgc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ljzpbhhf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3neuloudz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3awghhcan.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pownxezf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nftozfys.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3pjdmhgtn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nadzlmvm.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3obxxttin.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nzfbzcgx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3npxjytni.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3akuqfhlf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dpiupesu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bfbeukxf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oelvtznd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuddqciu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3iposcvci.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3embvkdfu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hkcdxtan.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jvkuvdtv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qyszycxg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vuhduutc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sybtprkq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3shbjlodo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmmvrspx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ogfexgdr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vzmiknfk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3tjaofymt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yyudtrzy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcsiucwa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gbtavkqg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3grwiaifh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zspnrztc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xeyifzkz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3arpwmaam.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lrnlcywi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zataxyog.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3fxegwqah.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ijvshhiu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3byezscft.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xdrzpnoq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvnfkshj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3diwpqwgh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wcoqjzxj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dlqikccb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3akmngyrz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ruvpbxhv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dyxglrjp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fgnjtxxo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yajdxmfp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ukveuwdi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zrvltejg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihxqimlu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zlqaedhz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3sgdikpph.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lhytphic.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ubxvhgif.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3nbkzlokr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dsbdrswp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3sdrjpndn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kazxnzss.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mrfgeinf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rbqaccqs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nyrudzhk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xwmocnex.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wllohwja.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jphofwwb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pvkmaqrx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cbshliwz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ywqulgbj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nvttzudg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ptzryzjn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3wocydleh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qxupmsrd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bopwnzyg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qtupmwsb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hgbbuped.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3biwodkub.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zbjgltan.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ivaocjxe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zmvchsjw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3yjfbakox.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tbjjiotj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3usyfynvv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oerwvmhl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3nwsfqnsx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ualxhhdk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uoaghifs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hrmikcqs.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3koifaism.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3froswwth.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3riyaxdig.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3doxsbjee.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zjhwndli.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ckrfvwxc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mrfzrsvs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ukyvydve.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rfqbgkpp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mgticezx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3btxzqruy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ffjsoyty.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ohyfrdwk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ebxvrvhj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vhzanzjq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3aadpvamn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3psoqihew.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xhsethjp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fcgunyxx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wrgtrghn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hcrcrmvd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3aajhthmk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nlezhybl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3tttrdkpr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ujlucfjn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ygxjlgyz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zftqusuy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3onfjvics.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ugvkxosn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmzsoqbz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qvnecale.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3rfgrcbqp.html


<!-- 参考信息 -->