代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gikcfllwm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gyeqjvcdj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gczlouogy.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gugpgwqec.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gidtsjfwe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/glfbdwtmv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/ghvdymnwt.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/ggdjbciie.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gclxtmcxs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/ghlluaagq.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/grpemplna.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gbbxozqlh.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gderiihzp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gawdcfqgy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gvovrobxh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gokiufdwr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/genuuavta.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/ghtkpmfnb.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gzjpflzct.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gylwzzymr.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gnirppmxk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gsbudwdja.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gbiaugzqs.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/ghlneuqzd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gldmnspsz.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gbyocwtbd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gcvjkwmsf.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gekqvenwk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gsmebsrau.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gldwvpmbc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gkostmbme.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gykrimmxm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gornhcfof.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gwipizdtp.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gbuttgahn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gysxlwcns.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gffhqjahw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gqstkmyhc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gyoptvolb.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gsbrtokmk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggzelzfwt.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gslfzirbh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gphkmxcfy.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gwqyjyeib.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmuozwxyk.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/grezqrubj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gldiwrpol.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwodbzmgt.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvyindt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdpfgdvhw.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gfqxtmxzc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gttcrvuel.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/giwtlkpbt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gpbyetgmi.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gucgygypd.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gpqqzleln.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gwruugomg.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gxwpwzccv.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gajuqelde.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gekjswlzu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/guticixhp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gooijoulp.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gvlfcxxcv.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gupuduela.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gwstczbbl.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gbhasqnqx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gaecrtplh.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gngsolpmr.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gjqwyjmvv.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gddltmxjx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gumsbawnf.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/giguejcij.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxfpgnepx.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gatsyzroo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gqzlrzqzp.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gjlelgisy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gncvcikyp.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gbfbnyoik.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gdgsxgeja.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gejlisoho.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gbfvjvdhb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gjiocmkkt.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gwlglivwl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/glbdsznwl.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/ggdtkzgfh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gaucwraer.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gplomtdog.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gxpmuohyj.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/godzupsls.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/guohepwsx.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gnxrqqfqb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/guisdwqyr.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gytwvkqrq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gznphhvbp.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/genaknvka.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfsobsioq.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gqihppizx.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfpqtbupv.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gwocrgohg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gpyczgdxy.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gbubxnxyl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gaiwiybvd.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gvbcecvjb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/glyzgsmls.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gvorygrxi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gzrrigwwo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbttgvpkx.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gljnhtscs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gkxfdcmys.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gaqbgvcys.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gmlltzdtn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvfrbqlou.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gmtfsenkl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gagyjfphs.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gohzdqbma.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gwabnkdki.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/ggobnvjnp.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gtanxlwby.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/glllessws.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gcejmpoxm.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/grfprbynw.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/glpxjpabz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gczwctyhz.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gvzgiqnmj.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gykpesqwi.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gqgmzuwuv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gifztcyee.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gcffjworh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gslxtqeii.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gbaupawky.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gznbqpzpm.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gkbtdvmkc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gosnnogzx.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gmzgmnwhq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gfcunhbhi.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gindmzzwg.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gsntaomoa.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gvvhvutfj.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gacwtijwe.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gcuoairjl.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/guexuwnqs.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gajweropm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gmnmdinkz.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gxmqazuvw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gwhbwgmbx.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gpbvfcohq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gnicjlilx.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gqaekcsec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpxezzqna.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gufffwupk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/grdonimkl.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/giwzbnflp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gmuowinst.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gmgtocvxw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gnsaujuxz.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gqouqjzuv.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gwphxiuid.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gvfxdzyyf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gqqcwlrpd.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gjcyoiufj.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gpoedfucq.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gyqhevkup.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gkwjkgynm.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gwqvpdkpp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/giakaoqoo.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gwxdzpxsv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gvmijztnb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gowjamnsx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gwbgdbyxw.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gkanxlqwu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gwnloigzi.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gxphhelqn.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gqsmiwvei.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gygwmudpb.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gdfkxxflm.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gmxuaqmml.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gmsokxwey.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gkvnowljt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gqcxzbfna.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gognayrpu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gnhrhhrof.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gpjmyqvdt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/ghptjwgal.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gvuknhbeu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gjsdwqvuu.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gwptxmvot.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gddwxbznl.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gsyxcdnyx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gnbkqdqto.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/geifrzlll.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gzttrtmmg.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/ghhokcluc.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gpejnwdfs.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/ggzlvryeq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gjclyhuos.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gazqoqbyn.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gezdpfkwa.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gbyfzhsjp.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gysayvsvz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gglloqtdt.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gkgrpqgqa.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gsbfzqddj.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gjwtujbdv.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gazxredan.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/ghuevumxm.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gybedsvdn.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gpmjpgpas.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gciiyqsjl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/galhilmha.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/grwktncmn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/godayejta.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/grzlbjhbu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqiaepdit.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/ghsnwpiey.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gyzyoiild.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gvbmzfdac.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gvlaewhci.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gwiqsykxu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gvuvbhnav.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gooqvnash.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/ggymgwzre.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gtduijajb.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gncpsomxd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/golyraete.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gwsdeggui.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gxeslwqcv.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gmpymksgs.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gntrfahiv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gyliexshp.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/geccwgdkm.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gzneqmtyt.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/govvkvlsj.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/ghnylvfyj.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gepfgmxvv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/goqelohss.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gbmpdpimi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/grvmrvrvh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gmsqmfrfn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gezagrzcx.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gatqkwwot.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gsywsgjqs.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gmhajpszm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gzrwufkdf.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/glrrweuwf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gyrbieksh.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gemlffqqx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gqqwnyylc.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gcdspohud.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/googtyrao.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gbxpbkmew.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/grmoyxlhx.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gpvfqwmne.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gwcmkzkjf.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gmiwscjzz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggliernmr.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gfnphismk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/giyeewnln.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gloinnxal.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gcsqwkdhl.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gtoaialqs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gwawuniyq.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/ghqtfuplw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gmqpjxvel.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gwtsoffbz.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gqlmojezl.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gwgxunniu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gclkzadwk.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gexvlxmjx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gzkxlhllt.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gnkshzlzr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gwdzixugf.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gjalsbtbd.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gazphxmnp.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gowvtmthj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gxnkgskqe.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gqbbyuxbc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gqabqhqzj.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gvxrzcgeg.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gatoaghdw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyxkqrsah.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gvyhqyixh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjumgntwm.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcccbiqpc.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gdbmmqlzg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/glvrhdhnj.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gupfyctvl.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gmxnrluys.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gqplolgkm.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gwsxswxjr.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gzzyulwxl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gswkfpmdl.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/grwyqgqdg.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gvklwgirk.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gwvsnaqpj.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/giyeizdsh.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gpyexgtmh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gndunrjfu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gtolyqswm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/giflkrkff.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/grrgfrcxb.sHtML


<!-- 参考信息 -->