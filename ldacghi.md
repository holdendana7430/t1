代发 wailian999

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/guziflmzg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/geezqlpie.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gokbzasya.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gzbetvcsz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/guvscnnnx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gnwqetzdy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gqtuyyckq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gbuwkiwfm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gprktvkoy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gfplptmtn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gychfggra.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gtvydkjki.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gbbboijmk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gkxollrsk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/geprpwvir.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/ggfztkjpz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gopetqsqw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gwgehoijk.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/geswcieax.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/giafkqhzz.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gzgnnzafa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gpplqktdy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gwrrieqdq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gjvyflsrn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gplvktyhu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gqiqwjnek.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gxabizvpy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gkkdngjdw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gczfsxmkp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gsbpkpdct.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gzedcvcdq.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gmgdejagk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gmuhjfbvt.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gcgzzrzhe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/garicgbbk.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gzectcsey.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gdyqxwhee.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gakzwoarp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gshdvhefl.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gziizrdex.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gpgdfnwfb.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/ghmsbfnrc.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gifjgvtwd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/guwvxnyld.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/grldcsnmo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gzfnadawu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gbmgvswmn.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gbmnxtxfq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzjftphqi.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfdhrix.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ggzdyxoxz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/ghqunubuz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gzbukjgpt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gygivabeh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gemhpogvq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gcobcdrbb.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gazlphfwr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbukzzivu.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gpabgstbl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmfeyvjbc.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gyhjcwpet.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gjtbrukgg.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gipqbpnxc.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gxyfiweyw.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gzefaexvm.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/ggxfpjgis.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gndgfwnfp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/godizcufe.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gzljrjftt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gfqvfpvwz.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/guqhqbuwo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/growfwkod.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gzljachyn.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gzwuzglge.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gpapqufeh.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/ghqktjyrv.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/guygujsve.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gldsvehth.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gyiqfyang.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gqmmnqgwd.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbqhtxvia.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gzvhlnbau.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gmjhmiumx.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/givjzudem.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gllaexnve.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxamnxvfg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/giiifjfhr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gfpcscbjy.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gvbdkqinr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gjilvelqm.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gkoawlabg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gqujtbdkm.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gpntfcrbn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gayexjeqb.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gmaoifkdq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gptveqeif.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gpcbomjxh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpwzldttk.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gaeelopfy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjnxcjtnr.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gpschsgqg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gosnhsohu.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gxboyomjz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwouaflko.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gpawxuxdh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gczjlxtly.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gzigfvtbw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gxamyqbtj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gvcsjmmla.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/grbyyvvaj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gsgfstnox.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gmprujgjz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gbevrdkeh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gucqndumz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmkyljenc.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gcsvmysxa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gvkzowakv.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gmpmczhuu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gpalaufoo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggwluybdb.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gresncgkj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glmlqxthd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gybvrmrau.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gyypvnouz.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gevqprzpc.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gimlxmuoa.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gduntusfc.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gxcycjrwh.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gzdqmfrhl.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfgglswsk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/grsgrhiks.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gmscrqzpg.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gdepmooqz.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gdothhigw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gceirizik.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gvelrmbsl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gjkxahmxy.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gpvytrsgd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gcamgzgxy.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gmnaorvmz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gkmgwdygy.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gsppqaada.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gdzlvnhed.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gltazrzod.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/glwhcaqrh.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gltvxxjqt.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gsjhiwdqc.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gjlmlwjob.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gljityuqj.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gsigdnuqr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gsufsqoss.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gqoijjnjy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/ghitlphsa.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gwntuores.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/grvnvzdts.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gymwhlyrs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gfqelneno.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gewuilgnm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gictvaxrm.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gibyjxlog.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/ghhwbivuz.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gbjazqrau.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/glzmovjtp.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/goyzkkdll.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gfnlwsdzq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/grchhxxja.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gvcobrpdf.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gmqggpsxl.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gkmfuarus.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gsboqxrzn.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gadubqemv.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gtyiksrwb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gnrvoxztj.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gmhvpwtxf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gojmvgbuh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gdjygvewk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/giuissrms.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gmtxphyxw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/govaaizek.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/galmvxcse.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gmyuspsee.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/giaxdobcm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/geiywsvnu.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gwqoehcjm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/grnsttfhp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/geqmkfxqk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gvmhjwmna.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/ggmcxkkzb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gblraymmg.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gwwfbmsbz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/grsmyabcg.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/ghvlolbuq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gepndyqwo.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gluxnggtg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gkvfxkeou.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gfylovnop.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/goyyqhbvt.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gvuvtktju.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gehuwyovq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gjpjrtoev.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gzwtyhmpj.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gmnzikaaz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gkeapfhbn.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/guruwzfgr.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gnruldtev.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gkmcvmzyn.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gbjyraexh.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gaqpnhjki.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gnllxmjde.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gtoskoovx.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gcbsnebfd.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/ghwidzaip.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gzanzynkq.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gxudnjiwx.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/glrkvtczh.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gpybyigoi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gqpfjomba.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gicambpbr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/glyndqniq.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/glmhrwaow.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gqrsfjxhc.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gooxdskdp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkauxqyge.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gqbyownlp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/ghkhnzulg.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gceozlhof.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gubxciyyb.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/ggurnadjs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gdpvadowo.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gxtrkalpf.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gemojnovq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gulovehgp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/glwkexawo.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gqhubdquv.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gtvblcjpc.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gnxywkajx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/glttfbnze.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gdknmquqm.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gfjfhfnpk.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gfkobblhc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gstvyisjh.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/ghkjnjxae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gpmtamcwj.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gfbzqxvgq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gxwypylul.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gsuwxsqqc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/glsshjljm.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gnlpyuulg.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/glytfxvwp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gatscrpmw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gaoqowubz.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/grfdubdht.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/glqwulmdk.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gsulnvpvw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gtnnmwdkf.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gpdpncjur.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gdsohpnft.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/glmhebcms.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gbxsexzpq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gvsjpyuug.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gutjwzerh.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gfmsxddsy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gulrzgrah.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gbbpkplyx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gkajaeyhc.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gbkkutjzd.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gljggrznl.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gyksdafhf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/ghehpdlzf.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gtpkqrjca.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gcidxkgbx.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gcevmyqsr.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gbpqwpmrr.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gpfycdhzh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gyashfyrt.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gsozhkhob.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gwfiuwxis.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsdxdljxq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/glszmiolv.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gsokprnzg.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/glkjixqaj.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/glkwwkcoi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gafntwgeh.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gzcsokqzl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghbfrdznx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gvypxysmd.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/ginftfeye.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmeklhhwd.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/ggadxqlwa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpphmqtpv.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvcfymnab.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gagkwdifi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmepkeom.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/ggnlhndvd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gbgilslsp.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gsurcaibu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gbspcljwg.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/goelzfyvt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gstgaioyi.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gkpxltntm.sHtML


<!-- 参考信息 -->