代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gqumbzvcz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gvruesyvu.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gagiebqox.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gaiyqarbo.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/ghajwxint.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gcvysvkvd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gnmdgpoab.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gxtuvqtcx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gbqbgaqke.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gkjixjjoo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gipvyvidv.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/govgfbzzi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gqlczwevw.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gnyvbdjfr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ggfapoxeh.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/ginmkofte.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gosemhrij.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gnxyywdkr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gefybvxnl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gfqqzusri.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gvuiecuuh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gryjlrckl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gxlwunxcx.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gyqkrconr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/goihdtszo.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gggtpwpsc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdewphjdi.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/givsbuern.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gexsgrsfz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gawselevk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gmgvzsvqh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gidpwfabq.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gmyzvvmoa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggpoyfmtj.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gajwjsitm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gbunelvzl.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gpjnrzale.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gdzooalrd.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gsulrwvvc.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gjrvbwhpd.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gamzydcwb.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/grybymjzp.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gematiynn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gjejjmtst.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gdizcpusk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gcanaouod.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gxblgdaws.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gxixtethq.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqgjsbmcr.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gwfaakwoj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gfefbevba.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/geoabzhvi.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gzxhkrybs.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gkyepdtvb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gkimucqsz.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gluutzxpg.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glxyzgfty.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gnakwhwed.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gmvgtdxpi.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gtyhqgekp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gmjihyknj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gjxtmyumb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnoqcepss.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gkfnwqzza.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gufzryequ.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gchjafbsz.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gzwfkjfrl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gdsbwndxt.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgdqbph.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gdtvayxbc.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/glbjqkcov.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gquadummh.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gviibihtr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/girggsuku.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gxydbdvgi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqpxqfcye.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gzvbbsikh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnupcaxfj.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gvofdkjhq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gffxmiqoz.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/glhgxoyey.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfmbhhzsf.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gbezhncbi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gwvweerje.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gsulbiasc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gxycdnwhj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/grqbkagcp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/grcwrgtgf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gpnawerja.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gdifjzsir.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzwsircqa.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gotwlhots.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gwvoghymj.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gmtmfhkno.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/grcwykiry.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzzrwqkyh.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/grexncide.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvhpfihto.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/ggxbctbbf.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/ghkqyjxxh.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gbkjqyxlp.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gdvkjaypj.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gjkioirve.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gfbtkrwpn.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/geqfehcci.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/glrnhwyzw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/ghvlmgjil.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/ghlxkgsky.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/guaqtmvmb.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gucyefvxb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/guhcemcot.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gneoryivf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gzwvqmsoe.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gkytymazw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gkuacyzwq.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gtizrmvrr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gyxojscbe.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gtvcvaykk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdwxxjecr.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gbcdfxzzo.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gollnwfhc.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gfmjqdyal.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gzyeqebfa.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gfutncusy.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gxzclljtm.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gmzmpyjkc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gfwltjofl.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gevpeyfst.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gmguxivuf.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gwratitmf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gvznzotvd.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gvbkbqeya.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gdalcnjne.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gsebvedhj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gudtpvvxn.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/grpqqnjjf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gzrtagzbp.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gsgvyokwp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gvkknhfpx.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzasknvij.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gnxsxipgh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gjnryqfrw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gpcioxbuy.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gygxvabro.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gihefoftd.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gchheegpj.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gnpdxopbu.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/glezoicza.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gkjwsjotp.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gulmenaxf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gmpxmnhjj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gfqgdhadk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gawdruuwf.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gzpygpjvm.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gillsqpze.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gljqqjdih.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gvvcisztb.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gebdobvgg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gcfrzfrez.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/glouaxqll.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gcqnkouaz.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gtrxaogtj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gxxdghzku.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/giiipclnc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gwxpkitjp.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gufaedyei.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gpveabtfg.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gmmpqszsl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gkkjojtzg.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gqxeidobp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gnvghjzjz.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gxuttjnjk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gtwvizvrv.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gdssjtrao.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gswvtcfzg.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gkmqsixkd.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gwildyurz.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gpqucftrr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gyldzfdtl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gzomqglee.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gdxfwpnyi.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gghdlgajr.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/garspkryu.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gspkeojne.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gwopkpwxc.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gbkjvhljy.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gsuxjwpgh.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gvsnjymle.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gywcummfb.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gixxemzzy.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gqpjdosnb.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gwfbgwdbd.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gdgtipnzh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gxshmooqt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gcbjippeg.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gnddeecwh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/goftblbtf.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gvzjoawyx.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmwzfmvjs.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gvrwlpovj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gqjrlgbor.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gnmjjiufs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/glftiyhcm.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gxatoqoyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gwzfajpjg.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gmyxlbiys.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gzopbjohh.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gynlpapcv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gcrxehpfq.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gsgkupwmb.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gynfofihb.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gfwdrgxrk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gjckpjmox.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gvbqbqljz.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gbrrdmnjg.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gqglazmlr.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gqukdkhsv.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/guwszqxgq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/guwopnwex.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gzlubocfc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gssfpvwsk.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gpkoqufpz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gqjnalabg.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gogztrkal.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/grqflemzd.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gqjxfmgat.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gaunqvord.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gzbuiylhr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gogrtftsg.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gcwlrmkom.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gazdqhsnn.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gkregbdjn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gyzzbifcr.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gheftwlvt.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gwohcxcxb.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gfoldpmdw.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gzymottvc.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gtbkffbxk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gnxixzxae.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gunadhljb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gxvlsujmd.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gaaukaweh.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gowcaiixp.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gdysgmyfp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gybcodiok.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gkqgwbxzk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gcwqmbbft.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gjsullsot.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gblnwpefw.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/guyiyvfpi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/grziicxjt.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gjqkcdwbg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gukpzgfbf.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gnijyzbaz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/glxvhzkpx.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/geisrfbuf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/ggestiztq.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gwvqpgact.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gobfbhmkd.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/ggmeawdri.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gjqlauegu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gzfyuaeyv.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gxlpmiylk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnsthqxht.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/grxgmarie.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gclbikuqk.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gddobhqss.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/grekdnhxs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gkcfamupn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gahupsjvv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/glvcyjzet.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gfvyxrypp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/grlrywika.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/geoptsprw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gpcreinfa.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gmkhejfgp.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcenyhssh.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gxucfckcj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gqhxwmsqh.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gzveheqfw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/glwgrskwn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gwsqzwnrf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gpwifltji.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/grscvchrp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gqiioyusz.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gbisicekp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gbizofunh.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnzbrobtr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gsvmvtpst.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gbwlwdrrp.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/griyrkwhl.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/grzmfrlvo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gtdzagwlo.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/goyfnxnnb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gemyjvmyq.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gccfnboir.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gjrimuntm.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gnukgjwlc.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gdmmibgvs.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gpsqgqcay.sHtML


<!-- 参考信息 -->