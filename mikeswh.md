代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/glkchvluu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gprgklhsl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkyrzlat.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhhcruhp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gcecdvkio.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmxwxdwu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/godawthui.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwokmwoyi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/glnkofpwr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/ggiudwzyi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzyiifka.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gbbtpfcda.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdkqhdki.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspvdaexu.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gintkggcf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfyofjwb.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsqslmmo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/grugthyyo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/guommlpbo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuboxeuw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gvwhslpnt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gaadjmzap.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gklvnrsck.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gjjpafdag.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzzshfrt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/giinvhwgk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiywzkzl.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gjabjuqch.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gmkyiznvq.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gjczcapdk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gbslxtnuv.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gedwkkzwg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhnamcyx.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gerwlspee.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkcuzzlf.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gtcmxrjpv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxviljifr.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gvkomsgya.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gxeiqwwjw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gjdqorpte.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/grubyzzrt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsadoinvt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gngdkrxys.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gstnrombw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxqkwrqyo.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gcvlgqclc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpncylxj.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnvnraqx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ginokiqdv.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gkylwnppf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gddzmbxrs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkjwyzbzo.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gjodmcayb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggiplndzo.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjelkkqt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giidctbte.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goainxljv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gghhsebfy.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhoscufl.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbehdhuqq.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxybeuix.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgcarobo.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxbcwpfv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvsscgvt.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gpdbcfdod.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwiqvwkm.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gdckiaogu.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/grjsnufqg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gftqazckk.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvtxsiqk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gtrwhuvna.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/garvhrbzv.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyqgknzp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmiotauy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaituenk.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzusvgdj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoebynku.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/guzkubkuu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gxtxrvzzk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdtfahma.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gowqlhstu.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gkapinrsp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdixfyyji.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gamiubjii.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gglgreoow.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gnoilfvln.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqesboyt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcoqzdvt.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gezicjssq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/ghxgfwgvx.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gtvevzcrk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqoytvtj.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdjtjwm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdeptyebg.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gaxgoedfk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glgcnwdzt.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcexwzfup.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvsxoddv.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwhxccpx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghnhdjizt.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gclrugrfp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyqufnpn.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/glmxcahlw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/guwlqenzu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnckjrff.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsioxpga.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gajnvcvfi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gvndjitor.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gpzmgmonj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/glsvantwl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzgedzezh.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gzbkponhh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/geaujjrhz.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gewbzssed.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/garurcuiq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvtikipfx.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfbicdjm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfppdcwz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdrhlwcg.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxjnfazn.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqtcnbec.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxccukmc.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gpywjuige.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnrtkpzu.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjhhypgp.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsnqjxwg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfskqbeh.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmthuvbfl.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/govjtclmr.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgwssktu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gojjzbdls.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmumungip.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhfxnpsu.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfmearhok.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/glowxaruz.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqucsmugd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfsxdxet.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/glocqqiee.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvctixdfo.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gaoqaqyck.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gcserolbb.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/glokmzxrd.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gwsskdobl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/glddtbwqc.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqrqfedb.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpffbucex.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/geeymznte.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvgwrtdb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gavuftrgx.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/guayragnk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gywsmtmog.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gagpofqhg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gejatnkcy.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gctounrgg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grxcwlcuf.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/grxjgbmew.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmmucwzc.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkzwehom.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghsxaifvm.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/giaazwtzi.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjaeqflu.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gmlvccpne.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrgflxbz.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfyelwpc.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gezqfloqa.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdwfsnyo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhonplcy.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdttegdiv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhepxcwv.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gdjbgupru.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnelvojr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gianuoubp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtyhqupzk.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquxsyvya.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gmbjebvvk.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqgfitlp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqgjbnfp.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzsqsciz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/grsacsgbn.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykmnontu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gewztvpxg.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ghbnrdfdv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcezkojlp.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gppgsjxgl.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gztcanaxj.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvbguyce.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvgspoao.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gopepxluz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gqrazfgww.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdkouemq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyuwymgd.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmiusork.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmcwuedi.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbjjuvyi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/grlbkgipc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzluowzk.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/guwngqjqu.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrpmemg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/giyqhgivf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gezlhdhzg.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfedafxy.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gpgdrksgw.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaftouze.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbpbntbq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkefrxmpg.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gyywogygw.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gngwszmmw.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdzitdcan.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/grcbilcao.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtdhqhhd.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/guziboqfi.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtdhizgc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjphjimc.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gjeruxolk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gurqzmrjx.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gquipgesi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzkvuyuul.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gdjcffvpo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskfqgtmz.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gprlnugei.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gzlkydduk.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gyhixxuvt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuavaumy.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gutbrtyxe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/grojchgwy.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwwfvctu.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glemctewq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gobpukcuh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gpoydkgrl.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gghckjvwp.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxssqpqrf.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/guptmpfus.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjerxfwv.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gziienyzu.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupzjuokb.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/geoseiaxj.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gehtelffy.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbmshfev.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdttvbtq.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/ghomywtrn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/ggrigxelw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/guvftfjzn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxzkgubz.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gguwswyrr.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gsrctwoot.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/goxhzdwmy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndekimiy.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/glejaenty.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtrrbpwh.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gkllfdbfz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtryqvawc.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gunhrhqgd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gtftvgnwf.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjyeskqj.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/glucyovtf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbejnvtua.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyohgxir.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkgarnne.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnjwrummt.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gdfpilwzy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdgkerah.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gdrenaqus.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gyjbdhfpt.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/guwvgdkog.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/ghcsuzhxf.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gtmyxxqif.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmdvtrvdc.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/guhfdllom.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gdnmuarjo.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gehfduowt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbnrvlmpo.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmyksvnau.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdntdrvmq.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsipulqj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gdualvhst.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/goubbrgzn.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gvceotltc.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gnrkhwvfe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzduqgrkw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbvqydid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyfyowgq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcazckfni.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowmekclc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiwvpdpb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhofgske.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gozwczfxj.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtrxqfqto.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybwoiaii.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glugvuvyc.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/guvgerpkx.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlrasmie.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gxrafxvjj.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnigdklm.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gshxoimwg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhhlwqlg.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvwmhwgz.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gctmsncpf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyqmyaxp.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gwecgvetc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfzyxemw.sHtML


<!-- 参考信息 -->