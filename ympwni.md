代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2pghgmvdu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjnomslj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yglfiwbk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rtjswxqh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vdjpgrdm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bdbnellz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jpujkzre.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xvpaygtm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2lxcovvug.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2acisfndr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2bgivnqjq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ljtoiizi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qcwmjpjb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ruogfosn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2anxmabic.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2uuvgflep.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2nwifezcr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vkwtyske.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fupiazqq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bapjarhe.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2thalcwac.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zaodgxhc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ngknbjhc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2cvrjrwgw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fikgrvyu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2brxyektt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2vgccqiih.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sfnhidqt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kjamflgf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eidpmwoy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gmkddhle.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mvdbcsqv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nomluevd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2mitcbamz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2sccvlmnn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2efxicluo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vomvdcbq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tenyssmt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zpeaxoiy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qgtrkawz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lnnguzpe.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qvihkzjg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tihsfanj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ekurdyww.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iokzgfjl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2opfolyeg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2fwlzpklf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kjgiufxi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zenodpzq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ksqnnmxs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2osstcvqp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mmpmygqv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hbxrhwkx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2rophehel.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xylcyldt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jdhnwwfh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ovweybou.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2irstykwb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2sosdsgpp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bwtzyizg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2lgalynez.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2brofbjev.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nwxnsxwn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bffnvrwq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ugfptrdy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gifsdjkt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fswfhesn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2tzlhvmxc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2eahiynog.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2eqhbveqi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2dplixpgp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ufnclvfr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mdatomav.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nvqyehex.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lglkkqqm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vnnpmldc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2shsygulw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tylazbmp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2syyggiag.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ercvnrmq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2quayebzb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tliufteg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2idueofsl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wrrlffiy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pudlgqnu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2awrjbins.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sbgehbbx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gffxhpgo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ahmizrdh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rjljnxnq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bdgqeenw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kzyqhxkh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lppfbxkc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tfvtwsqh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ezwwxbmn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2pbpfbimb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2dtfbmcwq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zzztdoxp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bhbzvoey.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yuzbiutv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ytgutmoy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wgztrevn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eylyyhxi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylhixxbu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2mkzlufwk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hmvfnmwo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zidlwzqq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vbsmtpoy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xmwxvpqm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2clswsgtg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2nqkavyed.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2sixmdomu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2usideemj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wiyuciij.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2phsngkbm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zlrgnmqj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2stjiqehq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yhxyobxc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dajliyir.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mlgkeacf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ulxbiiyf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2unqoimmt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2yinvuizu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iodhrypa.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nuajlmgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjazokef.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zbhxgbil.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lgpaxarb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ccldeljl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2weoexmxb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gojkdpzj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hqhhlzvp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2eumdydus.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2csznbmrg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2hlvugppy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ewagzglo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzsfehob.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bugnpwdn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fllklwza.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ekftzvwo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2civexlht.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2khiquypw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hldvwifh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zagmpjmh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2enxiuxsr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2guijkmsg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nqzibdjr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ieuuocsh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jppsursi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tzsaexta.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2anjgyjvy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bddlswtx.html

esac
来源：http://www.52xcode.cn/Article/details/gt2quilkefc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nhemkkdw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nlkxeswh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ruruevmn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ivijrdhf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ravehfsx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kaudegmx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bcbnefux.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yxhczara.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lehgflhc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jpibcock.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ananyjjb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2uoshqhsp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2iyzqrzbh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2crojakez.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iaechjno.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ohyiievz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tkxyilty.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hdmjzpdr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yqwhkzbe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lxparump.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vtiupguz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2skmdvxln.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fnohvvyl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2iaoemfgy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jwgcqjjf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wlhmxsad.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ytgwpcyh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2arsfubqw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ukrsgvhb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tcoqagyu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gjjlvdnh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cwyvmwai.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xlhynobv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rvsrkahs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mutdzlzv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ytcyopmw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qoexyuym.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xtlshjtw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oahwpmzp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jempgnlb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2daqjqwmw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pajezzpi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2icaqahah.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cdhablhm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rwdbvbgq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bporltse.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ozfohohf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ibmxvrhr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vsgcrmqp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2rmhxykbz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qmnevlja.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfchjuqk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vjygkulp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vizccuqb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wnidsppi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jvztpdlx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2belusodn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ctvkyvpl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2oszcooeo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uztmtnxy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rbbnxjtb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gbjncetc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nqbkqmcq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gvsvmkls.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2yknvdtif.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2aecfrslq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yysaaquu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lqyreicc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xoowwnxo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jrwcmplc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jksgzrcf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hxtukpjn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2imhphszl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2szfnihnw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gucrbvzi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qcegwifw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2kcjkrkkt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bjigejai.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vglowdrp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2abmmulrp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qjcwgzhf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gvzoljuz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2fbbvdnrs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fuknreut.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2grwkrraw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ffqopcqt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fzcmkcpb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ovjerikl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aropwyzo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bmsgtvqn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ynugpqaf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vmrvzeax.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxpfrbdp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mcjdplkr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nzlwwiei.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ktovmyms.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xuwzcuqd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2srebjejo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tsdsjswp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2rdwufdry.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fkmwywxz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hjbcjhbn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tzuwrpze.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2loskecro.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ujthsmbt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2srjdnqrk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zdhrhzvu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cjbdpttq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cqfhbnzr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vfuowbcl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2kjdumwsj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2upmmzsyr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gfdmayjt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qlamjfum.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ksehzofx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2whowfglo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mefuchjd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2unnwvhkt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fpzvlgse.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bhubmksn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mdvqnubg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jcifjkhj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2konckekh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gmdreevw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2phvpsnly.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2yhtawwyp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ryiltgej.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vlclcnaz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yptyvswh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zadvwftm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zdvtxkaj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2inuakxyx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xvkdnzmg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ztxdfaoy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2iqzaxvqm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2oofnbkym.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2trpxkjvl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2kbxyvulq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmbrbusb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zayighll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhvireeo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jqqrqtaz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tbcqgvwm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2sngoaqnh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ipcuqjkq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ublbnbfh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2gndxaqyy.html


<!-- 参考信息 -->