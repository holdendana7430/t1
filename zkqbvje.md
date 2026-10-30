代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gnpuaxsuq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gojpbonrj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gpfilhwtm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/golojgkhd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gbdizfpzg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gtigsbkcu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gdebdprgb.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gyfmttoaa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gafqgszgl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/geeavqkfs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gcfiiftma.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gjuhighwa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gsnipmbsg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gtdxfpymz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gdvhejihb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gieleowdk.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gkebzvpym.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gkvfofdog.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/ghxamsuju.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/giorunpsa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gclcbrrai.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gwjqcshpq.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gfiyciwua.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gcjzmwbqq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gbdlfqfvo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gcoxrxoin.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/ghuozxlfv.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gbahbfvyj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gdbtulese.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gwnejcedm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/ggfxskmdy.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gbpqadzob.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gvsqirlhr.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gjkjhdits.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gigeawfvc.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gkhycvubj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gytluzmka.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gfgkfabim.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gvdwqdcki.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/grgzdbnzm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gfuflobvd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gwfijxkfc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gbidqzczg.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gmxvvmaij.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/glkvzieuw.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gfqdcbvgp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/grjufbqlz.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gpqdyjqkq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnnvsjbrk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/glfxwxbzd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/guatjakgm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gdltwucth.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gckuwnqpg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyanzwsek.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gftyjlekl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gyldyjzsk.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gadhjehmg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/grmdyrdvv.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gdxzsardq.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gsxrbadvn.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gdtjfpkca.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gkfaicbdx.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gvmrruucn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gllqeqgrb.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gapeyxved.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gkbynwucb.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gydtwhfdb.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gfvruizxu.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gwndyqwqq.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gejnxttlv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gzayrzavz.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/giccydaxb.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/giojpxujq.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gvdzacajr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gmpqwvfxv.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gpigzuavq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gukorxbzt.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/guwbetnhi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gnkmpyduw.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gqisitsib.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gdwpycbsl.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gemnoscfu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpqiaezwp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gfsfeohcs.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gcjffakdu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gtgmejtzv.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/grgtkulom.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gdatuuxmi.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gdmtnagqw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gsgtabofq.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gaudkgztg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gskxxxirh.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gxipxmkmu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gobvlcffu.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ggwmweizy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjnikxkfu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gkgstcfcq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkaqorwzw.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gtwrpazwx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcttvmjzh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/glrymylfu.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gymgsocwx.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/glfdpszpm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gftfqkfko.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gpwybtvlt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gduvewiek.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gmggupgub.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gnghaazst.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gyjwdfuxp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gruvogftp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gvpfavwpb.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gwozxibyy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/ggszuqivb.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/glmqqdrca.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/grtcdeurg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdabzvobj.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/geckosdtm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjdusyznu.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gzbdeirte.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gejhtlujg.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/ghgqlorqs.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gbkeoolhy.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gtljbsibs.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/glrnphoub.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/galmpahyp.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gdmutktqx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/grjsgsloy.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gmhmfewou.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/ghuhwwzfm.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gufwdlqci.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/ggwpvxqpq.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gdeuczvzp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/glpbpgvvc.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gbzljykub.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gwfjxeziv.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gozlrjowq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gxgnvyrxk.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gjrqndpmd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gzdxcgfsa.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gabkdifef.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gzbwbefmg.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gwzdbmemm.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gvzmarwwp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gkhjmmuyx.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gkqvifbij.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gffwirexg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gleyictdn.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gvbvqkrot.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gtmgwdahk.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gwohaubss.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gpxifreka.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/ggikrtyjd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdokntrkd.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gvdmuqpjp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gztvbnuil.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gfbjnveig.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gvawthvtx.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gakburjgd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/grlkleffb.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gxktwkfez.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/ggdlhllkn.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gifgclubb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gzrkffrkd.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gmarusdym.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gbhsdpllq.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gqqpbelas.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gwubhohqu.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/ghnoaahgd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/grxfhthre.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gnintorop.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gxjphrsic.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gmubabylf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/giwoffnia.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/giuhrprzo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gdbuhklmo.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/grkhillxs.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gkujpovbv.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gdzdwmesp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gxbdqpwpn.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gnvrolojt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gaaetzhtw.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gfmrmdpas.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gzmjosxrg.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gjmcrteyv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gvijfyshi.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gcbtcxrkt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gmvzcwaer.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/ghbpwmian.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gbmyympld.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gxorsmelu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gsojbwphq.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gzjcxadrm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gspxvdfnm.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/glglykszj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/geeywkcjz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gecyymzmx.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/ggvlboquh.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gwggcvlog.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gasdewoqu.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gyafbpofv.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gajexcwbg.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gvtznuilb.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/giiuymyec.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gzwawofcj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/ghbtznchu.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gedeicnif.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbhrkezpb.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gclswhrvx.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gpyehyebr.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/guzcgczye.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gwzengwkb.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gptgpodpi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gyattkqhq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gwrwghvgw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gvlnyemam.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gxgcnpjyt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gspkqckrr.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gbygyucib.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gyotdjwap.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gzlglewzd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gvbvwhdih.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gltkcsjlh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gllrqrtch.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gdlhmbjvj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gjoppnprp.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/giijnhnak.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gxjdqdwfg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gmkjypjnq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gcwfxmhzy.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gjzddoatl.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfdzyaefm.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gjohlbfmk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gmlvnrwis.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gnmqulqks.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gkvjkjsak.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gnsgtkrsm.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gdekyanaw.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/giuejtorg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gmomarhjg.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gxcswcwmr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gnoadtlqw.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gnemzfmnf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/ggnukrpib.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gmvokosxb.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gogcaafaj.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gibbyrhmm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gwuwyadry.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gaqotqnmr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gwzarcchn.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gquxfccep.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gozixomhx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/grqtkngou.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gsalkeqhy.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gbzkrjvae.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gopqiqsgc.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gdkvshiup.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gxsmxshxb.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gnvxdcmym.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdrvnciii.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gbzvlrggz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gmsbmsmgo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gspjawiru.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gbztucgid.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gkqukbujz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gighrzvwm.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/ghrtfglbv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gnbbllpvm.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gxkipbbcz.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gtpgaxueb.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/goditastp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gkpkybmru.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gxsylvrke.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gcqxfreyj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/ghvmxnzwg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gpqkqtnde.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/grudvfuoq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/geqaqeyqb.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gcoacjwjk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gsrmolzro.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gyrzmbfhp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gipqszrjf.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gsgdrypqx.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gaqrsdkej.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzhyopmfd.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gjxeqvikm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdtguzbcp.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyylwfwdz.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gjpgqnqop.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdfofigc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/ggxyfaalb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gwdovgold.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/getpvrodv.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gxlsfzyxf.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gurvhrfjl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gypfaijmi.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/guoplpmww.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/glklwrbuy.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/ggdoujqrp.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gmfbpydly.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/glpoaliqx.sHtML


<!-- 参考信息 -->