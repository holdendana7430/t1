代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucyvnpup.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcraiudt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrtokyhw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqcdqcwl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glenklnuz.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxcvlrpk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqallrts.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmpawfrd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gcozbsriw.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gtgaxkmyv.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gwnzertoa.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gffhgwjll.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gozvmduog.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjebdpxg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcxwuhfk.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gikzjukds.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gldjnjrbw.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gynxopeji.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/giejoizla.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gfsxmknka.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmqpuluq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjmvlswy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gsgngkclj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxebazeg.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxcwshnj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gvraxbnui.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gaonpsxod.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gwjlspxlr.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gquigqvhe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gaggpkiug.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gfjeoehkd.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdteztnbm.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/ghyezwneg.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfhdwbla.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/glqefizbo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gviaunjcj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvkhdvgy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/glbmlptli.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gcubolezx.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmymnhmwa.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytmghgoz.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfkyvyjh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/guzecwvgl.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gimaqzuil.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamakkdgg.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gycrspjxb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjidsrqqz.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/goskkcznv.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnyotmat.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghelepvkd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gqbhpnruj.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjycpxrm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfffrzdcz.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gswglstls.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwzvzkoe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gthavpunw.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdquwyoes.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyxqhpcm.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyogojel.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gwyoqtqpi.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxutuksg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhfjfssa.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gevcryzcf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/grmfhafpc.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauqshuay.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpphuxqeb.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkxkaszhl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrqrcgeg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugfbihzm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsflgmbbu.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqtdugkwj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfljxwec.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gvinukpfe.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gciphbiqq.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmxlhcwt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gxgynsijp.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gsdftfcks.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gqaxvgmvx.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/geqwrehmp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gbqobummf.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/ggfelhweu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guejrpcyw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjunabtfn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/grozhanpy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkknltpb.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gjejaxzps.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcybapqs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsqlgdce.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/ggevkyuby.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbqnyslwd.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/grdttdrjv.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gyzwpgajl.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidpngykz.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gfmeuxgec.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwizhxgne.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkmivjyro.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfzkrtbw.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjgaukqit.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtsonulm.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gctgnhajc.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/godiadohz.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gquxkehuc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqzdnpqwq.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gglvnkdxh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzumaryk.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gykcfimxs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpujzidm.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/grudinkhf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/guipuhrjr.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/govajujcg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoduuwdm.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaeksalg.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gsojkfuqp.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ghyymyzml.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gswbjcmml.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgtbptjx.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdubuhvdl.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggymqgzcm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gftmnrqqh.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/geytfhcnk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grctijfyk.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gwkkyquax.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzfjprajl.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glkyzcnhr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gahfmdsro.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxksmkkag.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gymdvzioa.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaofyftf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbmlyrcy.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gzqmgsfdc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeczokjy.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdcunjrw.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glhazqttf.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/goxpvfqmp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscdrmjut.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/glcsiysvz.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfeewfih.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gesgrmlkh.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrbrhhzo.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/goabogtjp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzxaeaup.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gjrcqjhcb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghccyvugo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/giyhvnzpi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtmbffxhj.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiylgzju.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/goekoknhn.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/guurvbjnb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gajivgtrt.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzrsiwny.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gsrcvvbkt.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuqpqmpp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gagsmeqrr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmxdklic.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshfvbfcz.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gaiwqflgx.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghglwhjek.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/giqtbkqdr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyvdtesn.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gsksmdmlm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gqybtdpxm.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gsbxsyiey.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gefahjnpe.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gazicvqoo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzbyuawn.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gmcifgjjk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwjyusjz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzogosreu.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxdxihcd.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gptlntpcv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/glmimzgwg.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gdxflwhlx.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbyznsee.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gplqgdlea.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrigpari.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/glwtgncan.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gigefsumq.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gytsxlbnv.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsocblck.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydszcnlc.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ghugfimph.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gxfgqwrue.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gzbdxodml.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gdhhnprqx.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/ggfjounqg.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gzotpehpr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gtueftleh.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhcvsytx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhdvxemf.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gmhszzkiz.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gazibashb.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmisqnstx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gptcxnuiy.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnjhpmvi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibxfymgm.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gtovvknkn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkodatjl.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtendrwkg.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gapfsziup.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gmzctkurh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagybynab.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfrryhoe.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcdaomxf.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgiqxxct.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzqtcorl.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/ggadwwedq.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gfahwcvin.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwkbgnee.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/geoutlbpg.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsppqkfsb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/ghwiezdmp.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gxruqlunj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gsyonuncw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxdyhipy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmshglre.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gxbxgngls.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/giezzfrtm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdjrsxakq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gkijsibcm.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/ghrncvmcj.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwoocfre.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gebrwjslc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsshfqdqk.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaoclzvi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxmhiocb.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsngaiyf.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvhbftbc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbufhvdi.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/giffxnzjm.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlvqfvqu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmowtcysf.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gdewvtplt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gxgnpajww.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gpkebmqtw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkvyofxd.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gusjyoxrb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gbuljavbq.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoydzzbk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glwtfhomb.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcwappjd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrdszcjz.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gaugzajek.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbribgasm.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmvzgogin.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmxmvmkw.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtzqcqqu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkdcvsis.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdggsbkpc.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gxxwmqrta.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geonttqlm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsihkoqnz.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/glctahduy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvueaccys.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gidldykoy.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/grohbhicd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grbjilqbi.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gnxdprzst.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgtvcmgt.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjfchhnf.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqssfidko.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gonwyaory.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/giblpqkru.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhxusdun.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gojekizyz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvbyzgri.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/grfawmeld.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlnylftk.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnvjctrc.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnkscyukh.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqktxtwta.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvfavmkx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gurprdjsv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gvihaekrh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfkozvrf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/guvjsevti.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gaebkdzkb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/geozqgbts.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/goldehnux.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlsqztzj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdqdvggz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gdwhgtunh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmkceazdj.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gnluxvzps.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsvzqzknc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gkkhztlkr.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgyupqhn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/glggysxws.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gjoagxepr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gciqwgvcy.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gpeoiqzur.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gusqiuxdp.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpfmlsgu.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ganiqthzi.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcprydjwt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gowczdauc.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfuihvfbv.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gbttedojm.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpsjhkggz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gqydriynq.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsfguffp.sHtML


<!-- 参考信息 -->