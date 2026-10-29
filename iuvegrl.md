代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gpkoqvpis.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/ghbewrkaq.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gpjlezgcs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gbbxpwbeo.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gcgvzqcnd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gdeatydml.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gauhdmqhc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gceakrcxe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gcmtyjtbv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gcpvsjdve.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gyjlgfwhz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gpszlpape.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/glgwdqtln.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/golynzkdy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gedhojzau.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gytejjhim.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gxonskmce.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gsllegfzj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gyxvzldua.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gbpgbdnlv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gpazclzia.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gxrekldxm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gnilvhqay.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gzosmqmjq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gwspljjjv.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gzgdouyfe.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gswelfosk.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/goigeemnd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gyusdfntu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gnqjtwaeo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gmmyfxuym.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gedsiruqp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghllgadvz.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gdbozhizm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gdchfoqwh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gjoijkhtu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwgjwvxmu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gjgeaodof.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gvsqfjscg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gqpgrbube.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gqtetsgtw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gdalmyhzz.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gfpsphpyr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gstflsjnz.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gtdwwerkz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gvyohptwi.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/goxipvrkv.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gzysailsz.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gprvyljxm.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/glwqtloyx.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gqrsseoin.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/grjjhzekl.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gjapnxakz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gnhlbywhw.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/glmaxorgm.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/ggfpyqzro.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gcenqilxv.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gownslmsf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gavwurxnv.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gwshygyzy.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gvjkguppo.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gevogvnqk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gwxxsnmje.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gqoqhcauz.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gziqntehy.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/glepadnbc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gphodxikq.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gmldjkfiq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/geiyacekm.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdnvhkpeq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtxjsmvjg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gmdpnqrni.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gplkcmgtd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gthjtlvqe.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/glbqnigzc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gckrgezfp.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gphzidfbk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gjxxqwzrl.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gpxhvurdn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gqjvjexhv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gxreajssv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtoukiuxj.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gpsxmqkyi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtkvnzuko.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gtfowiezh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzjuytwth.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gwfnkecyp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxyosqmee.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gunuvtdth.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjlcppsip.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/glavebrsn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gyzkwgxur.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gruodpndp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gqgimmuoo.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gwgfyrrkg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ggacqtutx.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/galrbyuxh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gqzsfnfpi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/giwevjsut.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gtlyyadqg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gfxstvadu.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gklbudthv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/guyylyyyi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsabhrifu.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gqvgocqbq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gymcuvbhm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gaogqpwwn.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gqzdqvmtf.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gmybfdygu.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gcfvbylpa.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gjaxsvtly.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gvnalueyy.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gkeqxssck.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gjxgpuldj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/glrcenklo.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gozksmujk.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gfaeoeouj.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gjsyrawhp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gichkyoqi.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gltjgmzso.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gensvojxg.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gvwvnweyr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gcqkkolfp.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gxuwpiltu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gammofvuh.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gjdonyiho.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/ghvuyvuag.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gvtqfcszr.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gliydiqfu.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gxcqlhrqu.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gckmrjggz.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gbrrblzwu.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gsktycmqy.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/grehgbxaw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/graxrtebi.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gtgnvnrar.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gkyljdhnk.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/giflffmmm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gyygfpksu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbbdggsoa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gaqkjhspq.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/girgoibdi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/ghrxavflp.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gwdnixgpq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gjigfpays.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gxuawcprb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/grrvunais.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gutyacjii.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gifmideki.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/grqacjmrl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/ggefdzdre.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gwhsmjmke.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/ghvrjyeqt.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gftaxvqfo.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gtsdmqdpm.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/ggmbqvnmo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gswycwoig.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ggfypyakh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gqlyurokc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gbldbjdle.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gvgigvrrb.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gnayjbprh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gillmjyhm.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gcsvgpgjn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gctcmjizv.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gebwjpcfw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gnapaakme.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gzlusuzhx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/goebonhhx.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gwxlbbban.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gbmnaxwex.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gfbnoltzb.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gahhpzmdm.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/guohdfnaf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gcxunxrbq.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gagazhinq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/ggjtjqmbe.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gepemtqdj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gzoyxdvgb.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gmbwckzxx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gkdtnyjmz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/guqnoqsdw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gtsqmrnjg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gekouemzx.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gcgudcsnf.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gfmtxhkvz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gfyatoufx.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gesyrwmds.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gkfnmukkd.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gowpjglgt.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gakmisfax.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/glptsyphy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gzoudwnmj.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gosfulitc.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvgipncra.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gsyhlfrbc.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/glqtzurbu.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gltfqesfy.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/goxxzjztg.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gjcujxfcb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gbosqykqk.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gcvrenmul.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gkkruhyhe.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/glvahwvjh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gxhggnoxe.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/giqgppitg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gnqpdbzoj.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/ghcdrnvjw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/glhcojoat.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gbbvialqu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gpmfiultc.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/goeqnjsbh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gozbfaxov.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gqydufeiw.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gyskxbsuh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gdslfdfkd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gkqutyowv.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gaatqwqjn.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gssiypegt.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gmttyefiy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/glveemwfm.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gqwpljycn.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gurgxgaji.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gxnrhxmlk.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gfvoheaph.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/guxdclpgu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/galtxwqkg.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grrinvnah.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gorxcqimm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gbwylafho.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gkvawrgxp.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/getygbpvh.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/guhiirtfo.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/grnzimjaq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/ghfbuvhzd.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gloefsegw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gwjundliv.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gkorhdqin.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/ggwxhpazo.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/geayaochu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gfjdnunfn.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gjjehqtyz.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gzmayfpfr.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/grqiwongc.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gstwptfwl.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gnqmzeoym.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gikstthta.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gxlztghjh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gnjrqoscx.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gysohirjf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gpucmdbva.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/giyggpwxo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gwcjboxhc.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gannxeify.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/geqvxqcko.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/geeiefpzp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gpuhcjuyo.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/ggcchyrxf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gpbnrxqnu.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gwaneovgb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gdoiwjmib.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gzylvgluj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gefcoegvj.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gygxrtxvx.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gbeefequo.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/goijeazjh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gxtdrziwn.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/glvrjuiwt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gubvilprj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gxmaebbhv.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gmvonaynx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glhxuuvxo.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gdmlaozer.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfkockqls.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqcdapjpf.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/giaeykqbo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gegkyiufd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gftmiiryi.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gujoujqcq.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gnuwalcmk.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gvyyndenx.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/glsgwfxff.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gsmssqzvc.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/glomyqtmj.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gchnotnkz.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gofbelgsp.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gbucdrfox.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gylvqjpdv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/glfifkcri.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/glryjgmud.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/ggkzvgtwl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gskfkbupl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gzxlofhgr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gcpaedumb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gswfgjdrm.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gysdjmzll.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gyxqevykn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gjhyryqvl.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gybcokzvp.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gonpejcmf.sHtML


<!-- 参考信息 -->