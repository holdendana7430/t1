代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zkiyktsv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2iohnfxfs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2edjoxhhh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vbjvnkjh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wrurpgiq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2bzmvsmdx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nwhjzguo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dgakmpxe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uozxnynh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2agwhqbgs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vccfeyfb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ecngkfbc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mvsbutmw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ptilfpnt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kmipbxfu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2iknswdaw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tfcbyotw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bfknfeca.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xwiqpibp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2fekmctrd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qktlsrjj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rqswfbek.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2giknwqfk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jtmxbvpg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dnwajeke.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tfdjzzah.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xpujwofp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rseuhdxp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2octpsvcu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aygvjyzo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2kzlxffgq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2huwxxktz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bzypwzbh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kskecxzv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fmvesuac.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hurunwpi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2flvzltgn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vnjzwazr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2uyhulzrz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qhufohye.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2sdflgtih.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kqanenyu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ukkenhvu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zgokekes.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2uvkbjqah.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jytwzwwc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lzrgwyfo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qlyrwysk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2boeiobpf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2trcmyjio.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jswidyja.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ahseuldd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2nwifcjpp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfogxpb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jbupabyi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2khntinfr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fccwuayp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xvxjyxli.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pjnkdrab.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2phsidygk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2odgiiigv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2aqlpyywl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gyvciwue.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2sgayjctz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yddbgorb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2awcqaglh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2azvyouck.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zobjxfoi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ridrpptx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2foocrskf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hvmsxepp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tshzqvdy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbcyxesr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2anoexzpo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nmnftzhw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2zqbfxelb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2emhpqehc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xuohquph.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2locgbhqb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fwzvdvzy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ouhbtdsx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rwvphxed.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ozxffqsc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qwepwvut.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jkqofrff.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tjokvjbq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2eylqkydz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hucpkwyx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2itwtitni.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rtqiszae.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wgalpnvy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hxetscxk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pphgtngj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ehxrogiq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cwjqxlor.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xjepmhtv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jgzuxxfv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ntjytlii.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nygdhonz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kqymzyab.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tjmibmss.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zpdpwftj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ifocansj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2lakutdru.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otsmnbgj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2irofskui.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ozekxaqi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zbbihxtn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2bgvexckf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wputcybt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xrjlsgyu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nczxifah.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vdbluzrs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2brewqnuz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2mccygavh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kxshegsr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vcpymbex.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2fmolmmsd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nwlcyjdn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gnphnxvf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rksdqbsq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2esleoxon.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gswwhyox.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gypbqbbv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nurdjlqi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pvcutkfz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nriuqlip.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ytbagvcv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2axnmjzvi.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gltxkbcd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dnlewkvg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hfuxveeg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wcvhfyrp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jlvpwaty.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ibdolhwl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pgywihdj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2atyedftu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2evvzqlaj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nhzpcbxb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2czplcptq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vqtdxkoz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ntwhsrdk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hpxwrcqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aidbrcmf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uidhujgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyyhwyis.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ejnuiesz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kzvemomd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yajlbxxe.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2nxdkhucn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hfosvzxa.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ezwgpjel.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2fnauvadj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mjunkdwz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aanuntoj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2atogezpj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdizcthw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gdqxvhks.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kecejnwt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2fqwxqufl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ltevbhji.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qtfpnwln.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kapdymtu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2axfcffzr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zdawosng.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2wcroocpw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rnasurkf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nmwbmdwt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gteujlyu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yfizmhej.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jmxfefxk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bzqemfgs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xjqkrbdw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ieplpgml.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2foinzvzr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mbhukaba.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ttmgxucs.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nigsjgmq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbttxrtb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2auhcglcm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ocsgvzzf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2obvpcqmj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yxgacmxi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ntudyhdv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rzhwogjm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vskhbowx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ztybzctw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2puifkvxd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nokbvius.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kmzlzobp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2efdwftab.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tkzqthla.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jtydilei.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jfpqgppc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2oftuvchm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jjzhfacy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2knmrzirn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vgbzshgq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ecczahem.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wekmfcnf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcduqtmz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pqcvosgm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2sayoefxy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2czrreqnb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2sjnpjxfs.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2pzglepjm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jfbekzge.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbsnairb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jaopvisd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ahgzwrqt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pqnfemgc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rzueftmb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2quwnzict.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2atdwccpe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yftpoycr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qxwkyxkg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fyjanfwl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xcmfmiay.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2feuoupwr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vklysfzs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pzobhnmp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2atfvosbo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rzpmzrto.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wchaypko.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxjbytgj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2cpaqkrmo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yulgthyk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dptjikou.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jjefueuv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fcqkesto.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2clsayptd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tfhazqye.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uxgooklr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2puarmeur.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rncikmbg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wfpazjxt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hlkzluav.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fvtgtqkt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hgekhitc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kogkpylf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nrgzpcbd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ooitnixi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uzmkztaw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2karohrux.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hoczaplp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ghrdxcod.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rftdvurq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bedexkgy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2akselrzg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ixkqtvrr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mcbkggpk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gibglswi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2prknhwyf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tkxlbhof.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tztpcnrz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sinabhfq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2lifasumn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lpjegfzz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2llccgecw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2oqukvrpm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2oqhbeymk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2joelgvxm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2btssgdtd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jyofyqxq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jzwjevpe.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2adhuzawe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ghgdfjow.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2epnhnjfj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2djblbgzw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uibauqbi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nhwwkwyh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kchtgwcu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dbzcokfd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2suyzzxvs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cluaftur.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2aklzyuvo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ohwztsqy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2eppsrals.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cntplagm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pessjxle.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bugqhebf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xablwtmi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qsyvfqst.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2eovhnapi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kjdfnofo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qibleimq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hkqgzmpi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nrbjsjix.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lheadslb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2txbkivaa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2cmcipsie.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ccfpntjm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hjhdxdrb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2esubtjdd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zipxutaa.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nporhznb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zfiojmfe.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nyrjrhwi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2pbcjmfrc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2igkrddqx.html


<!-- 参考信息 -->