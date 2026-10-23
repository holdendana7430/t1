代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tysxmklp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mlqyripo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xxaszjqe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3czhcmghz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gaymvduw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3exhhubja.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3unhletxa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zrphhrsu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3gmpdhsft.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gxkvknrx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qfopnrtu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ifkirzig.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3gzafuhwg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kchnllmw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ikdgyjbu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mhmrocig.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3jcspbymg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hrddvgkt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yhspqhgq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xycvctig.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iguxzqxu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cvwmycls.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3oaimsyhw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3oarmlrbk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wxtpnrfo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nwsfapks.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3odqumzzs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qawopbiq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xhxxvyiy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3khouhstk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3djeyvlgc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3rkljkgyc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dqtuhezl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3fnznseww.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3aivocxdo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3njzahkne.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fmqsorog.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3bwagwuyr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3susztzcf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3lwlcrgai.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ecwrnvrz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ixvseqmg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ksluyjyd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3aqykdktj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oybcopws.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3utzzkssu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3iygusgsv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rqhdkdfa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mxngnlef.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3htcnsapk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rpxykiln.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3dryjjcyi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fqkmlutd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3uffbernf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ljqdrjcj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gicnpagr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xyptguee.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mmbwypai.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lyinmnbm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3leiofrhb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jrguyogr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3clvmqekt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rhpfpatk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ezjuuooe.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mfszzkol.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gnprxzlc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3whdqliuc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3njencccp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vwebrszm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vehtmkom.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hdpfpazy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ziebewgp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rdcixbcu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3abcdvwmi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nevwtrxy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ffzpepgz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ntkayccp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3scsdrtgh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3vthkdltq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3gbzwfzjw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ugwvzgxa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nearsoqi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wurhrmeu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mgupfcfj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ryujebes.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3abewjhlp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kmibxchn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3dpdvmazt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3jiolrbar.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3trhvbczz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3itwtjdwb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dotekiyf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xwostxhy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3dpvfmyja.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rchhiwab.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ixfpfhcg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yokjftzz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hszqflgz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pujtsopi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvdpphye.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3tizygmxl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3livtvako.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jcxmklva.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iochogok.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wyorgpid.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iwnejgxb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3yrrfumrh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nkropdwb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zkadusvs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xtzeqsls.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3epzkknpn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lgrfkfxe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vhfarnwm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3eqxltwie.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iuuirymd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lsakbnog.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xsfwcbhi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3sraiomqv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yjrdzrzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gaksfuei.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pqxmcuvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwbgajmh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3grvhwozr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kiklctcj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3gnpsucfw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bqwckijr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3sliggfxz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nltbltbi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3fyouptir.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qfyjnsgx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3pnzkotdz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ilxkvxsh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ngtmvydu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fkriknpw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dshdokts.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkrajxte.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tawouhfp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bdenaioc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gqljqbty.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dbabmpsl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wwbryoqh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qdjjeewb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rsivnorf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gmvjlolr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zzdlykko.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3adnqenfo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lvaqrdyp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bfnhhqqt.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gqyzhhwn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujtuqxws.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wikzkjwg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dzuldzjj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zrqncknr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nahrfvph.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ghqtcwki.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zuygoqcf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3dkftfawg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3heshhxqt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dlvlqyff.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mfbxhwrw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3csusetmi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hxfjdfmw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nfsveelg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gnmjygof.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yygyqkbv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wpksmzqb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3adhrjipd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bmpizlak.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sxffgotg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zpjoltzj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ezlpunfc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ctqdrxph.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3itlpflcb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jesbdpie.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ejkhyuab.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3iodxivfj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3eqmszwkz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3sgwwepca.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3tcfvwaqx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3eeukjfxn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3urlespjl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kzhklpng.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ajlwbngw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ppetlcvv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bhrghpyp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dlnpdyrz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mroeqpgu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptjkllgv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3tncoqsgl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rpxzgvso.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zniorkpk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wgqwqwfb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3sncgznkt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ekhxcarm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zqxodyls.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wclqhdyl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kanbinqq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mdpaaeaz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3vrtsrncy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ylpvkhle.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ldsbjire.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gnfzbgal.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vvzvowgc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fsbijmwt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ftcnbiyj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3amhrsmat.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ihmaiooc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gnutvqki.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lnmnoceb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rldbmdgc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3agadvcqj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3svazbahx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3kpmtgnem.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fzpmypol.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vfndublj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qugejiad.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sycbbtgj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cyrljrgx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3akiblyfs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3aupmgqjd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swhdvcqv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3afcoatqh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cfytbfle.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ydmkugll.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ddhautgh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3flsynasc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3duqrbrgp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jwqljoup.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3giqrvevv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fjltfkwg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hjhagfeg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cvhnxyfy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3aiqcsjij.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ygqgbtfx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3uqzvhdst.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ytdippki.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rulkwipg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ozosxqlx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qikiqbjz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ylpqbutd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qegmjzqb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtodzkcz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hxoflkdv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nveecrkt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3udjuqfph.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fuelqwov.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3duxegmbz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3feyvvvgu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nkkesiac.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qibafeoi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ififekmz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rfusafom.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3auhoorev.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3fxhnybay.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwrzwzu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3snkgghxj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kjxkeotx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xmtxmkle.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3veqyuyva.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3bkvszwop.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3orlvvrot.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3hwnejfzs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sipsywru.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3skvgxyln.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3baaydrtb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qeqgrujo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3smnrddzg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3moyptgfq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bpzonctd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wkpdwneb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3oqhhxigu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xbsvqmby.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bzpmusoc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3axhtksad.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wecegeyj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lxewnitz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rkujiley.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lyekftwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qrjhsrba.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qlgosblc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xvexswqy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wvdmsgsf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tigejyln.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rpxwqdfl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3uvmjwooq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3brgrdjwd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pnovqdlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohkjgbjh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ojgsbaqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkkjgoyk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3owaanaau.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3thrtfzra.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3abbuozdp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3eycbczam.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xrcpqwel.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3edbsvnwh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zjrqrujs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wdorajpg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zpibqvpo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3szqcfwen.html


<!-- 参考信息 -->