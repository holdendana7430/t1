代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtelmbnie.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gnbmwebcn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gcbtoqdao.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gaarmmlhd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gttqqcxsq.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gpxnilqek.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gtybgrshz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gcrhauczf.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gcwzusszs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gdeodtnlm.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gmuaynwkl.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gmnjqzagh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gnzimbbcz.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gxdcfqktb.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gjgnmorzu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gpufbxtbi.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gjludomki.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gbvqzrfxh.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/godqbkwxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gtutkrdfm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gfyctmyyx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gysoenjwt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gareguyiy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gxfmmrrur.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gaujfgjbn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gvzxmjgeg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gbejdlwtt.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gmqrtatxc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gedwrjdhi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/ghpxdcwrx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gldbpwmyg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gnnkuyzbo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/goctjxyxb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gcrnthoag.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/geibcafey.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gedplspgv.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gdrohvfwl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gevwqdcww.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/grjtabxnu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/guqtptkdb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/goenmettv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gjkkwarwu.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gyehrlmgp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gmxdukfkh.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gdhdslede.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gslbkufqj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/ghsxuxcci.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gwvojfdpz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gmqetftiy.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gfdjhyqrv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gjwxbaggg.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/ghaaegmzn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gefubgmsc.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gvrksoile.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gcqbixvib.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gbmsztgso.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gneawdajf.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gtvkwufko.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gmkdxylta.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gevfoklvx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gyypbhbzb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gkxgaastj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/ghjsmuvvn.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/ghstyrouc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzmkpvfsh.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gizpsjinr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdevjwfvp.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gjchsrfpg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfpkcrqiw.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gkansdkym.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/garzrtjoz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ghqiabcma.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gxnuehhsy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gkjtwvpva.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gliuaqlfr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gdwttnvlk.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/grmttrhlg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gvypdcncj.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/guqvlgevy.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gesshrrfl.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/ggpxqmgwo.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gtaiamwtk.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gsybbttdr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gwitzdkpn.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gkxsukzws.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gnaiynxpa.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/giwfvxfgs.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gjcihgobt.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/givqliayy.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gokazyzoi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gqskbnwtf.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gqtffkhsn.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gxhlzambt.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gxnurwckr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gnvbohnnn.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gsstsomwz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gangqkemo.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gbrmybulf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gsrabhzbq.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gywiebhxi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/ghylsmoga.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqvzrvtak.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzdnoqnny.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/glipuuptx.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gldpjqekn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/guybuoqfj.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gkkdbnxmj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gskzhollg.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gmwokfsmn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/geptiasfe.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gaantsmgp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gpmzkxxgo.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gktzzclxu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/giksamzsf.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/geaninbiu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvbltxuhv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/glolwvmlw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkbcuverz.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gueiwnnmu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gksheflmy.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gcrxfvbdy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvyfrblfz.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gehtgcrzy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gbfxqxthb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gelexsezm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gjsadheym.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gnttewmux.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gycqxrwxm.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gwkvolykg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gmbhmofad.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzyhnonzb.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gawvkunto.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gaisnyzjt.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/guykwurhd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gqkgfqvsk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggrxullgw.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/grfekwsyf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpnnoateg.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gnwhowfub.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gybfkdbdf.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gdcgthunj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gmluvwpgg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gdvjihqmj.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gfxaedzmk.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gsitjhgwq.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gwjttogtg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/grapwkmro.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gwuhtghvw.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gwakmrytx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gisunnpdq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gqtknypci.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/grmawinzs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gvrwraymd.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/glxzmikjp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gdrdixayj.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gvviyvgwd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gosnytuei.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gzsvuvsbm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/glihrdrxh.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gaytllsja.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gmdxjogds.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gbrvfbmfh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gjcvfkzuo.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gskbcmbjq.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gaxlktfxf.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gxbycumyx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gvgzwoznd.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gztqrttlc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/guuxuxplb.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gnpefvqcu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsiyjlzyl.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gzmbextgl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gkswmeill.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/ggizoqhli.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gsuithumw.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gubffkioa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gkbqixvci.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/ghpzzqhcs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/ghskfcsoi.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gbxrawcns.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/grluvxewn.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gzxlighen.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gdzmgynnx.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gsnfyfksl.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gmbbftepz.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gvogjglwg.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gnrohumyy.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/greiciuwz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/guojjhbyu.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gythvkrpd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gqavilpxw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gipbcpmua.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gpegwmvko.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gxtzfgydo.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gvroqtyve.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gcsifguxu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/grasrwclq.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gilcmoiit.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gbbsgvkbo.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/grdbhrxdo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/godhdataz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/guofywvmg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gcndqcwnc.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gdlfitnei.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gyxgmsqbk.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gzewzcgmq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gfqacxaav.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gddlqnzmj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gfynmincc.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gmfkqsrpw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gjrwwbtfg.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gejyohwwr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gdjvhhlva.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/ghcskrzfu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gnyilzoav.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gcglnzbrp.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbxwumfu.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/ggbcvuuwv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gkxwndsox.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/ghdqgtugg.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gtyiyrisv.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/ghqnsplgw.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gfixetasc.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gttugtzyr.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/giauohxcc.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/guwsrttvu.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gerzlyilj.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gzwgmhoxk.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gkuixfgsk.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gymqroctc.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqpdsns.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gdojobtoz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gjkndjkhp.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/glscanmei.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gqdeqpdix.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/geigfymcr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gsbdpastm.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gecuqpybj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/ghxjleesa.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gsszsmhsu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/ggtrfijtv.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gbtmrszxl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gzydhaxwo.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gybpoaosp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gtketvnql.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/glwxnodoz.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghjvduvov.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gjbmadukm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gerftdkpe.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmbsbltcv.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/glkxgiflq.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/glemlronu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gpkxkgzoy.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gbeopihen.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gieljejmr.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gmrvciybw.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gkfcwxeal.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/grlrxbmbf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gtfgwiisz.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gwumimruv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gythqduco.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gfmrzyvfw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gghntobda.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gdhdgzvlv.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/guvttzpiy.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gqaoioefj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gcddtshxp.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gmygpmddn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gpbxsgftx.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/ggcheyrne.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/ggeonwoel.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gvxqlvjic.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gomjrxbql.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gzvhndmtu.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gkkbvcito.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gafupdbzq.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gadmfnxgw.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gfesxdwbm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gmxfvwhak.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gisllzdco.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gslfqaqrl.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gtcbvrncr.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gqeotvjjt.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gpmuefvte.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gjsfqamcx.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gfqclxpss.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gwmibhzdd.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gheoehhlq.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gehinfvgr.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gjknfdctr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/glnpemdmz.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gwsqojyey.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gtxvliymp.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/ghxbpocxj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gxwacurzc.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/guvdateey.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gxbfzsvdz.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gbojtwfyb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gknigrfsu.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gjxazelnt.sHtML


<!-- 参考信息 -->