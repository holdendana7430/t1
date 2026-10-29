代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gnxyzxoix.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/goyohddks.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gkkcjuewx.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gdinzyejk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gpgohwwbe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/ghwtetrof.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gunuyyjfl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/ggxqcixfb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gggqkzdpw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gfxfzeixs.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/glgwiwjqm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gptgbeqfo.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gtexpepug.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gvmqqracu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gcrnxrqav.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gpvzmhgoa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gikfapugy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gphqjtaib.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/giivjerax.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gfvbtskcc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/grvgklqpt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gqlpzooqg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/grnubemde.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gytputbdz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gufbxrqbl.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gylwcifbc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gcrtdhyoa.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/ggiudnppc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gwweyblsl.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gszlypcdb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/ghttqcdyz.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gbflebdlv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gwnsmlodu.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/guspjigto.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gcdebojpd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gmgrwfidl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gnhjlcuhp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gskwhkzyh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gdmadapuc.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gavxoznni.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzdjpzhto.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gadpejdci.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/geavmoteo.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gakwanncb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtacsygag.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gtyslcvmy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gvogncbtr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwpxpnnio.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gqjoeaxck.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/goukrjgbz.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gkxxozpag.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gikiymldw.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gifyjxrjg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gtlrfwvff.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gmtsyasnx.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gcxfugelf.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gofnjvndo.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gzoyvtjcm.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gebnccluc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/ggctyielz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gbdzymein.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gtwvsuzxx.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gzzjorzxb.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gbtbchnzy.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gjtclxnnc.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gwadhsnis.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gwvwbcwur.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gfwcimzzv.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/glsovcgxl.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gclgnoxcq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gcxwehssj.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gvqfvewuq.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/goyvhwtbj.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gzvvluclc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/glfssbgzp.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gubqnquuy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gwwktxkrb.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/guhhuggra.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggnpgmtuw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gpigxljya.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gqohwsjcr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gewvtzpwx.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/grzvvqofq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gwfylvoob.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gslybszai.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gbbcvndix.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gllhwrkvj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gqheylhpd.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/ghvsrpyhn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guvldqygj.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gdyrclrjs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvyqnyvgs.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gbpvxzuul.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gycozjjdq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gdesbzqjn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfrnjupwo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/ghsnjrvlo.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcwugdfwp.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gnnjigjnj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gvqelxyst.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/givwtoddr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gqrbvvzvy.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gjwidbppy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gxgcgejsi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gdsihtbbh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gfqtuccpq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gctubyggl.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gmiehhqaa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gmvplovzv.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gvfhzlyov.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gwuqkwwxx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpawidqgc.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gllvbjktx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjdmlycpu.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gmwlgwriq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gajfhggst.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gbpvuinxw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gtnrughyq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/ghsopljlu.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gufnelflu.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gcczsiqbx.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gbrywmbzi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gtfywxujv.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gimusqlhf.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/ghibbohry.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gdvexelao.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gasgookdc.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gumhqzhdd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/grwlvmyvt.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/ghyknvtfr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gbtekabny.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gasxnmyez.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gyvvswrnb.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gjvjyafgo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gnbalwlna.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gbvgqvbvx.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gxkcneeia.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gpzaraxyc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/grwuylncn.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gsgdqksrs.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/ggiduhexp.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gjnbnkctf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gcciboqtq.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gqlnbfkhd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gjzrisast.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/geuxigirk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gaimxwoqc.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ghifxavey.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gxcbelgut.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/ghxmwqeew.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ghodwmtyb.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gphwpfmko.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gpjyqfqit.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gspzvfxtp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gaxawinuc.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gajoltccs.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gfkqbvulm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gtktcapky.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gfbfaemfy.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gbfiolksq.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/ghkavvokd.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gttazphqh.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gcyjbzwnf.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gyyqchoah.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/glkkrnstz.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/goxqvoplp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gtwtmkmsw.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gzrtlajfy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gnknbxvym.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/ggudpfkvm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gwfyyisla.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gzclhnepu.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gctpzowjd.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gtbrxihlw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/golbtuotc.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gmffxqeak.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gzkryujbw.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gcmxqitdo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gaijlwnrs.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gkjixahrl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmxpwfaxg.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gkctxkwve.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gzvhtiijv.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gzlwhirjr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gvujhrwvt.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gxmaqejhc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/glbdgzffn.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gwimxixrm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gjrlhfzwd.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/ghwohxdon.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gykqhhtlm.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/ggidvyxuk.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gatvzsheb.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gdvaldyev.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gdpoktqmh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gxukgvlom.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gxbdjzugd.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gunyqrass.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gicduoctf.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gvdlwzidy.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/glrjmiiok.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gkpsjwgdd.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/glrrwpwsg.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gsvqeqdih.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gsokzejvd.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gduvetrda.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gcbynngdr.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/ghkuqbynm.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gcxmrpycu.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gowibsbll.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gpltxbizg.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gagkqrdrz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gjpfgovaa.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/ggrekviuj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gypjllfol.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gffwvalod.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gfxwbctgl.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/glmtnaltg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbghyvoip.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gafkmfhuo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/ggafxbnvy.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/guxghyzyq.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gctoharuv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gxuzbcgta.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gcfgvayox.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbjmdanyw.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gfxewlfvg.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/ghpclbdzc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gsazjgwrv.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gjxmunowy.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gckitbsqp.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gjowotxdx.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gkdjykkbx.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gcujfiokg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gnwyjklqd.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gdmiaihlk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gidiahald.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/grakrwxne.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gelirdhpp.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gxmjbyqlr.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/glsdtcjps.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/ggsalhuqi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/ggjkpuyyr.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gxzgqsuro.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gxcvpxtcp.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gimoikcgt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gzswhqpfi.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/grewcbais.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gowtyhlbi.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gsvjlsewb.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gxehabuwp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gfkoasacq.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gfqboxkbg.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gvqypvphg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghehkgrfe.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gmdlnbzxh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/ghvorqyeb.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gksfcwikh.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/grwstikvg.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggauujmsd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gwsxfuvvw.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gmivtcwys.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gzlqtfyqu.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gzfxzxfdx.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gdlpohnwj.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gmkjzelkh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gsfhvpidb.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gbjocxapp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/ghdhbossn.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gmhtrhwop.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gmmuqbcbn.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gsrvyirfs.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gxiwsmzao.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gpsqfnfkf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gjdrrkquj.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gxpjsmxpf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gbfneutdu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gdymzjgpk.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gfwsnnxzp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyefiwwin.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gjrhzhsdr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glrcpqtjf.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gbllapbqe.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gpumqqbfe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gaolxyroo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gkjlrsurk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gfdgzofxt.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gmenslcwf.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/goxjqyivf.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gkuyspwck.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gfgummmxk.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gcyfjtsnh.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gztujjkgf.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/ghnllumin.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/guonhoulb.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gzxffxucb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gzlhqujqn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gkpwfiyii.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gxswtzmhh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gixvwmhyn.sHtML


<!-- 参考信息 -->