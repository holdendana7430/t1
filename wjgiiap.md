代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdjxpfsk.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gdpuxomiv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqehkfjdd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvutzkhi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtjkomypw.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gicajusgh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gejcrdcoj.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gzqrgwhdd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gmbxqctjs.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gptjgcnhm.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjmhoorb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzokmarhi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnmkslwh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gsxmfoilx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcorhbhi.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/ghynzmcgj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzpxqmlrv.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gxaexujby.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyphohxhb.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfjtrgqy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxhsipex.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gtxlxtstf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gzfwcmwyo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxfdazss.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/galmcyczb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqkxqwra.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gluuxiiaz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzesywhu.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gqopjnhwe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpmulrjl.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvrknudo.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmcoughb.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfsdvawe.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gzsiirwok.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcdnrgsz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhrkyurb.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrputaae.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtabztujv.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/ggwocuepf.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gymqjobps.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxnwlvvr.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gasnbutxo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gqshhlcfx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggygpncfv.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/geygyxosm.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrjmpmxi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gtiyswouy.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/glzpmdfxx.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnccjqdsv.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gfysvynsh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxbghocn.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gptaodhuh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gyxsrpwhn.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyjzgjqc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/glwfhoncu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruruxljb.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gxecxlygd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gwrkfpmfm.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gtbkehkzm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gzjvgccmz.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gptqxspnn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjzikzqd.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gojqapyom.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfrswitw.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/goobmlphk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyecuoxyc.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gophlgmbx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxuptvoe.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gpsqwybxc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxvnjyym.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfucncmx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjolgwacl.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/glvsywyld.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxibloqa.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyvaxupj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaobdbnwk.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsrfzrnv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gojilsohg.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfhpdvcn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsvvqqnl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gnodyvuju.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/ggsyitcwa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbbkzxtr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpgifoic.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gbpodnofh.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/glgqyqbvm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdqmdpkz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwfbrlftc.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqozezzy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjtgsiai.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/guheukkfv.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gwanzonrr.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gxhtrsdnq.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gixupoevc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegvwtovv.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gedpavzfz.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtadmisl.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjshbzla.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrjdatxx.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxhmzkmc.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkdtkiki.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/grxzqfhjt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnbklqmmz.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaxwpypl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gthckfcjr.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvuwpkhhr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqngrjrne.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnzdtixgt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcqqjgyx.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gpkobmcde.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gncgmkovf.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjprnizh.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgmaigzx.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyjeazve.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gptlylxtq.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpiuvwiq.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyjdtmxm.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gllpdygts.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/geqaysgxc.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqjiwzhgp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpxvabdkj.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gqrefyeph.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnpkrdnz.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzngyadjr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpbwhuuoc.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gcbtefmmr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxvkxolin.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmruxvowv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gezjtplna.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjjoraqz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxtrlbcg.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaiaulpi.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdpsdarqf.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gtmjkkphi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaimocwlp.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvdqfyqn.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gftueqocb.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gdoenbqeo.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuwbfpke.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggytobrwj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwjvmnilh.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyehxvwyp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyobgpddg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gvdqpoiff.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gruleibbo.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvulbzajf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtzzhusx.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gysariadl.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiusyabe.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeaajzsc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvritqud.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/givugxbne.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasisusvb.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gwibswkbo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxmvviqh.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzpxtdtsd.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxamqzwd.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgmcrotd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkywkziwe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjylxxuea.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjenzqnsc.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/grhrwylos.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gywndcghk.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvfvmkxp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqkqyukj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gkilrtcuj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvdsjwjn.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqafikegt.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsjiikif.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gmehnvbef.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gfypzbjbi.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gomizgufj.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuvsbzfh.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsicylbad.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbomudzd.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gytyvwkzd.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzrwqxcc.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gudpbcyst.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwpzhiycg.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrecjppc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvlomapa.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gcxkzlggi.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gfetucask.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gaqqewhsh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/geefqkyhp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/genlfolsw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/guwmmylya.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gscbxmtet.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfibxtzzd.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwdasfdd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpelrkftq.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gplmslcnw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrcuxrtj.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gfhyazmff.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giijucneb.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/glfphkzii.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gcgsfpgye.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gbgwryqpa.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmvodawz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gwiycfujl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/guujkxbob.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpovaswlp.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gewxwaulk.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgwlwmbq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gexhgpzly.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gtzswndax.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gbszjhxhk.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gwycupcqb.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gadlvsmub.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glksclvue.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gepfwyxvd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcktzacyl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gbdsrlpus.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkffdqabh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gspxozohu.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpqfgmjc.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glellmqoc.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/grledsvot.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gqiacrwbx.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gcvvdigzf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqudcpd.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhycwtei.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsopdnwqz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmcdniyj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gdrhclpte.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gyyxerghs.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgvfitud.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/grllwkmuc.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gezvdwbtz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaimvgzdc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggewpuzun.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeyqaahp.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/glhpxoqhf.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gelpndcnk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gfazsshjk.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfosefil.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghujqmhnj.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gbwmpqmhi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtpairank.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfmtyzlk.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gljgdlona.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/guzvgqvbo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdooroeme.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbpzuuaiu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvhvlvuw.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glpphsdpv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/grqyeowmh.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrzetaly.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/geevhsswi.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gjemallfa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gexrfvijm.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/grquapjnn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpppsmoee.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gpplgmgnp.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddpndpfe.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwycepqy.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtnokcth.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwhoznnvg.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsipeiisq.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gknkeicbc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbldyaopc.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gvtsykczy.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyehhkkex.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gszwrbcdk.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrbjqjvj.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ggrgmbdjc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjgrsozu.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gljjimlzf.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgqgbvsg.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gynvmpoar.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcclmaxg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/glimihuvp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/guhwyxadg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gqfmaming.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gzciosrnu.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gbzorhece.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcberqvbx.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuotoowd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gpbbcrgcy.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgsdzraa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxcgrzbf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmtcgkos.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqlopnrbs.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqnwxlijj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/guskrlbzy.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gwijirrbo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gizzwfutq.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gctbqlbew.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlbcifti.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/geuuvoqrp.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoredlnx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwocbxtab.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gflvtywhq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfomfddzg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gqxbjyjgu.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxkpxhrdu.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gnldffixm.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gfsbhphjp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgxhmztz.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/grtfynqcq.sHtML


<!-- 参考信息 -->