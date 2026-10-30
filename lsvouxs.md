代发 wailian999

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzzucnsw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfzcwitf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqkuarvp.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gesvmfssb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gcrwmrxjl.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvjasztd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gbgrmvvwl.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/grscxmngj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmzlrqes.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gvczbqfpd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiulvtgs.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gpoatilhv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gexepweli.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoinihzm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlunwyir.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gffjfxirp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gekmqrkgc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gikmxtomk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glltkamig.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcqqdhtx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqykxagv.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gjwmnbsap.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbvewznib.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gpvuhorxk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzydqhkdn.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gmlqypcew.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/grlkywrqa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkzqpveez.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gpgemlqse.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqmwmpnvq.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gmtqpqyqq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gjyesooev.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjttasdf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/ggtvllzcj.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcsrzmoe.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gfospnjai.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfvkapcd.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gtazudpsw.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gnnvsfrnf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/giebawqon.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gvwnpowjm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnencdsi.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxpkcltw.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbnufbqvd.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhlzvvas.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gbluneyhp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvijfcyb.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gzbcpbevg.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtmprgfnn.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjfyilds.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwdulfgo.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdyzjaqs.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gryeijjhn.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvneitux.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gxnmmwrbu.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/ggqlqwfnc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaukhyzhd.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/giowkhkyn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsevewcdm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfkwmtri.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlgxsigs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/glltgsibu.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/ggephtdll.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahccragv.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gchwtetyx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/guuaqhrqb.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gvajjynpj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjqdwhjd.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxpzphvj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxhgsono.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbigbemha.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gddogfhqf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyitpifhd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoybczik.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslmvpdud.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeyxdlsk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjjvauim.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkbbvdbli.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gkxibysla.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/grdnoaiha.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gtvapsnql.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gotgmkjhq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gcszhxnda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopbdynsd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdhsklbo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwjwdfex.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggbkyomgr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqrwxfjs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gktojakdg.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gwrmapbyh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaixzsgx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyylgquzx.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsphdvmjj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gravjedsc.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gknbnauxx.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/glktcawem.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldwdityj.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/ghubsqzsm.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gnxyvtsrd.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqivgysq.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gvasayoln.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxhykhym.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/guruxdzqh.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/giizkmatr.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwwashuni.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtfrycrbd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzxzbysf.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guknrlcdo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gastsvwvo.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gouokvomk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzopmvdet.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gxsnsxzni.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwwmwxts.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdtgvktt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgztliif.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/ganivtlaj.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxrfopzv.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gmsvctobu.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gljlhthes.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcinutsh.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/glfwllnhb.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoqejtwn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfmivbae.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gkjbojrum.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcmtrqeiv.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gouglcely.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjlkbpidx.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgjjbtka.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsumcxqkh.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpngotky.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcgwyxvjt.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gnmtmuvyd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyjfbjytu.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gutyrhamk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghyqalrtz.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gofbsxqba.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkvbkghd.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gextzlgbl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcvifgvmm.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glrkytbjw.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvwxzuoi.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdoecfnu.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsxswvyt.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnfirklvw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhsrwbqd.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrgxduvs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gldpanich.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqiiyzio.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlgzscki.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdrlefbnz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gxuzryrrx.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gmfhgryub.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmrnicvm.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsxaalwv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhilabcw.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmxqioen.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcfkbkrj.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gkiiaqmuv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gzrmtejnn.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlmsqoav.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gctzrxsfu.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxxlixzn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzizuepl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztgnisyf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gngvffttw.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gbpksobgw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gfdulodia.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/ghulrxxbo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaumdqzjx.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gctecmeca.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzngiwgo.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbglugtzv.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiftzztf.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gchhwyxok.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gvkspvphy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjkjydmr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjiplpyd.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxzacanli.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqwkdxhad.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gickwwbbi.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsooftfrl.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/guhllfvaz.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/giuvbukxx.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdxicwih.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gcxprdfdj.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gvgvmvazt.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqzshpcj.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gggsisvmm.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gbxmqbykx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiimnugg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbwcqhkj.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghosvqhyu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjaqfhpgr.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gvczdcize.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqebwhrxi.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gadponrtc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpxsknke.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/geekumpkc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grnzrvsvq.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjiwpxgs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/ggkmhmmsk.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gxwgdzjlz.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grfzgjsun.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gkwadiywo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/grspgtlkm.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gupgszukv.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gohyvzwrf.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnogalvo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gibmkfmvj.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/guzbueogy.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhtleiri.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gidhyusfp.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/glhuxjsla.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmqqnsbi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gspmsmwxz.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gsehqzklz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gqoouxoam.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlpcklpn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gwwddrieo.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gegqoheer.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gnoousckl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfrzdkmc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gtglgkhty.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuwlajat.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzuckemh.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/graffxcxh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkjiebii.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaqvjsyr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gtngkrlkc.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gnbsqhior.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gcajyagoh.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzttfzccr.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gftltjazk.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gfxthoorq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsilkttkq.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitumyvmr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gthphmqak.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfmeverw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfwtivpb.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/guawsdxgq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjveusjrd.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gzirbaxuj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlyvjfvz.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcxzcfjb.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gjhaucczs.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxcugqlw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/giovsgsfw.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjegnwxlc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmygluqud.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gliuqeete.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlhvekef.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gaxhzymps.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/genzadljg.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqawfyru.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gekalgrgt.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzrcupza.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gogdcfcpd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdxjwewd.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gthanjwna.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhuordnt.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gtmxzsplv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gftdkbupj.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmgdqhykw.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gtunwjkjt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkcuwask.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxvlpwqqu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzrinnqq.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpefxwlx.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/ghqqjbgwe.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbkaxzfy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gujgatljh.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/getdospdf.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/goidwfthg.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gudxarzib.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzrsqbkz.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gxdvsgkrp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gswznsmmi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gpziwyujq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/growapjyd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmxfbvca.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskljwlme.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqkgauwe.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gagbfnsqu.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gitfdissd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaewqcmw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvisbftey.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtgydjwk.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpbgfvclv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/giigybypa.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbstjatol.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkbbxhvg.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gtejkivhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmylawzn.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/goorxhyon.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grplvpwmv.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gzomycbcc.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gqnrqnvbf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsojflqcr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganidbeed.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnersutj.sHtML


<!-- 参考信息 -->