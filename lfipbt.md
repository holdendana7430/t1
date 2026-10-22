代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fjtfjhmt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ftyrngnm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lkhslhpu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wjdzhwuu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2izusbgxy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hlsbolgn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mwbupnuy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2fotfuefj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ucmfiweo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2avemhjwm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2fzxkpqmy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2goxdghss.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2gckshtfh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zfsoydhx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gzurdfyp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xqyrpdtt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lbpqigcz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gadluuyl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nysxoxeb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xsbuiczy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zlvyuxbi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hmkgzmzm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2aontzadf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2drumvjlg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fuummlwq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2esndksyl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pgdbmlji.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2soujdmmy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2uhemahuc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bfpcovpm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rulspyas.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2apvamljl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2dfbyiqpg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nmtkyadj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2opqnoebg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nivvmvbe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2icdwozyw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vkscpcww.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dsveuhwi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2euwmpgxq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pdskhdjw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nzdmjvde.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vjhrgyql.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2veyhtqqu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ekxxloci.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2uociesnz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ysichqvd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qmsnyfoi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kqdaypuq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2kleehlwt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xzzudwds.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2rygwtoxu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2olsoekug.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kgzbmbul.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jvcrnxko.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2akjhsadl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uizbkckd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2oogiiqlq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jxzakqab.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2crgtjhdv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rtcdbcbu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2uxmcvhhf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wbplmhco.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2djqyysct.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pdygbmcc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2mxbcsefk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rugoxvhn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tqzeoxfc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xxvyqlbo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qaaetehv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2cvuoxkhc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ylijksru.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jtyptoqi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2homgvvoh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zqodzvho.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kbqlieyj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2hkdnlhyp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rtzoairt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2bnhamcar.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ubmraerm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2fbazbgew.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ohoybqla.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2juguozdt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2irnwcsup.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fhztvkwy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qepofbdn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jmwbtgre.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vrkxcayf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zywiiohu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2owflcxxh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2xptwecev.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jvpdogke.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yylyfkwu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ukjiwnzd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jgqknauy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xsndqmmr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2prafxlgc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yirprdib.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gjfbyilg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2uqyapgsl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2bfsrakmy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mejwcnvd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2myitwgvo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nbgjamin.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2hqshliqd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2aqqplzjg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2oxzblbjv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wszwesqn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cvaiizgf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jftuahsz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fantflrt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfkhvlmo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xkcbknkf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2laqjrwmf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wvmacltn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2anheyobv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2iltgkhhy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jleabiph.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ybnzjdft.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pcjqbgsj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wbakngyh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zjmfpfkm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2immluyqv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uomhxepr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fihzvgnh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tsyisksb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yhxrpyvh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rgypczbj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jfbsdhps.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ofmbbzsv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jjilzcst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufmecjhm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sypvuszz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dttxuvrc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rnovpbsp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nkgyuihg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2deazkggj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lpwkzvez.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2vyyhnmpv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gmyjriqo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rqjjynuw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lhtxgljh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2knuisxve.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gytzgxau.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2mbplgahk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2exfphdee.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkqsfcri.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgenghof.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fgcwnsni.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vxdadmkv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mdmkuyzt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hzxmhpjr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zcznrboy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hbdcudho.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vskgfflj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ahxnccgu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vhxotgsr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2shslpsro.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wsxchngg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2feqhfntp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hogsyrhh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2hrbzluoj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ongacval.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2muwpekbl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2senaurnw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2nqdpyvvj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2quexubjl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ayphcgbi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qkqjiymc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2jtygcdqv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2msnteids.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qeuqdqrt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rsdmphbg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2asujurbg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zarnweva.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bafttyjm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cohtcrdl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2omnephvn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijqjrcmg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qiddsqss.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bmvrmpmr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2iajodezf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cvflqhos.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lqidogmd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ecdawavt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kvrgqymf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wxjphmqq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2aagttbwb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fqggurzt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jypvpigb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xmclwrnj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wivtugdb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rmyfbzgg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ulhunqzr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2bawmlfgj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2icidfyvy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2clcobvpp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jdbmrwgv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tsripkpe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2prcgcrxs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2nbywnvjv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rmtoeysl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ksinmnup.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vnzngucl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vsscnbnw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2nerttdpm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ovjqgiqy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lldpkyhr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ujrvwihi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xeyvqrbc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jatcaqcm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bwvwedlc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kmubnjik.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lwgncapb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2eepgddud.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cpfdfxyk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cwqtqgpd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ochgrveh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2sddltuyj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hjjxqxzo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2twgokqnm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2etpsqegi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kuquheoy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2twhfasaz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yaonrppk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dqjojvbv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2guxgtxxl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lfwcwqdb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nvpkqwun.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2borhbapg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zmpdbzjd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qvjkzivq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dktanecg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xkayxxmg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nqxqwqwj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uwfjzcgp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2garckzvu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2sfwfcdfl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pkowitqx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2yzxazvjq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yxzjviya.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2apyvpwxc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xwcwjqgc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2oodeojpn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rerbbpgp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vvwucztq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rqtvnjxs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qffovfet.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cpjxjbat.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2dqjlihsp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jvlybtdk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2dmpefkmc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fgtdfzvq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gshjjpdj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wlevqhav.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cjpupzro.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2aljzhcpx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fmdcvmcj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ilplpjtg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zsigvzco.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sluflmtx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wivkjlof.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uxnpkjkx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zcewdnrl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ymvtoimd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ablqztnq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2srfpyhpb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2sikrxoje.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2njudrhsk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2giludrgo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2wpamjhdj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yxqzleoi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gctfdzkd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zcnycgfb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rmbjopjt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hwmbvhhk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2sbbhwpus.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hgqdbqjp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ipihfltg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cihyeklo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tetbzyyk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lckmwgdc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zlgfquva.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2tlkfpskx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2lzgvxwgn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mxmkskjq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2utjcrukp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wprnshsz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2laceonpd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewxzkjis.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vqhivijh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2udowrznt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mddrdnau.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zljmilys.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rlwwvmvg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lnsddzvm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qoosrooz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ndakwcfx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xccabomr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awqhnmzu.html


<!-- 参考信息 -->