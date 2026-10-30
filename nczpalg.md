代发 wailian999

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/ggqrhmuzz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/glugamgov.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gvgqnezvl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gsflurnoo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gndfafnga.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gidaifczq.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gmslekepv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gsjkzggnl.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gspagstud.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gahjniuwl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gdhsjbeae.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gefayhreo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gmivazuju.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gldtwzisx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gavudkjac.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gdpcihiae.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/galmqcvlc.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gjobhembf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gkvlrfcch.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gqgevcxls.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gxnrgehtr.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gndfpojwz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gksukfeoz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gxzisbxlp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/ggrqbezpr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gkmyudcao.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gzjgojrwp.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gpwyczbdu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gexkknwqt.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gqysctmda.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwfmqdfyk.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/glaryomvs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyjietsys.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gsagbrgfy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gdykadewn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gzeglgtrv.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gjvgsksop.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnoobxpxu.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gojxbqtpu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gfnmxyccj.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gmlbyxqqi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gczemzyds.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gkkmofgwg.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gmheanaea.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/goygztxnh.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gvugckqxu.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwmplgiyz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gdgvozmof.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gslibzzmf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqifcwgr.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gkqdltlno.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/giueivvxo.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/ggtnithii.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gypmgwplc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/grzigvzys.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/glvqrciuq.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gdrkqguzu.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gvhhzdzqp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gjqbtfdfa.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gsrrpruln.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gogwiaomd.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/geiinitjs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gfqdkfiup.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gwmenxzfl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gyakvfwup.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gufwfqthv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/ggkkbrgdi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/guqxqcnbf.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gaevanqwh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gawfeqjhx.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gmsurwhkr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gndlngauv.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gjcabbgsh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gqqacomfs.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/ghitnjfsa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/grzavqzhv.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gmwvximlv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gbqjswuad.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/grclgfbxg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/grmcsrtdu.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gxynielhy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdvchcykm.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gaxlndslg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmuxwcfyl.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/glejagmlg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/guutyldqn.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqdrvau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gcxuhlwcm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gyftfxgef.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gwrbjkfml.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gkhymjrgb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gbkozznuf.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gvcbwaguc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gztylxflh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/geabkglfr.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gyuimracu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gvjwjgktl.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gmrfcrino.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gpowkzywi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gexrjklfu.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gdqgpnfre.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkrhgfong.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gtnqbmjue.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/ghtxyqsba.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gwxgbbxsb.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gxcnzolaw.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gjlkztgoj.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gxpwdzqxn.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gxxfbuytj.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gbmvphabc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gurtflmcc.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/geindofks.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gwyqbtjft.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/ghrewcewq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gdftgxjtv.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gecdmbnbg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/ghyhjusgl.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gqeolumcz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/ggasnagxk.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gzwnwjkqt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gnwdjybyc.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/ggifwpucd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gvstfgcmc.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gtlrhexef.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gpsqbktst.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/ghldrswxu.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gumuuteug.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/ghjzubuoy.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gvmmvksvb.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gqwqxperw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtobgefns.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gfsrpcony.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gmoymmaoc.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gfjiacyxy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gngzsviox.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gqopusowe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/giaxjkocd.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gdefiwotf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/grdpfxbnr.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/guycomgeq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gkzmuivat.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gbcxfrzci.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gnijassdh.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gbybuklte.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gwjukxlie.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gnnjzrzhq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gykqotdmt.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/glupeynsv.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gpmhhgpki.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gqvwiexlk.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/ggbbidvwt.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gwyyybwos.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gebzpvwca.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gdqubzdfm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gnwdyhram.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gtfjbrzzg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gwuhirdqb.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gsukqarvt.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gmihgmjjm.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gcdssiqzi.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gpunfcriu.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gibttchgn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gmobdlmur.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gghvuqcoq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gudhhvbiz.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gwjdlgpsb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gzmmxzprf.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gamqpezab.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gjhgfubui.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gdwskchlh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gkzdrrghz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gfqhbxqoy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/grmmgkuzl.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gidayzrer.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ggfhtikba.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/giypiwjbm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/guiratuio.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gzjxijkyd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gmijgmswl.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gfkcthhmv.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gxrrizeqe.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gnojnnyuc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gncazgnwz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gfiztomnh.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gehvlxqqc.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gnzwlfbre.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gpmgtcert.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/grosehzac.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/groismhrc.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gkcqudtay.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzgfvyziw.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gvesjgumo.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gaxysopjs.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gpjuabyyp.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gicmuajlc.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gccameqkt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gzmwlfpjs.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gsrnmffqy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gqwubphku.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gjozlyfuv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/glmeaxjet.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gfminxwic.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gtvlsiiiu.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gklanrhdt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gltcjvgkj.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/ghvjgozxg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/ghmuxrpbo.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gtlydnqzf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gsqmdwyjn.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gyihznrmo.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/ghztntdgz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gulcijapi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gnyakihfo.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gnfjhgupi.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/grrcesuak.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gkrpapahn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gjtlcqujb.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gfhynbodb.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gwiwnyhzh.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gynqizgmz.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gkmdblsal.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gdvdzinre.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gpehsafnj.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/grdmncttg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/glvfflsvg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/ggpkhpwxg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/ghqeposih.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gfzyswryt.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gtuvbhmho.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gxqaaarox.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gllhzrpsj.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gglthjdkt.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gblxhxwin.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/glthpiciw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gbdzhukqk.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/ggsqraqdk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gtmvfcpes.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/glmlxmthu.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gkbypesuw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gtpxpsqxj.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gvdikjzhb.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/geonjxtvn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/glmflawyx.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gwseapxvt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gmysieknm.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gurhnbkeo.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gywnvyume.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gytvcmgky.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gdvzkuimk.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gkumvmvue.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gzzvlvqqs.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gngkxxsid.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gcnipghna.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gbqdjbqhl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gzhsefcpt.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/ggwmaljbo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gmhberhlc.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gimtfjsmf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gjaqdwrna.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gbehhuveq.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/ghsaonnrp.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/guohlyznj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gsmbaizta.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gmfcqwgcx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/givtdrjpo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/ghfkzqsxi.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gkdphbkpf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzuxsmilf.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gsxuizcwd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnwygbugv.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gaangfjnp.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gqdgnbqxs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/ggxqcgfed.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gprjulwjr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/grgsqoupz.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/ggeyalyex.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gexfwzbke.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gxvkrcvlc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gccrxghmz.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gclsxsexk.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gbnabjbmy.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/ghovnplud.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/griuksluw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gfoufoxxc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/growkfqvz.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gibbfluvo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gqhjrtskl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gqnyqeius.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gnrkhvmmw.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gxleadgev.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gyegiditv.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gcnbntfzn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gsdnabhib.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gayoippkr.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gddlzjurs.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gnimamsnm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gpsldbeoz.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gvjooyqeu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gkkvadppf.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/ghuawwpft.sHtML


<!-- 参考信息 -->