代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfukbnqrr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpvbxbva.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghacpspxc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gkuqthqkh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gscntvwlx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/geepydzeu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyvjetdq.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdhipwhf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gltmstdxl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gtaousgsu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyugygujk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtjkbeym.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvnkpoeq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/grqfrlbqq.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gqidekrod.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gszivatsw.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmdsaabv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwqncqdi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdmnfzho.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/geypnjhzx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gkeobxdfp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/guznylvzs.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gascahrvn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gmewrfqer.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjptmicl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gbrnvjrtd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gqykyzxmb.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtgwcenh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gqyrratzp.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gdztgpjrn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwypgupm.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gkdktiman.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtliuufz.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gywhsjzbv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gixomyovp.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwcgruwc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gnmdsxyww.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbgcjesz.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gupzvkkqb.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gpsgovdmw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgbetihn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhnwhco.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/guquutnrl.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gssjapqja.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdfujkjd.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gkuprgguf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gshvvpqzf.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gsijnufup.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/godbfwxal.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gstvykyjq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgvaklji.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gssicyvyg.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhxfifmo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/guzypcfxy.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjvvvfgg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gfovmznva.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpoohffr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnxozomd.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvaqyoul.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaudtviyi.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcwygcae.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gqxxpfmnz.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ggogwglrt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyivodqlf.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxjeeuao.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaorwqebv.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gmmznbbqg.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gapgnbaww.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtuhacuv.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gpenjipzs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrmwzelm.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/guegwqvao.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkenyyejp.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcddczzcz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gabsyhxnf.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqzurzaa.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyisoopj.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhgdeeua.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gsgybghva.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/ghonteqhy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuqdxkhv.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/glasrpmbq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjuzmpcea.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyrzyejn.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxklydgq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhjegrnr.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gfufcemhd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/glxognnxf.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gbytntbhy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gjkdsxxkg.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gljlckglt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gvhnlbscq.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gijlqqfdu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gccfckztr.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwucouvow.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjycviwzg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkewcltpq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpezdevl.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/garjznupz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkoswaqo.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gnssbewck.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmnozlzpj.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaamsdbgp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gthbvihks.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gezmzvzto.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gbubifhft.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxthgvqpk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtdufzaz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/groyedtrv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gbpelmbtu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghhagcxay.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gwalxljed.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjupyhmrn.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gnwmybdns.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gufqcxvsi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxxqhdth.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gtesjbrow.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdltenygu.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gbktegzmk.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gkmggyuzm.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpvlnjle.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjitpkhs.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgrvnrrd.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giafzsuzh.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gsnfwzqme.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/goqblqkyt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gsrxeftuk.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwkeyqnu.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfmrqftr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxqmruzy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwqlvdwp.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gowcxxtgd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhvuwdkr.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghghiwmrn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebcxipnv.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqurujxzm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxysicamy.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/goemjuibm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/glxejfarv.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/grnqkvnih.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwzsnovc.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxckpgudb.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glximnbau.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaaioxtr.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakrvzwwf.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxzkduqc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdojbibvp.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvnowzid.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfruicebs.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gidaseczt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvchofgi.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gerwnzohd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrfafjkx.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaxyhixr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfxehvdvm.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gbjblrrqm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gurrtegkj.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gmynljmtq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxshqqcvy.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gelgoklpi.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvriqdpib.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/glepxckmn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsazflugl.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuhammgo.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjycqnsjb.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gzjlmuuwu.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/goggliabo.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrkrnmuu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjlzseti.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiidxnov.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfxtytbj.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtedbbnd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gldkwqvah.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/grxabwzgb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gvklixooa.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gwsxieyfk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gkaprtvjq.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gebkznlib.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrhjlvhu.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gckvaadxw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gpzwrzhql.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/grmawfszj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpomoiav.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gklpbtqds.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxqvlaxfl.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gtfsmtpfw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gewjahzwa.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gjagpkwyf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gnacznnrd.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekkxgrsa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkrioxbt.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoalvuqt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gxnahbhrj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gawsuohxh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gjogjqwiv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvrpzucb.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/glixauhuk.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gzirsieru.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gtocftmip.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gybrbofep.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gcexnfjxd.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/goozwfzxm.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfdnqdszc.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlrtifnp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gcurqarlr.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gkznkoycn.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuvqihpn.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtcntpspm.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gazmppumt.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghakbsxcy.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gfusuqghj.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjbafxbvt.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpjtetwt.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppovyesr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gjnhwwgqy.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/guvpyzayd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpximisva.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gbccuyeqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwdqnujt.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhwpbjym.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gxmydfurn.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhlusbtz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhrhynbr.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsmbhimd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgtnolsn.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gwogkeonf.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcnkhewhs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gzellhfyy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gwxuojfnd.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvppgtisj.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsadqsaye.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/ghnkmlrbe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gaesbuigw.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gzmhamzjy.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gelnkocsy.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gakdujyni.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/ggrvufusw.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiwhtkiz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gnbsibwiy.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/giirmlbpg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gjyeyqwui.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjrioewc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gveqidkiy.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxixglzgy.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/ghrhukrbs.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzasibcpj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gvzgvrtci.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkeskipe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesptzole.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbjogooa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgplgupe.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/grxqugnte.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbejianlx.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbjjjzib.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjfcopkwo.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcoitzfx.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gubgnwamh.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpmlmdsz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giuzyfucf.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gyblncins.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gzidwtqwy.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gdskvjbqt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoehwijg.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gbrdoydso.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gtminyleh.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbtnnrmp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbngwrvzk.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpmmvxetb.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcpfdkfs.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/grjuqnspa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwidqgkij.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyabnbft.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gepdldwsz.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtcjbaanq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gswohfsje.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gcgefaxho.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahfevjkd.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuulqfpn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxevbwml.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gshonqski.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqkhlina.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gxxvpsylr.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilvvtrsp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyrnvhayb.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeqttyzg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gylrnejmr.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsvzaync.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybhqsiff.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggbbsdxgm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/ggzelmdut.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/ghylzjjig.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gxyqflvnw.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqpruvkr.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiglzghr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gwshdyhvy.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxccontky.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtmkmgxk.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ginybzyxp.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gzflyfeaf.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gljsilrjj.sHtML


<!-- 参考信息 -->