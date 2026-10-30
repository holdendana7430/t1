代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gvrdmlhbl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gwdbgaygr.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiwjpsmr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gewfkojrv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzylieuq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaedzndo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/goqupsgrz.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/glhkntjwa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpjihydy.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gnecwtowd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvubmbso.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcishkrtr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/giciyiusy.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizdajsez.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gaqnoyzsy.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshhatzzq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgnprrsk.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbzwfxkq.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmwevxph.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gurxtjyqy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gnyhwergn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gxqdtdgor.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrzxsfoh.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gudplulus.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfcbdqfx.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gwmdfimle.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdmircvo.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbaneyad.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaplpowe.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gqpiiqtbg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjjwzobc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjkdricbf.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gbermlqtz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gsrjigyov.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigfhbwwr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/glmfqxhnp.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/grpuwgkon.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gampoccuh.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gywjarrsp.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/glexkagih.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gheiqrlle.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gfhphurjs.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gfzltsoze.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gjxsnjvla.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwalhikjy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gllxbyucf.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gtrmxhpyo.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnibajuya.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gsdasihpd.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/ghddswneu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gbxmegpef.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gpiudolxt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrjcruld.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgintojr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gdncbbgef.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gcxolbvay.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdemyrbx.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmhmgxao.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocygdliw.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gvpjsjzeg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdwcnjrc.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqxygtwpz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gsanaiwmo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goplmgvdd.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/galiynegp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gargksjys.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gvrhpqvmf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwdnnkii.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmygzvgt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gotufgalo.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gdbvwrofr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsqzwupm.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofhhfvad.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gteoryghe.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvbggdzd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gflpobyjk.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwnelpqhb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjegjgbgy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorbxxsuz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdavxszup.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjguajge.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeagqpmt.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gnbcjerem.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gprhlrbcv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjfalryj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfspasxf.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gaavcbweh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/ggksphxqs.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gxbtprzix.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gtuumcnru.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrfhwuot.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqizfxydq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gvnnduqnz.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnssgspfe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gldgpinym.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmiypvrva.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gtjceboch.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkqbtfnc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gebfvvkvs.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuojwxlw.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gbcnakhzr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtktmzzll.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gsybvctsb.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grbrixmml.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfcdtjmd.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmndvngp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gglnckkhk.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ghlawdbjb.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqihzkyul.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzmyablz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnzuympsu.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/guohypgjl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gdudphala.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gaikmlcnc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvoplydm.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibvdriez.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/giqmrjwrz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfylhyqtq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gbfxvmbnr.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsllmjsch.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gbxtwfile.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gavyatlfd.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnxzttgq.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gsnxhtfes.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhtzqlet.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhrcnudz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcztxqzno.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gddmhdztg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghggotpbm.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gdmlglchs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gusywpizv.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gclmuinyg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gunpdltnt.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuuxdarv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gekxlesvg.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqmqefvg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnmzeufh.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/ggeanzbnr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvmeydso.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmlsrslpx.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gblqxiisq.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gjsfhqtky.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyuyljssn.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbzbetowg.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfgrkvgu.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/ghhxjedtl.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyunrwlxm.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtmpwtls.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxwckiouk.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzivnvwhx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmonpijpg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfrcwlvf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfpxpkyza.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvwqhyzm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaathwnp.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeozhgdd.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gfhisztlt.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfdhmfez.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehsgoatd.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gotlblllh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfxuidfbb.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gbrbrxswc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuzseheg.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzaxghyp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gubcyzjve.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/grntemqvx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugxhpmgd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glghliyxl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyidftep.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/ggyajeudm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/guhjssshf.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gperuwcct.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptxsdrcf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gliqhfzar.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxvlmffu.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzkgmded.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gersklqca.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gxygxczwz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gqpqnyqir.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/goszpidlw.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcgjniwh.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyhdpesm.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gsafpnyev.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gbbopkcjm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gkvdqgbpf.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznwccrwb.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsctgcte.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxcoefwd.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbjcfcqf.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gkijtxnhr.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gykaxalek.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/girnoynek.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/grvwjsvmx.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gmkedlmio.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjhefjta.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glpzhdyym.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfyxgeqp.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ggephbfhg.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwgrxksnu.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfaxeyxh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gtjycjzgk.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gtdcmaorc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzssrgxq.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbxrgdjt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gwxyymvde.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsynzyna.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grkdfhgkw.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuteapjd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gosldldjn.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gedzjmojd.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grtedrknj.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gkjtxasrz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/ginsoixow.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqupbkvg.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giodowynv.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gghfinujo.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfakbxdkj.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gritaitpk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gbwwaupbu.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gtfpcxape.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/grqdmiawx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/guyiapvko.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gkxeulmyo.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gvwasqxbk.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gabkqkpvk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcwbzhll.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggndgniye.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gangwoclm.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxlxwtgl.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gbsznqtpt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gapquwkyp.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gsbffffcm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gtjgfkopo.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gvlmanujw.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhfekrlt.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfxjpvdi.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdsbcoqn.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/glboumcpy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfcjppcnt.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gzrdosygr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyyksyzu.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gcflsourl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gpizvcyep.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givjnmiwm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnyxtgjc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxynwtam.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfokikkqk.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gragkqedo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvvdpzkv.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwdmxlyy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgfjyjvf.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gylblwdtw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glijtibtt.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnjofute.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gntytzilq.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/geemepczs.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gykvpritg.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/giudjrtud.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggwgjzwna.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gkbeujgya.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdtaquit.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gnroeibxw.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gjptxelqz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsasppgci.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gvqrqslej.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwjthkglw.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfrdrbwwy.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gukigfqct.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/girigjxyr.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gwurwnwhu.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gborzzgze.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/guufourud.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtkeziuu.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjfgntbt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutkrdbwo.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzrgrwnil.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggvtcxofq.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqixdatf.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gutgckjus.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gkqivknpm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbihjcfqa.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gsextdjle.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gadqohxgw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqstuosv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gcpdxhshg.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzlomhds.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gueerwomc.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/goiteoooj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gcolfahiz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gppzwkjyc.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbqthsre.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggehejuxw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/glpseojid.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gvnfwyhcg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhioqwsw.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsskqqok.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsrjlxjf.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljcebave.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/goffdjalc.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gvlbjcgyr.sHtML


<!-- 参考信息 -->