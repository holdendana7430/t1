代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gthvcjyrx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjogpsjl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gptcyimgg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gwdofcmsa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gzsmgdacx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobdbthar.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gghkilger.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gscqpbztj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gnappvlcr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gannshcdh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gckctxzoi.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuutqruz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcimxbin.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfmiqabm.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gljyyzsgq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gprervcgl.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxmypllb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpsiltbs.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmoqsacx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gpaasarcp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyooawjg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhokswfw.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gphgioygr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gwlxubtxv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeikfoyj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gibtmvixl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkmoyrpe.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gcpaeidle.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmvlrqec.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gvveohwby.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/guevpakhr.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gpvwlpeuf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gsksztvbi.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrpurjoy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gavvrywvl.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gamjwbjem.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/goagbkmat.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gmkqzofdq.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpadwbvb.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gpahrnmsq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/govbpdbra.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxngtbedw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gsgvaspzs.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gsfogajqp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxfuhrcbb.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gaxjcqazo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdhytcnv.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfxbdwvd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnanpwrh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gackzzdtb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoxbifba.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbeaouir.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmhcfcda.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmoktgqw.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/glxzsisln.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gjkfgjttk.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrgawoym.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoebgckx.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/giceykmgi.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gdmpkwfym.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gvtnnwaom.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/glnzclzql.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/glzrovfga.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxysxxyip.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxtgpztm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbathetfb.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gzexzkdxi.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gunecuniu.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggdusybaz.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gnttzgsyf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gtctnqnyi.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gvweuahpw.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdwbuqpj.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gjklajynl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqirxyqc.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gbetfpdua.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgyhzodw.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gemkiqrrd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/guekxfsib.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gqicpurir.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gbdqwoqid.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gklysosxa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbdtuwxh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gfrvqirvq.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gcnzcwnav.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdmhmpiz.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/giuibvxvg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmhwqclh.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/grbygnrtz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gimtnnump.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gytecboio.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gpufucyhe.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrjbuqlp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpawfmgly.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggxsofcpv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmowefvrk.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/geutotxhn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfhsxmgo.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgkaikta.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyjqjoly.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/glldndkmu.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwlqiteht.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gbaffwwzp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdmcpbls.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gxmkfufqf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzidfgpm.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gporwtxhp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gfsueohkz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzclsxmuw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gnhontpbf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiytsbhp.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gafsaysqq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqqhfbbh.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmochqszi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimqhpbwl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghorqfzvf.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcilyvqz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glgauraef.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsujhdli.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/guyphpfdr.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gnakqhxpn.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gzovpfgub.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gocgftwgd.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgcjfvbh.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gcbtbinfd.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbuhwjjxv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gviqhloci.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gdqfxeynq.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glkggwovx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdiptvjf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtnbsijm.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyiwliyqk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqvgdtgyx.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqrllrsk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gykdvmrlt.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbamictnt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ganuejewc.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ggvwlmxsf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdiyotcpq.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/ggsizkari.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnalnjek.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxoxnyxo.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnscqsjr.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ginuldiwz.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuafhyqt.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsyjbzaf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/geybkdlje.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxtmalfe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gekvcwbru.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gfxmwwmdh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdziyfbag.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnhbizbr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glsjhjdjg.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gsltfengc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdfrwptza.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/geeypgyed.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbhudkaw.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gypopjumw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsvfzmiv.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfcombyr.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmparrlf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaorgvvl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzeglvzr.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gicdehnvc.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquisrakq.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuxsqatp.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gquszzygw.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gosfhpjwa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/glvoocxfy.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gspgbowzm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyxueactm.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/ghorjqxfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grqbcmnsl.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnzvmphx.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaadxllny.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gcxjemwtp.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/goenkmcox.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsjrssee.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvyrpsrg.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwfmmkogh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjlgafjt.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghceenmco.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gidczkspk.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/genaeyuar.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gstwpzjad.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gwegclrvh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjbpedjpq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgglopbr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gypcjqbqy.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gepphqsii.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gzwsdogvs.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gulmyeqio.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzijrdmzc.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/guwaobvtf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbaijmua.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjbsiadp.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gpvmyrhwc.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gqovnvfij.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxidnuz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpsmpwvn.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/giqpvnucn.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gccuoocso.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasvbemjc.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgokcfud.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjeqqewt.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcedtlgtu.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyxencvw.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwofpckvm.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gszgtsath.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcrxzaem.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gccbdumvp.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gzyvwvnyo.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgkrwcdx.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gprondzyo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsnzwjff.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/giwxmxlcs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/getozvceo.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemkwgrav.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvwrzjzup.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gfwzmrmfg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/grrmismuq.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnkpijsop.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdigzhex.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gpepehyqf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmsizyvj.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gmjagfdja.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulcmuruw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoyhplmk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gquwewihr.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoyhyopw.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjfzflmm.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwfghdva.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gonfgqslj.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gjyxmhqcp.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gugbceozr.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/glprsauba.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gfejqamhk.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkxsucbm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmruvtfj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaupclej.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/geihyvxzw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkdgimfn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/grpqseshj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfykkbgk.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcytlgdz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gytlkruvs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glokybxwc.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gangwadvc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbhudniy.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gqbwafyaw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpnyughu.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnemklvh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/glhvizqrd.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gryryuyrt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbmvbtsu.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gerhkwgjj.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gbrtvkffm.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gkhsqcjho.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdfflilw.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gosibnppf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/grnuvktwi.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gibmvbdbe.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosyawzsk.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggloxhmkx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvtagcix.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/grtbxwaja.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoigvmzd.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghmlmerur.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gdwaknvea.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyecfzcks.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfvznyba.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqgkilfn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/guouqzvbb.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnagkzcpm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwtnhrnpi.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gmzuvtrll.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gincyjatm.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobpiixrq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgkxhxii.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrpffgnf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklwxgmme.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtukspjf.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/geadafdbu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gapgfhygz.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gwluyjyoz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlulvump.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtddymcxs.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzntjrnrl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gutojyswb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gjzpsxied.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsyfeldp.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsdzaqck.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhzsvkc.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gtneoabzh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrhbtaiv.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gydtxqdkr.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/goyafyfzo.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkwjvwaa.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gknsbhdcj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtfepcbb.sHtML


<!-- 参考信息 -->