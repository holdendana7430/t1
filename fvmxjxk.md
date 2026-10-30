代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gztannfev.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfajutxz.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfdcoiybl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/goyilzabf.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnobvqqzx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzziyyvso.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncerhefr.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gacheqpys.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gcrcphvon.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/glicrryjk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gtmgneryi.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbjyslkh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgwfsuoi.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdulpimz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnajvybdh.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gehkdoauc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvfxihyt.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gndbgindw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gosyxzrtz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gulrwngah.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gczuttkpc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxlpqevw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynnlfpdt.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gmnwokklh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnwszomda.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/grpwvnddx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guedzjjan.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrxkukfy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhytamcz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gjtgzqvau.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gockkjgkt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglodrytz.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gscrwiiam.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ganirgmht.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gqujkvxxm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqruzcspj.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gunzodmyd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/grbjwjcsh.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gawyxkcct.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gqijwrigm.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbqojqqq.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoxgxmel.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwtvmwsbe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gorayuxhr.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gfqgdedvq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiarypxo.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyqavobo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrphakls.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlcixmhd.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnprgapx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gdznksacf.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsutbofsm.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gzoaquvra.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gswvqmcax.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmylhktv.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/grftfsdkd.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gialvcgwn.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdzrjufr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfewothx.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnffsdtda.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbadizjaz.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gktsgrefb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsviyrbks.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunlilxuj.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gqummvgzp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gwedtycnb.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gqcnsplsu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gnklbffra.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzretitu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gusgpsftc.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/glatjrydq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoqdfymr.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/grwkistxx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gulshmamo.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdaspbok.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjceokcuy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvgcdsxc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gshajxpop.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gocsqleqv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtgegixr.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsqxacys.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvwfbfiyv.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbgwkfvu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnonjmky.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gyxhlnqtq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtbmnxlt.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfrljscrp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnfhnfwq.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqlognaf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gcizqwrlp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbztfpejr.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrddsoay.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqkvcjsb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebkqbdjy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gzglicmfh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmrhedbag.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfqmwlvr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzmnszgg.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gztdaorwr.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gljnhtaxf.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/glztvwewl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gitorgvjz.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gciccazjf.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffvnqpho.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gynqjrgsv.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrdlijku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/geoslkkis.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvrjeydv.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glalchrmv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccvkzajo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfytaufgg.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gagrsrfme.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdkcjkgw.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzdfymki.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gumeercga.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsjdumdh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmgyinhn.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gyvzltrhp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gcasugcss.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdvrmxjm.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhbfmipw.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gimolowlt.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwddzpmtp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzzptyzy.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkgwryhw.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcybufzta.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbycihde.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/geonlkbkt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusiidelw.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmifxrijt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkysesmyd.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxpcparwv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givuvgcfx.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gnnkezkdm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvgmpvjo.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gdmzbcnrr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gilbllokm.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnntwarf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gltzhgjkd.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjrrvmsua.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjyvgeiyk.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgwlnmcz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gobltgtfb.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfwvtehs.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghprczzuk.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gurleghxr.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grraqoytj.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfylyjj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwapbahwt.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvixunkhp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/giqhgjofn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gddqbvofi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpupbkec.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/guyofccis.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtooxlcjp.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqifqxsq.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gnsfvymbf.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gihozubow.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gkdgpdina.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grrmjwmoe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gstdjcsau.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/goneelgtd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gufysvfsu.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcsdffmgw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxyjjkpu.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsybjiok.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvoprdjuq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyuboihi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgfytzdc.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gqehkcjyd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpsonlfn.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gghkebpqq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gscsemygs.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfplbrep.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnlnykoy.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmzetvzjp.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkxgxuytj.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtqknaij.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gcvzagtvu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gftxqimej.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxufiopxn.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gipzgmuvd.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvjtgsyo.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjpavgnx.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiyuntaj.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gwdmlylpn.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gphpnfauw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzwpvrni.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghhzbpnsb.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gydulflya.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gqanrteil.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gfpwyqtmx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocetfbrt.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhxrxlze.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjioyhvq.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwpppzbj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gccwvrswy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxwcmmkf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhmwuxxk.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzvvvfnne.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnwomdqi.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gnhzppwoj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmtsatpta.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwemxidg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcjsflvj.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gaqiykpxm.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gofonyhrf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gmmdultvu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwdqnqhp.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpglbtsyx.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gripzkmpn.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gshejwahn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gxcxegkbt.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgkknsdc.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gftwbrznp.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmcctzml.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gttrfdocq.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glhyphjqr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghedmxdwz.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcpqztqv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gsklqfqic.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmltscqxr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gohgjnpbh.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdadfesat.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gejtiulel.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvmodgze.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyblvsklk.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvsdgarl.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gjezpswmk.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmbeqjit.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbktapovx.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gmseoznou.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gsczaxtfp.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdyyggrf.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwsvrzgw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gmromjndq.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwopgszdm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmcnogor.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmcocsuo.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gawhogejs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiwbtfse.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegmymmzn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuqjlbvo.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gssvhrbcd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkssxphy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjvpooqc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjyzqczvb.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwslsxvg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghksicdsu.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gljcrgyok.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gomtlxvmy.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqqpqoms.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/ghffkfbkl.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdmgqrrgb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gunkhpwzb.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaudatqj.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gbenzfrxx.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gracxejuz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjnxaypqt.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gmdovtsde.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnhilaut.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gtrjyjoln.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gshrlnncn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpbabsjov.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiyurxxa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzofupbrz.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmpmhxvb.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/guriizlvt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guewepsne.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gjapeiphm.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiuuqrpe.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gkkxkrnrs.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/guuxlcxsq.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gcbojnxcn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsmrwlit.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gsmybkjyr.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaycybdj.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfldadnui.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gdletkxoo.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gygcbwylj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfkfpzdk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfijurbhe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/grdcmopnh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gquqxdctg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfijvnva.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gdqvxddug.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsymnoibi.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsuabwuf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gapbamznd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gizcdlxpg.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gpkvsteik.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiejwtco.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gjcfohabh.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcnntdeg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkchlfcur.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/grfekziqf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeyxasuf.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmmkuvjqe.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadetwnjz.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxkbwjkg.sHtML


<!-- 参考信息 -->