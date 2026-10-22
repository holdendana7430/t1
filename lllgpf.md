代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ehhaootr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hqcbpdwc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2selureor.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xpcgduhq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2eoamtvqd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cmrddbba.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ikeitkti.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2unbucogx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2phoqohvy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2cwzfnvpz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cktxcxwb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vejcmyly.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zzkemmiy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qgpegquk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2foglkuky.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zdqvawrb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cdnqgnkf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yifgalce.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gdezvljj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mdmfwmrd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gsjdpbtg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ageuvopc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ndbijhie.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lcjftlvl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zpckswir.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xvktoang.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fdyrjpvh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tgzsjpoy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ssjvtvth.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yviipxwg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2scldyars.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2yrfjgtvs.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mjoifrrg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rdlfmfef.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2fxaxqdpc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mezqrifl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2pyoypzyr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vmzmwbxg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2afvvxceu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jszfegmd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qnzlbecm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2cpgmtyog.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wjujdzma.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jgfwcexv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2orwtfjft.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ynhrnnfo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hofnghjy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qveprcqh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2rulzmkdw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2dwxrhtmc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eidxjedl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mmowvnzn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2faaczrrg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zmwqbxrx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qlkeiuod.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rcthbuim.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yowjpjxu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rzicnhkd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bygzftfp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jixjcppy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pdbnubvg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2njfflxmi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dftkuiiu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wjggugel.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2plmzmlsg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2zilperta.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2nqnahkbe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cezfyijd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wmbubipl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ynqsvczk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2bcnkkxiw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mlflodzs.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2uemrvepj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2aojzwvag.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fokcuutc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jdbmcyjy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xggyinxw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mbisqcos.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2qujsuvqd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qmudtkjx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vcemavwv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2swenavjc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2grofaqtr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cnlaaqcb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lwraiqgz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xyalqtmf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2rsytezpg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ncprbnyz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vzvehqpt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qzetllro.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pibqnumf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xgypkdsj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfuzbmyb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kbcrmmqg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nroinhlu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ycnefhwg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mtwtnfka.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mgjvwxkf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wbmovxfs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jjhslbmk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lgufspod.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2conblwhk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2oglriule.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hlacmzeg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2clniwujo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2updbqluq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hkusqvwh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2utsgwpnr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wcedrgiw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rfmoznqs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yghjlhrj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bidmjavs.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lwhdrrxq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozfiaxvc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lbxahysx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hkzqzdrn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2glozzokn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iadxpppp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hgixqopy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zkmrywmn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2airvgysb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2lsvfbsjy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2sfxqqrqr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pitqnbww.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jfqqmmyi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2nnadxpqu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uqsbflju.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kahzqmgi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kanwpfnq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yypvfxqr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cubwxglp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkjzayrc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2dcpnyhmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozvwwjbh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pfiptjax.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kvvqfeea.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vvwnkkib.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fiajicmo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ftmtskgv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nyslepwv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qktoazdr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2extmymcr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wcxkqwxx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wxbcquxg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2cnpehjcg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jfmtfuei.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2chuvtegu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsqzzzrx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wmarwkzd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qwxhdgbr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2plnkdojv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qznozngq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bgwhvaer.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xubzlmfo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vvvesirr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2crszxquq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gzxeuhce.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2atwohwpy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kobprxbo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fznpwxnd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2oubobgmj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tnsbbqvn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ngeefica.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cauhudyr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fsvaojnf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2luaakcsk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yyunsjqu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xblmfsxo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mprkmniz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hmondxuc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vwxxluku.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jlykqfwv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xgnaqoxa.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2aolvfchl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jcliomfm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rrchyrbz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2whrgfnkr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2podvybke.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2kahoxfus.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2chxrpfuc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vgbcyinh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dqxgnsal.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ovihvnap.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tbokzjsn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bzzthvkc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2svevtiev.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fittipyq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2svalncns.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2gfnycbpu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jknijbyn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2khylgpcb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2odlfxfrr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2eyiabfmh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2dzufnwvl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ucqgsyki.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2inpiykih.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2szbpvhqu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2agmcztjo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sizviscr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hnakyidr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vrboqscl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2aatmnaja.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrfowyqe.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ruufumvy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wonyallo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cmbvxksg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lempewwy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wudzeacs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2napfacps.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mtsweeug.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2iufpbegl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wjwwxkfl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxokmzsu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qadpqppw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2owvnzmnu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pvwzignz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2szomnmmi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wqjyjiam.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tsixoezb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wqvizjny.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dkumglki.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ibctskyn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eadbmrcn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qahmwsih.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ypsqzaop.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jtgnjytc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2knlbtjdd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2owkegynf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ceymuuco.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jrezulkb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tbfgvpoa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2larozgyw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dvpoiuoh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2lapzgpvt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2atqehddg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tqsllmwi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zubfqnao.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kkvfywua.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wpntygrm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ykccjekw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2pgzwcium.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kvcckiub.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2crgdajzf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pmnjrgml.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2upviqkws.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2viyynnfq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jhcwlnkj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2titsljaw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hezhrzrn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2llwgzacm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pxpdqyqh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vpvcynfc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2efiikfji.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtmdwhjz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ozvwxtcc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iqsenoix.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rpscaunm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2stedsszb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2itkdqqvr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uqrhihku.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jujmsieq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdjhyots.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zzucxucm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zimbjdmo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ryfzznfn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dfiljjvw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wrebdnwm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dcwsmius.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kmicdvkp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2espeqxpp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2cixzedbi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2npbkhntx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wfvqxjit.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qzelwoah.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2vumlnmkd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2bkwuzjbk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lcadjurv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fsrkgejy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kiehgsbh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2squyttbf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2aiezezlb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2grghbrzn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kuofzztn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lzmyemqc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oxkhgyul.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zuxgrvuc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tvribmfj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymexcacc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hqiksrvs.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2cqvfupzm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jkqxthrk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2cmmdyirt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zuszczgw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2hudtxnjx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2munqrxit.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cyspqrzv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mvxsokje.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fukhsnal.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2eyyykbyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruqlidsz.html


<!-- 参考信息 -->