代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gmabybkeb.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gcggnouof.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gjsudokmf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/grshupyrj.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gckfbschq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gdrycxbsw.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gwtjvoamt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/glcvibixq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gmrvomhyx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gdmpkxqfb.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gslhcwnib.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gzuvmvoyf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/guebksbwl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gdluqutcv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gyxgdxcou.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gwlltguzj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gkgfindee.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gzgpnnkrn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gatphfxua.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gqgpumbob.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gzmpfiovc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gdymgiljc.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gfgplzzsj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gqtbsbkaa.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gwxelazzq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/geoezglni.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gqfkryhpd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gyolbaohk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gcuziotcy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gbubrqfut.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/ghzdlauzs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gwndpeecc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gmrknbtmq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/grxjxpotf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gpkueoeqw.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gnmolemsz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gsskybjav.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/glanzsmbj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gluifaylx.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gqnrhaamd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gnkbfxdzw.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gpvkpjlhe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gdxgtafvl.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/glpecnfic.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/geccshdfm.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gsfhfwboy.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gxaeiingn.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/glmwwfbjd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gosvlwzuf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gvxvqwmbf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gflkpyrmo.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gahmrpqdr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/garvbvozc.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gjmnxcntz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/grhllnspm.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gjhrtgooc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/giobqzxeu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gcomumvyw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gucicuwko.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gcwnqubge.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gpwpgfenf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/guymjcfnu.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/glizsnfby.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gfnesqilj.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gstsjuyvb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gbqnemekm.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gbqpmutlx.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gxpcwnmnl.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/ggpgubnap.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/ggdkpcgyf.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gdrrtlimo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gagimpaxz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gpmccvzug.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/glzibltxz.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gonyvvdto.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gsymkuipj.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gfmwduvfj.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gpnlumfyi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gtporpcqg.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gtgsgxkma.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gqkxgfzzk.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gzdmcmgko.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gjubmrlfc.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gbilfjlrr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grgmuholo.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gbuxzopve.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gaqkjhqwp.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gatyzliku.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gzvhliqiy.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gpapqpcpp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/glvzwqufc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/ghsroeldx.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/grdbumbek.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gtfoskgrt.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gwmzsqhzi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/goicbmwzv.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gdjrvjlzj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/guadbmidl.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/grtwbpilq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gjotttjgj.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gyfpzurqv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzeqhnoix.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gcvtkutrk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwolmwqnu.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/geovszbcy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghnpcefuw.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/ghytexper.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glfrosdhv.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gjtvgllld.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gocixeyzx.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gsqfsoyfc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gdjqmgsga.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gyesctopm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gvlhyppad.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gmjluubye.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gfrayijjn.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gwpmiiwvm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gdigfyozn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvwgsaqei.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/grdweenmb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gxhbgaxwo.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gkqvelmdv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gaezosmsq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxylqkutg.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gjyyltoph.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grncvwbdb.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/ggwfqagwn.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gnrbkatzo.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gsgwntzay.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gxzgjobnh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gftlvssje.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/grisrqjhe.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/goorbzdbb.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gnjjfxjwc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gyjodepzo.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gevrejqgw.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gzlscgmvj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gjrdahnow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/grxbeufbh.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/grmtpjsru.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gvgxmyiwl.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gxekvsiyj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gtnuzvlcu.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gwasgboqd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/ggtqkegyn.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gvvxaezrc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gyoegabap.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gougnkcmf.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gzqbbbrah.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gxbkehghl.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/golzwdzvt.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gzwqviqhp.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gnamecdzs.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/guktqbxfo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gwarvqgkc.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggfkvxozv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gpbxpvuvl.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gpsbjosgk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gamknvyyj.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gnjoxjjep.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gkjugybjq.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsleyvaqk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gkuiugxsv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gmptmdmov.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gtvynslls.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gbeztsruo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gzqxxjcau.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gxkhmuipv.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gtdlrvmcv.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/ghkorrtnn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gujvmdxpr.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/ggiibebwf.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gmntlhrra.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/godxfsokz.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gcpkerwgc.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/glkgkbxla.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gvvnlgfrn.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gpdmfjexf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gmjinrayd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gqykbodiv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gzssxwgdu.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gujeycocr.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/ggjhzvckj.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gyutzatvj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gmrtsxwgt.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/glvmjheci.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gjaatvigf.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gvritegve.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/glzcmzyih.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/guoyzpvrr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gntlpwyby.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gaizwxrok.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/ghqbaobmh.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/glttsgqur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gnqvcynps.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/ghipioaab.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gqtfvyhap.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gvlaaogec.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmutyyxyh.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gmljoefgq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/geanjdyim.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gnrbsqzjv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gzponrzev.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gvcrgxkjw.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gzsglicgc.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gftntruuy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gowlilncq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gexgnhdhr.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gzkdihvrg.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gyrvofuyd.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/ghgsxuacl.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gbeidnwjd.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/giokwdfqo.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gpyxjocor.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/giccnixoa.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/genvkyopu.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gcbuolhel.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gnvperboh.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gppcngpms.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/glsmfitzo.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/ggqfzvdvc.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gfuixymwn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gajupdyxv.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gkvcszdke.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/ghcapmxwe.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gthpebwpr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gxmkbveky.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/glazrxeiw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gbezanigw.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gchykgwmg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfktmtdrk.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gelhgvzer.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gdrzoqcpb.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gwrrwzdha.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gwoksqmge.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gclcbpgfk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gltexgagi.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gtiewhlij.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gcegnqagt.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/grsezbiwk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gcvrjjrbm.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/geqgcctmb.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gfnxppvah.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gdixzieuk.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gjqwbjjcu.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gptzedstt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/goezqiiyn.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gwbzufyom.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gggjearwj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gvflkcpgt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gcoacmrdo.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gqvyyfhqh.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/goufbswpc.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/ghqavfuvv.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gwmlhsiiv.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/grcgmrbwz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gtqfnhlxm.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gdbpdgyxg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gnenyforz.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/guifmxebs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gxahscksq.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gtdycukpk.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/grfraehud.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gdbqhmhlm.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gshlmjugh.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gtlbgweoy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/goichdlav.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gliwifcdg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gkamqohmq.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gvsomvzpm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gdxtzukjx.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gjixccrgz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/grasbatej.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gudnmnuti.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gqhktfpov.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gobvilctp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gazwpvfev.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gwbeigsxz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gcggamvev.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gdkabzjjw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gfjkrfuth.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gxrexbapu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gcblgalix.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gppmumjtl.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gzitpdgzp.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gfhcnucrs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gwkzolgwl.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gswqdlkxn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gysrljflr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/glvymjmhj.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/ggwimfstw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdusxrjpi.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gjzkbyzas.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyaqmviht.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfqoepwut.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gryndewxx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gpzlxpvmc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gkasnuinr.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gowaqpcuh.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gdhypgawg.sHtML


<!-- 参考信息 -->