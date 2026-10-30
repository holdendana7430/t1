代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhamneco.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuypbwaq.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrapadzp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaluxdxz.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylxgqxyc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/ghscftrwd.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjshwdqr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyolzlcr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gnhjxcstc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gyvvtkkeq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfssfpcx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/goznffkci.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmuhteno.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdlqwrxb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaptfmjp.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkditshg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gvydqitov.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/ghvofriug.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklghrlnu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjucornn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgmiyrjx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxczdpsqm.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtcfmfjq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gxkmfqjmw.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjviyzno.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gipbywkgu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gdttmxxmj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjadjncv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgxovjcv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gikyoxnbo.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gistbqsoc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdofdwne.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gudlcqaxl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gcljqvosw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/guqsvkfni.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwqwohsz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnqajzssx.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/ggfotqrkh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gedsztiep.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gfzjyovep.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtwhzctm.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcetcspba.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gomdpxcda.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gpgrkekxc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpqmlsfy.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjggmitsd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/glnljsdsd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjfmwaax.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gejuxplei.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaniehos.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gcbtdwcsw.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gtphibyac.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gehogesua.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gprqrttjz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzygcmfzt.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskdpwaeb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfayaukw.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxrgpsvy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/ghvkmyriw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gyycyatai.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvnsweeb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqxbygxk.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gpicuhlrp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxqbygqz.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbjoqnok.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhcwfggk.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcyeznsg.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gxeeduykd.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/ghtizrhzw.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gmccsnjtw.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gglnmdwui.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyxiznrq.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gunsgeyxy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrmsodxo.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gjeqkvmkn.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gyfumrliy.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjaigjwxg.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/guejwjumm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvezphutv.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrtcjfom.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gljtgrema.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gijoqosnc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfoovwat.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gaakdgonu.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuqxgmkg.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gqnhoagih.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfqsxyoo.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/geimfxiet.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/ghdsuzeyo.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhmfiurg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gywwckrtq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweysgkat.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbkqlnqd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/glgchaahj.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginsnnayx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gilossgod.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkolomqxg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gkejnrbyt.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaujoqco.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjvjrulm.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/glwlyavcw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/giydzfjen.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glqkzibjg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrnfwiqt.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gonfzhylo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuqgeglb.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfmgdeca.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghfisvakl.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnqdoand.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grolvxxbu.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gafdsdiyn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gczpqeccy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuhupjgw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gwzbfkhxy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/ggfflgxab.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvecdfzip.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/glmylagmx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gaziplbye.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxirbffia.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbecmbhxe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbvnsjxs.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gljkeasze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gyfbvnyse.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grsgeavsx.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gbthaedbj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnbcwxbu.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjorylzv.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gddbtvopx.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbyozxrq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkofnotb.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/grdigaqik.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjvdumrs.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gagnuiqjo.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpzgfalr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdolnisje.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gkiorfbvd.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghrdzwnkc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gaddirdwq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwbchqzw.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gggqzhwmy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gjabolujm.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gstloybdz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwnfingv.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcoqzmjwz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxkegamsv.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gdookvzga.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghiwlhubk.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuwrmtyn.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrrfbfwj.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gndpcdiod.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gdpkhmpbk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gvjrmmupv.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvykyyvir.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gexcedyis.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzofprncb.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfskrhdw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfugttwqh.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gpquonfxx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzqdfpewi.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqrockwg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gummdxajm.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdukqwcka.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfxzvtdwh.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gcwszgpcw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/geypddbxz.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/ghxcssbyp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxpimqye.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnhuwwnra.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gykvkxuhs.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/giwpmbxns.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwlwoxlq.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghzinyzfh.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrumoaaq.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfiznqnn.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghrtnmdwx.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnolcfndr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbrhahdm.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gnqlyfndx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gicrvlixc.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyborpgu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gikhubxue.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/goaaemhmg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gxjnjjvmj.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqtwtztc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcouirxeg.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gtgeyutyu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/ghvbusuba.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxzfqhpdr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqaahtmw.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjtpbesb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnmfhaoz.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdnxoblir.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gawxydivz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvcipxdb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkrnkmew.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grctmrjfk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gtjwjjyob.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gfonoaeiu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gtafxfxjh.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gmafuqhmb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeevnixb.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gkeodixzr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhaoqfbc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbucnlvl.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqpozrxw.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ghyltssdp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gceemfkuy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhblfott.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/goeqrnsnf.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqzggyms.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcprnkvn.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gptslatco.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjofzzgp.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/ggdrnhbdo.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goandqriy.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdoayibwh.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/geycfwwca.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmucteigh.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gxwgxoxsf.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpqfavzg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gifmzxyhf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrzdkgfd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gpjwdheql.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwoonfjn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcnrrmibe.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsygpluz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjwmnbpy.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gvkjllxvp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/glxojjbdv.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzglydhda.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvizqnmnr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzasqsznd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggegkhxcn.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjeyqmix.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfsmcgzf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhvpvzpo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/goclbquaj.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geufockzc.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgwknyyf.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gnocuztsj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdumuajlx.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gwxpglvtp.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuohrvdl.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykhhajmd.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizmwsupd.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbygkqaxa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzdhouvo.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gwrfygkgn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gqwhoiyep.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ggieujdav.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gknpswvfw.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gpnzciejr.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfkanlss.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcascoqt.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gojmxolek.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbivhhvuc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/grsliyjal.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/grdtivjwm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gdczaadyj.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gncmghvbi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcohhszp.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gxpdargqx.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhiiphpo.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiskolvm.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gesnfwfeq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqbubxje.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmlgjxmzn.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkxgjfel.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkprrlkpv.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsekqbjy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcgbjpxt.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gtbiwwkfu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/ghqgqgqzz.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtlwzryj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsihlswgn.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/ghzbwjedc.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/ghrxigqrm.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gyffzkpij.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gstfqgxzd.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfpxaxbjp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/glzawokpm.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjsnrghuu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gputrvwdh.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gaalxwqjl.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gqvojtgwk.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gnvevhmbc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggdtuwhnw.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gedtfzzeb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdizrjdil.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/grkfjejun.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/ghgmaxnsh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guezjcdvw.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrrhkdnl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaaxtpsoz.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwilugpsi.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgaxfevu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphdkblsv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezjscyez.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guawwzfhw.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdktxsmjp.sHtML


<!-- 参考信息 -->