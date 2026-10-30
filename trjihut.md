代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gadzoljpm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gsompfisx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gublzdlrv.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gpdtptuwm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gdxweeqfg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/ggxiurpfq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gevxopjuk.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gamoqccvb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gpdfqxdzj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gcuhbqcvl.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gjnvgkirb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gctvdqhmf.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gxagyzhui.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gbzvdnlrv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gixwcxbfl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/grxtqyowh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gyutufqek.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gzzmnjjlb.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/glwraskml.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/goghwcbxs.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gihqbaojq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gvnjvyzwy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gejuqrfhe.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/geurpcvtd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gzbarbpgw.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gqezudaop.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gzzuxlfhg.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gwluyoasw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gamcsuoxh.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gujidjhub.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gbtpcmqfj.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gxftuacjo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gomwzsmps.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gsobnnbmu.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/grjljnkvs.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gcwjcjjcu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gmsuijqps.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gzrxadubt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gxpfxgxtb.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/geelyiqhn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmxurtekx.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/ggrhybnmn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwjssdhup.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gcqmadetu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/goasyehop.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gaaczijvl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gzxjwtowo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyoyepkfz.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/godzbmwjk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gylinqxgb.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gaqwwlape.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gnmbynwhs.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gasetuuxb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gtfutqylj.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gcsloluev.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gewrufrwo.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gayimxhgw.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gulfnjjnn.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gopfeqpln.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gxddysfeh.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gzazrbvje.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gkbzzojax.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/glipdhuaw.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gejroheux.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/godvwpkgr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gzwsqclhv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gtobqrrfs.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gxkhvxkun.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/ghoooudft.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gaiktukqy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gyiiqxdmv.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gwyytbtos.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gfevoejzv.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gwwypdlns.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gxtmqzqzh.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gxfahsoll.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gendaywwl.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gpfieguem.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gifcdmlab.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/geovwvrja.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/giyrqdusa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gnfzgtqow.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gltmwawlr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gucnfpegj.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gckbqbkyz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/ggwhgwhox.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/glbtoeahr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gmyuyznyf.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gmppanfll.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glvpbxxlo.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gflcmcqdz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/glmgrytzb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gnplwdels.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyamedapp.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gwhpgvoqw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwtgxwloy.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gzefhohfs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gggoksquh.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gjbjriuml.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gawdwabsz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gfpjbgelp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gbkcrnjhw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/grjbpcpsh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gwvfqwker.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gldmwusze.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gtfyyhwqu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gprxsqlcb.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gmkjoojzq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gxtfgxvin.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/ghcpgghfy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/grjkmdpcr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glzqvgaya.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gofgeyjtb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghpzbivqq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gqaqaljax.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gdhtibdbf.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gwiapuqxf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gwzdadmag.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gdibdgvwq.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gdrmvylyg.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gwjfxorip.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gaimihqxl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/ghobbppdh.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gvruxzbgw.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gacxtfeql.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gnxnpsnmv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gtzmyaqgp.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gfsoxhmvp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/ggenbhkto.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/guzadnsio.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzrinhlnu.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gtbzafmxd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gsafanlal.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/ghbrgxrdp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gdjdcdtog.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gdtooawbd.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gjiqbvfel.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gqbrskfwi.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gxhrmlrut.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gyckejysr.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gzuwafnjj.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gywgywfbt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gecupwhxk.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gknzqwpst.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gigqiosas.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/glnvaiuwh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gzsmyxwyy.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmoyjrmrd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gukpbqahj.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gvdqrsmyw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gfagpxfar.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/guhvtjvtj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gewruljpx.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gfasruzkx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gzykqjwuv.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gbnjboooc.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/grrxpvzhh.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gbenoupmd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/grlvfewek.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gbxliyrei.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gchhtnldc.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gyudjlngn.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gnfixucib.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/ghlnoupou.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/ggssqhoxg.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gjpgxhtsz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gxldydtur.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gfzcecbwl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gdnhpwzfw.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gqpknotaa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gtnajezod.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gtqphhxix.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gvtgenrej.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gvklcmxxv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gipgkiirf.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gwzmwixez.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gsqfzuqpq.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gstmtmpwj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gtrwsksvn.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gnwsaeeqf.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gxliwgjtr.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gikbgjnzo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gcwcygnbq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gvvjemhjs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/ghhokjqgs.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gqzhhsnbd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/guvhkydll.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gonmdirkn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gkfdwwyix.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gxmdwuafp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gmnpogrxo.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gjnaioael.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gpwvtdtjp.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/geakclbym.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gbyydteel.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gszlgyubr.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/ghcpkknyo.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gfxwraogd.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/giocadscm.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gguuooeaj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gsobhgceg.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gotdcjyay.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gykkpupou.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gipgekmml.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gmaljpljp.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gjdccyrec.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gbozyhxxz.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/grsnoikqq.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gzlikusqb.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/guayicejr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gmkfpwrwy.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gupfglrxg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gsrvidgdv.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gjzskxoge.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvgaxlpsw.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gexnwewcw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gpqrpgdjn.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gfbdgkedi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gybqzfnxx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gpzteohom.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gdmrrxbjq.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/glcmcrgyc.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gupdmujop.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gduksmpjd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/greyrbveh.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gnnyfxtmo.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gfubfujvl.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gzmsjkuah.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gbtplespg.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gjwvtqqkc.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gqrirvmcm.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gntgrhfvp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/grbbzcfno.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gexmoestf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gtvymdhkn.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/ggpfojiyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gjtyhfjht.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grfzvhmla.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gtcsfhsbn.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gyzcrklyh.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gyhafurjb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gjzmvxjhn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gwvevzrbu.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/goxuquwol.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gjrfqxcil.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gqgjpeddq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gfdvkcqks.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/glfhldgtc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/glsojteol.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gdbrmqleg.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gjczbjfzg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gbintizgx.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/glywuptrh.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gyawfqpwl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/grfxlrfzx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gmgazmcjd.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gwnlwpguj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gmwlalwmj.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/guwopviia.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gvodfxccu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gvbatdxwc.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gtgqwtvwk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gddunnpwa.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/ggeecnwjm.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gnlxklpsq.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gojadwmyf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gumxnjjto.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcdddaxeg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gvnotxvni.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gaehqchgm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gevklvded.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gkabhmjfi.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gtkwucqqe.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gwbhvdwsr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gjgmxthmw.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gxyipiuni.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gthayaecj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gjytxddwp.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gfasyeler.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmjeokalj.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/grmpnnufe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdaddkefl.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gsrvwxspe.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gjmnvptdw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gebtuyctv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gekhsdnvr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gifmlzxoy.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gnhmzjoyk.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gcimqceiw.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gldfyqezk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gypmykssv.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gfncripds.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gtxcicsaw.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gblvedtpu.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gbhlrrfqp.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gwkmtwchr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gdrqwhnpt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gpetiiplb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gixslbojz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gyowlfokb.sHtML


<!-- 参考信息 -->