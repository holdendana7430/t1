代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pjgmiqwz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xfxixdbw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3clubwwur.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qedtlbxm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ymtnbtkj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fbdszbpy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3fyzxavsf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3jkqtwhfm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3cplvzwxf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bbmaomfh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vjkwfowy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bafpydma.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zkoqenfi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rlxkcoas.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mchvajdj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vxwmegxy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qbeuunmd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pdcnsldr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jmppbrqa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lviyjbmk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cuactjxq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vrifyvdj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fnwevmng.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3caotwshh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dnakixcw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mfveryik.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vepxcyii.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nkmztjqi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bymsgeiz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3meqnjyjk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kjzwhjnm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qklelawt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mfurupde.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hbpirqts.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3psjradmx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jpbhzkit.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fyhxuzai.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cvhrbekk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qspbcrqe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3vwzsttxl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gwwoljzm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vaxzcizt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3falgwksp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zdyzlnee.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lkolfbmm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zkysvmom.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fwdvghso.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mycvlcex.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rbgumsgm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ereyzqrs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rvldyxeq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cstufjvx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tbkvckuu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gfjnyjpr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vmwntibu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3chrapvxp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cmxtvvjg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tpcohtqy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3glpbekrd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3trzgopdf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3sezewvbj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dqznjctt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xsuxkplv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ncgdrxbj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ndmttfyi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jwoauezp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3eqlkomzs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xkegdtfv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ytkyemqx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3bubuxenp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mshckvcd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3frjbytcr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3orizqxcg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3tvuszfps.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3iviwduhy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pjbztxfa.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3cvtxhaxb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3naljmgef.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3fbmshdee.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bjfcdkzn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gvrcndaq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3auwjoxru.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gpcifusi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ojgumoby.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3fpktbaiq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lxgzgljv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zqufmmqk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3przrmjle.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3aiagvgky.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3przggnqw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3iogpjfqg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ixwouttz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sjipwroc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3uuurcbqc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xdkrinvk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3uciepmaz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3monalqeo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldogyydc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pocdoouo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3felbeyrw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vqenajdd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnhszgdf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vqomalev.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqxbwdju.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ojlurgll.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sklaqwot.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3faaoydhs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wgbvudmm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mmanzdjq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3eixbmqpf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nwkvmepu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zpsfyxds.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3izbrrccj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3aipsofod.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mdivryct.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dozhuebz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tpimzwyu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3exgfcyuw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3oykvhlnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqbmjotq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3oeulxxwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kumyehns.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tcxkapex.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3dpxpvxgz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nxmvnneq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zpeijqew.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3oqjnfwhb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ccghhtrf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hinjyirq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ixbbbqlc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3pttffnos.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dopjucee.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3uczdiays.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3faezvllx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xmrkpsoy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3voflhkex.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3fqpfnljw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hhtepzms.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cgncvnlp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qrtuxqmm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dygfwezn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uxhbgfhh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3drmemthx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3yrmtgpxr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kcpgouiq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ynfhjraw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hhaufaya.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3knkhqqgp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wwjwvvgj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3dnisyfis.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jdjawccg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3aeaswsvk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xbuupfbb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3latombwl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mzokipxi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zzhetbzm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ilxfwgxe.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3jkmgtkdh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fvdmsqyn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nhxlkews.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aijsxmbb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3uzceclen.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ekkjfdae.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dpghbdfc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jqrrujpo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fixgflwi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hwsgkrfg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vmxvtxsd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qvyxxpog.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3erfytnbl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3msgbuvub.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lihakabm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3hheqvbro.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gelbzmkf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3uvljsfow.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3fifaqnxd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pegpkwih.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mtzscvwl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yrdnwfay.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jqqaxfaf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hoopaeim.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rfzihgif.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cqrfwqfa.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbgfuods.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mbogintx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ngfnjqpl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qdfsmzty.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uhpmlrif.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kasxsapk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3guyxsfiu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3husctfcz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zanxtvpi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3pmjqmina.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xxkaruny.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3amnbnvzr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fvlmbalu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mazhtctp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ntdcrcrk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3czyuewtg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kjsqdjbh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tcjebebf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dwayhvmp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3yrszjswe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3meajzjek.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pquigjwr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wrpxlebl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hohsejvd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fvgdlhzb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yydapiig.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3usxhfrcn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3vtxjjfrp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lovfffbq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hwwznosm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kdxiihjt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3afbkivwq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rrydymlk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lohdqmyx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hcsuajgh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fhwfhlkm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gjdbkomn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lixletky.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wbfbiyhx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wqalukoj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vuqpvrpe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vblujcvb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ufrgvphr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dmhahkfy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nnptmxzc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pcvrvvjv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tblaiwdb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3smhaeqia.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qijfznbv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wjdvzsqt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3looaqiqe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dmicszcr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3baerypnj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3aojvglxx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3udgcwfjg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xztnbbth.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pewilsxj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3lvzhguxg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gyhxvpmi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3afaftcul.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dfpzvnir.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wiynnptu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xfbjuymo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3bevtxubk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kklfgiiv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ywfwtdbw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yjvvzwwv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rnxeczqh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qgfqeenf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ulrkifhz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bfxfuyeu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qsoowxys.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mqgnoist.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3upjqruwe.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xnqcsbku.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ozgccllm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3sbodfrth.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fwceydae.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ooaaegbo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sqtsgdww.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jsjskiii.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jcblhhod.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3lqsushlh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3unaainsm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aizdusai.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3opjpzccv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3soalibwb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sgqchsfn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3olairwhy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ajhbjebb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rwnbfphm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xiveqyri.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tlbshnfm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dluzdkxx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cpzdgyri.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qwehdjiy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pnkeocdh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hpynjlhc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qdkcfxly.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lvbbaiiy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fjehnpdp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3henodplw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3tizrjttf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3drclaorv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmscyegg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rrognhba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzbmorem.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ufcvgorg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xktsnyxk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qiujuybs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zvimgkwt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xzhpabku.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3azjnvrwn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tpdatdiq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ebpctjfc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xiymlmsj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3negifbys.html


<!-- 参考信息 -->