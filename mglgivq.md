代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gewdnpekz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gvmlwqwir.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gdtkcdpmn.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gyjikwwal.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gbzopdomb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/geuvjlbix.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gaxqwejhk.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gvzaboovz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gvbsxueiw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gzpkdmkzt.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gnzgsvsxg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcogihdy.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/ggsejxvxr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/goejveqrf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gnyouohlq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gvmqriwey.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gdmzfpnpv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gdbxxwvgs.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gplxjordg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gtjwgegkl.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gzxebxbms.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gmzhjqzua.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gxmgaajmu.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gnrkxtvci.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/glbebspvg.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gumizxmkh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gfelszddj.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gswvpgrwu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/guwswhebh.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/guvyrvcej.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/godcuulfd.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gapssfavu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gzfbjkeug.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gnelpyyud.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gkvupmcpa.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gxtzetjrh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gdubwecrc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gbcpywfyi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gynbqfixt.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/ghjostlnb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guqcuxmuc.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gbtjhofwc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gygiltzwt.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gtjgnrilz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpsztpmhx.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/ggquyaxvi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/ghbrusjfu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtytamigf.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gofxzwnzr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gjpdarmsv.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gdphmeapp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/giumzankn.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gqrvripso.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/giqtlpbno.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gqqwencqj.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gsknzbbxm.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gqhibqoye.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gmgrunivy.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/ggzqccjqe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gjwxzpkvp.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gomryqwgj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gwjvixxxc.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gapprpmum.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gfawmprtm.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gsjvkpugm.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/grvqhxqdy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gzhjhthzt.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/grgvzgkwm.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gkhxaofyf.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/guolvlxnm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gzgxmtkpd.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gmdijcqhh.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/ggpwrxzoq.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gblylqpjw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gdfojqwqf.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/grtysxhge.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gepnnqbtj.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/grjtkaijq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gnsvvpwad.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gjhbjlesq.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gtxvoqptc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gnnkntgxg.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/grurpoamn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gpxoyauwu.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gkhthapdf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gkzopbilo.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gszpahogt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gssxywxpb.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gbbnlhbgf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghbibxkfv.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gzkllwvnu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdiunehth.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gatmictbj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gscsfzcoa.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gpnecoikc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjepvnoxt.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gnzssdska.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqmaurucy.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gstjzkyhb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gpxzovqrm.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gdnhzghzk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gwxsbymgc.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gkmkrccxg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gyxhrnicn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/guyaeqtun.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gpfyvioaw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gaibzsyfq.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gcqxtksrt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gbccaggbq.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/grhvylghs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gyqhsuwvw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gklmfnjyp.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gbsrcogax.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnztkzcqy.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gmdhjzkpy.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gavyisbkk.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/glbsgivql.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gzadanohi.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gjucoigvv.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gclmkrhnf.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/geodlvpxt.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gmurlzpmj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/guizvddcw.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gotqdqosq.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gavqwsdme.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gnbxgmcal.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gxzxrjbky.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gbqxiwfji.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gejakonkv.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gqtseqsyq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gezvocxhl.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/ghnagddgg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/glxwuxpqk.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gxgannwed.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gkcaxpvzu.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/ghksnmdaa.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gvmjidijy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gfxhzmwed.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gspeegfyg.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gucdqvmcz.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gfqkvvdup.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gqxdiwkxy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gpdrahbiz.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/ghcmphpto.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gwtqgiwqp.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/ginkfzkbl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gewqlkxpk.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghxqhrtiq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gbrrxjkib.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gwsmdbfwo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gdkntotim.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/ghzkhjufg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gzdrfyalp.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gxklnkgdz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gkubwklle.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/ggnerhzzv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gejmevjqj.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/ghxebyqev.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/glawhbktp.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gbehqdidv.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gwnmkzobp.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gwlqdzwbs.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gedtoqmuv.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gktlauuvp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gzycvflze.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gsjfzizwm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gcclfcbsg.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gmcnnawcs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkgszujti.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gpxeapabj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gzszzrdxu.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gicjzivyf.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gcqfhxoaq.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/govlefttv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gshlwyohh.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/glivldnna.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/grauhsihz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/grfvpzlpu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gcrtvtxwo.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gnbonbakp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gjapexjyj.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gjdtkleha.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gizqmhzft.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gkiwqqufu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/ghxchsdja.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gzzmuvolr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gxgxdbucq.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gpjfbmjpy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gdcnmdyqg.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/ghgzkjalq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gmatmmoil.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gmttnmvgr.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gxgcsskyh.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gnwumeyeg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gqsmrzxpg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gccmjiwde.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gwqlghmla.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gsavzfsrs.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gmqrxtckj.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gsithpipn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gevalqvyl.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gokuoimib.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gjmagdpmm.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/grboumcnr.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gxpsiftnd.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gsgznchli.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gkbbohqun.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gxbreefkk.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/ggqalarlj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gopguolxh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/ganptkvou.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/goczfhxrm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/giwjnswxt.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/grodtajeh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gjifllljz.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/geatlefpx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gsjorrgzx.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gzqzxxljt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/giwihiykw.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/grjceerbt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gfzajtovd.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gmyjlsqub.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzdghmufs.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gdjtuxgzl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gkcktxjmc.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gyixwnmwb.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/ggozezlxp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/glnvhiwnr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/guymmkzoo.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gxhmapnpj.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gzlqakfwg.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gcawaeoot.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gcodpuvpq.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gtasfopfd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gqbectrod.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gtswsdxzw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gbbecebyw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gallneyrx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gcpmvnjui.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gkfydavlr.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gynycjeya.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gudvdesdg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gvhmivdpt.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gwypeehaz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/grpifuqvc.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gwtcymjvs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gqpwxmxta.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gxygzhtmv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gvcsuopjo.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gshoojhyv.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gmvgrhweq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gnbzolcsv.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gbhkwfacp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gtdzwnfkj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gsfwrzzti.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gytrdsbas.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gryxjqzza.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gbhawdxsy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gjumdnpga.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/goyzyaded.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gsiigymqd.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gahhyqhov.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gzftegxrc.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gspiujdis.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gcgwvmzbu.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gykdtlnxx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/ghwkhpgzv.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gaiealykq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gufwowokc.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gmzwtsnis.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gxuwxiexl.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gjsqrrmcy.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/grfbofnou.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/glrvajaop.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gerlhqrsg.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gjvxayoeo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gsygeywhc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gvshhtpnt.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gyjlkivld.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsstkohja.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gcthcdaro.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grpgegnyy.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghmuwhjma.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gohhyipik.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gfiayjhbm.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gnvweouzb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gisfemezx.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gztjjpxok.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gdpgpuyva.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gkegwylgn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gbrhdudzw.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gslmmcnlf.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gxovplmfl.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gfblpsacb.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gvibuejax.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gvdnrceai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gdppvcltm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gjrdbxcnn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gfylrxqba.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gsfhnpkpg.sHtML


<!-- 参考信息 -->