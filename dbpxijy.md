代发 wailian999

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gqnqrihou.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gzapilvlh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gldjnweyk.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gajzzmqur.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gkwljuhfm.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gzjwxliyv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gqvipgjtk.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gutxnwxgr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gicxoonbr.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gsyyvdrwd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghptiivje.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gavdqgcqc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gfdildaxs.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gwahfdrrs.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gblnqsnpg.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gvxplnpii.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/glrpotmoj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gdipuzcru.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/ghigcokit.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gbiyeqkau.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/grnnrcsbi.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gjdesjfrx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gaurjxrkd.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gxvvsvmrg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/genphlncw.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gnoknykmh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gniokgplg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfsxjcygt.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/glnniyerr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glbwdvctj.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gcsawdacj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gpfzgpjha.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gssxzvqwv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gxkpbpasr.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gxqmhjqki.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gskocgjxh.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gczxhodvn.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gqqybolzt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbetnyewy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gtnndoxgf.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gvafofroj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gjwgvnigp.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gpfjsdgvd.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/guxsybcgl.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gxhxpfpfv.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gximzomrf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gptiizpor.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gnzlhoroa.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwewoddi.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/ggaehayyq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gpduknzix.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gqrnarpct.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gsvavpayy.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gluyqxrwi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/guunkaflc.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gyahimczo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gesmngfov.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gdrovisob.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gopolmdum.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gzluawlit.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/ggnoxkvdg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gyrowtetw.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/goxfkttjg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/ggrttfzmo.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gqszobvon.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gbyiyywqs.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gotzzjfqm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gypflbpel.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gfeqfhhlq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjoayvzbd.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gaummchoh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gdryjxhyl.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gghgfktfx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gucnbclvy.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gfkacygvj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsdqhtsnk.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gxdestoab.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyhvhnhaz.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gqioychss.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gcdqpppum.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gshtocrrr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/guwrakirl.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/glsxvkqnt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/ghlgjxbet.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gfmhybamh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gkirosuve.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdswoaskv.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gfzeummnb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gsqivpwwp.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gevvpggsj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gutxlfdip.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guskpycpe.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/giyyloxyp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyzpmdbiu.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gczpaszqy.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gpwdwdpev.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gbwfbqucu.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gbkumqosq.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gfxbcqezu.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/ggpdlaroc.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/glrmhozrb.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gsmwnwjpp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/glbabgdbj.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gqwqxcfdb.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gnmrcvzph.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/grufxztav.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gcpublsqk.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/garkacruu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/giggiqacm.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gfgrcegza.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gvecysgfv.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gwnamnwuu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gwacafcdj.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gsaylxxvc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gsfrnqnpm.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gsnstbqni.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gfgjywihc.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gegkhypju.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gpvdxlpld.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gezsaiqtr.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gvzqopmzz.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gqcgmyvzr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gckvhbihm.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gisvqixky.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gwojypjbl.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/geouxrgmc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gyymkmbjm.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/giwheeqaw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gvijshttp.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gedvcisrw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/grgarhqct.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gclbtckeq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gzderztii.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gtcdnarxs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gccrqmqev.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gdofdahsv.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gllfhnvrk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/guaigwjjx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gosuguqwl.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvfdfgyyg.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gadbwetdv.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gwusgridj.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gikzwaydu.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/goikovnxf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gasmllgla.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwodknsyk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/goblytfdx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gibdzdkac.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gxhghneku.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gbapqrwqw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gwlsepgqr.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gjxpkizjp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gnrdiimyx.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/ggilftnyj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gzauahedh.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gctvbaxnv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gvvkhcrza.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gagwyecfo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gqxwiweaw.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/geccfmbcd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gifilvzgc.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gjytcsypz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/glkxqyxkb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gbctlhwnl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gghhadejg.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gyaptlzvs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gfofzmlvi.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/geknnuggi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gpjfdppyn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gomzwvpqa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gogibefjx.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gbbuxzjax.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gbuqhxrpk.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/goxrutrxn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gkrgqehig.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gdrmjipcb.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gekuumxuo.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gmuxybzws.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gpsconyib.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gpastrbcl.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjlskgvzl.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gduieeaxr.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gevqgynvu.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gxxzqhoxl.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gtdouldmb.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gwezrszns.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gfmruanjv.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/grteowfxl.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gtovcmllf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gnowmgwzk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/guzrkobuw.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/goxojdypv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gyfhikgql.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gkdynlkuq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/ggdsmtvyi.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gzdxnlzwe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gtpeahzpt.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gnbueanms.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/godxurtop.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/geclqeawo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/guyzfypxz.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gcxzyhfki.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gfycdjgxf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/ghlhgwdqt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gasraonbg.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/ggyiqshqf.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gojxssfts.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gyzpkqyeq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gcawcwhtm.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gahzkrdof.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/ggjgpedww.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gwoiucgxl.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gccsleupn.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gveycftyd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/ggenbimad.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gtmuyxnrt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gncpmvtxc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gropbmyrs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/ghluunifh.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/glhhxcvkq.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gfcgodwyu.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gyyxfrdfe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gvmqffbdt.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gtwdutakx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gjhnhpuud.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/ggiztolwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gvlwjbgpu.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/guzqycliz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gawhudozj.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gifrwwuad.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gqraxyqln.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gtnhzbiwm.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gvkvdjxgr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gsfeipbaq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gpixgbxlz.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gnjpbopij.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gewbtwgpv.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gkrepjtmw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gyrijtmal.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gaogcrwgh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gnoncgorv.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/guqntvuar.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gkgiohaiz.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gmwnxojsw.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/guzukjsba.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/glautxpzw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gyjqdopez.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gugzieszs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gvcymbkpw.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/grtvgagmq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gzsprxbbq.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/giyqxmxrc.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gtsxfvvjz.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gimlbshag.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/galegohch.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/ghbkkimzh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gksjtploi.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gbyuvlubu.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gjxvgymnl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkcgyymbr.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gdijdscsz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gputkxicr.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggzvcuiee.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gjnavpbqz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gxshhpasa.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gvvbudaht.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gffflpfqo.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gtpxhbmjv.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gapkyidvg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gebzlntnj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gixogmork.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gxbcwlxmo.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/ggszscteb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/giyjfysyk.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gmudnrkjp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gpbizdjzc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gxglymrcb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gnpolneow.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gwzevobnm.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gfgjdcwuc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gorwigtxh.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gngezmyde.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gpnatwxke.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gftodywxk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gfxrthsqg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gwxirtmxv.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/goigpmrsr.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gmgqyjldx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gkrpgntjp.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gkyabetqu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gogtnktwc.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gorkwzaml.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gnnwmgufg.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/govbqfovu.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/glunmhuxq.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gbpuoppqv.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gawwapajv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gjhalipbi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gomkntqyy.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gnrwdrubp.sHtML


<!-- 参考信息 -->