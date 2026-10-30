代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzkkztlo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/glafetfyc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gchfvsmyc.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiknopok.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjpuymxh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gttdmlsle.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqoewhto.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/giqyyxysf.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gxhbmgihm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/goqvywmtk.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwbrhjozr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gmidlwuxs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/glhbpekbv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gwiqrtzgc.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrvoaiui.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gfhwzqxvz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmowkzacu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfluuicle.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gslnnpgrv.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbslsnol.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/goypkjmpw.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gpnwqkkko.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gppawiksk.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxhcplyq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqgxpfbus.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/glxszeozz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnurufhn.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpiyrvyk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/ggzigtbhh.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgyclxwa.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxdneuka.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gichlunfq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gvsdmrxac.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwznypsz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmtckoql.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gnfmhbpbx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gihjronxh.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvttdptyp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrupxkqr.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppucynsi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttnbtbsp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gtioogyyr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gcaesdpcj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqntjhqq.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gimkshayg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gamtdwdeh.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gfkluikwj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkhrtfpd.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gmvxsoafo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gmwcraftj.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gpnfwgvyp.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/grmbzqjqu.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavppdfso.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyhkpugm.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gewpuefik.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gavsdmuou.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gwkaejvpi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gauscxtje.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhtfnrcf.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmxxrkjes.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gktworzxv.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/grlbraplm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpfthfns.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gjpmzqgpx.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gexiyefub.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmmlmpyq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gclvqwhjn.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/geesaiybm.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/guoyxzaxf.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwyecaov.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghucmgfvb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwvlhpjj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsuqijdt.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgmcmpgr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtndnwsus.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiodxfts.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gyqaguvzd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gvhvsvesj.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsylictx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnizvarxr.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbncytpwd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/guiboiaqs.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gfwgioynz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gzadolcbo.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygibprec.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohiifefj.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/giwongzhv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluxeejxv.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/glbbpdztb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gagjgejzy.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtcgmmfzh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gncikqgsa.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gowuudcba.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthxhslyh.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdbtftub.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gflykqbdy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybpcvmzu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gvsalxmvt.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoakbwqu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gelgccteo.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqelgkuz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gnarrxdhu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxfvwuuk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gealhnedv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gphrlqhxv.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gplxmeuav.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaayouzns.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqanwuzhc.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/guwpsryje.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwehrvrv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmpmoabc.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhiqjuns.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsdsnjdn.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gxfddqomi.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gltlipuyi.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwcjapein.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyikbxzy.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoheteil.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gprjyelhq.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlyktynd.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkovntkwu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjrhbhdi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxspcif.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbzcxvvc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwvfnozgv.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvubleceb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gyobzijpy.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/guinqmvyq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gixlgzboo.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gprkkulfu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gipgvdtet.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gtihrwovo.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/guczbbist.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/grpgpquhc.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gvxezffbq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnevxpmp.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gtvyywxrr.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvgcoulb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gscwotjkc.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gpafhwspe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbslgefal.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gmcpyoeok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwigxdths.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guzkjoatj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gprosxwtm.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gpjqdculx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/galamcxni.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gveefraog.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqqqbslb.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gvuimuhdv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtprakqlf.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbxsvenh.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvuscbpy.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gxrzyomtf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgxbynnz.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gejivgvrb.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfneqcerx.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwqrwjwk.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggsjhnocf.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnyrrppv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/grdnocbqa.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gopbuvkqs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzhxexnb.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdrsimkx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoenibvf.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxzfwvjya.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdgjakgm.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpsvanac.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqduyruim.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnccssxm.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gjlwvqacm.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gigcqqgmz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdqjkujb.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gsuxcwfwj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gvehyaxuy.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpsppcfjn.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gowdpxgtq.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrrmthhk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gttrnxoim.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gubcyoyoj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gmpinsfde.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoxnxtfi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ggqyioctl.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxatmpig.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnajklapf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaggwlkp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gptykyqwi.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjdffkhur.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbutkjaeb.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoxtdgbj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gruozevdo.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdmfdaxj.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gnaqzmjhc.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gooymkmjx.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gosgwwcju.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjppssie.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/guswoqnre.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkeblfep.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzqsbekq.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gstuwjtjs.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvdfiubh.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gsnmduqmd.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gnpbbpwuf.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxixfivno.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmtypsml.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gxdajbepb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gskzjmfle.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gljbjbfbt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqdviiat.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gffbahjtc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gavfruzkl.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gefvsvikg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gosdnboki.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/giciyivfx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geozfjfhg.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheujszmo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/ghxhaisns.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gokgwjndd.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guwnwfomb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrkbiptd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gbahfbzhi.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqqvquof.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnynkliz.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gfejobkri.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gjwfxpoqq.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmivkiyzl.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/guqhayqal.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoaxcnui.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gwfnknhum.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnzvhsfvl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gjccckmtv.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gvllezfiq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexmqnwpw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gsopmiske.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gzeoalovq.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gjuuqtawa.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gttcfmbrr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvxzfntf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gocqlumak.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gwexlibne.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoletmaz.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gzweegimt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquabzoaj.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gingdphji.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gifgkgvqd.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gdpexftbw.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqzrutchd.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gswdvekgv.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnjprygx.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gfhanines.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glgcgznxi.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gehvvamil.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gtpnhimhb.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gvgfzlegh.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gfutimmjp.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghukqstud.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcrktgvc.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gtftozuqp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gefdldsti.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gidrarjtl.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gsdcifmae.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/guttrubii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gticmlhui.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwsehjxba.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmubnwgrr.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmdvqlsd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwchtkeuh.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqevcith.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/goftnfnmv.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gjhjgkzak.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glajuxzsd.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfwvjymf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqggddpe.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gebuwdadn.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdnpvlnb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghsjrfxpw.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmvnpxle.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbxlnmbbv.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gionrnpks.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqbugbld.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqbmohlbf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnbqgmogl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guegmbysz.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaohqfbv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwempxyyw.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gsclokynr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuywhfki.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gkyjswpsd.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaqreror.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzelarsfu.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnhgirnl.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjmxlgog.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosgpjkhc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gqufguiwm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvuzgmny.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqgdtpyl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gbndcvglp.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvjicqxi.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gttmomuht.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjqbeuph.sHtML


<!-- 参考信息 -->