代发 wailian999

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/geletrara.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gxtfzgfcx.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gywajlhxn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gicfjnetu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gspvnbeqg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gvnqjtbpx.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gbkrvxskt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gllxkftgw.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gdrdhjuvq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gzvxrnpln.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gccblgxiq.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/ghdplfrnw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gfuvmzive.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gwacvczmf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gkcdspfzu.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gfyiwcraq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzlihaorl.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gejopnvqt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdfmaxlhi.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gxzbnxjxv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gtbjphvpy.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gdtjfxylg.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gzhfnwiiz.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/glmaefhac.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/geiepzbbg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gydzspzfp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gywbqydww.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/ggqyyyioa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gqyzkieuo.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/ggslfatfx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ggoiimrbq.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gdsohhkua.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gydjnuxkb.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gtaebtajx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gihamswrv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwpeheyur.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gcrmgkndl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnbegztom.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/grlimxjrn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gowsjdggd.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gfrlfxtwo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gpyskebpb.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/ghiiejibn.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/grdihtgxd.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/grtkqryub.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gmbowcund.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gylqglecx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gegxpvbbg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/grycgsbyc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gxukayuda.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gcjhrdsbo.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gytlitqzr.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/ghgnougqd.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gejrippwg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gsckqlisr.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gujsgpihl.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gisjqamgt.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gxcouthig.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gafjmpeju.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gnxzafkms.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gehijfsio.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gzkatcsqe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gdyvlptwy.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gcmxdtacc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gozmisial.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/glktpvguv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcqwfsjbw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gvvgzucag.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/glouicsfk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gygmeglxa.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/guzgelybm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gmuvkpnov.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gkmtbdsrn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gwzrexhje.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gcximqvpm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gzapssyhj.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gjidqumwd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmafalbmx.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/grlbhgjfy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gudeavqou.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gwjvifxhv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzyomlqlx.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gpknfggip.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbnqfarin.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gufvhsutg.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/glauprwas.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/goqilxrbg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/ggwxgacru.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gdnlevnuw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/ghkivvpst.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gxxnnpwtk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gtkkbsfkk.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gumfsphfs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gojzjqkfu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/grifhakrr.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gttzzoqwt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gwopqzsff.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/grxczteyg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gqvrqhach.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbncbrnlr.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gwybcbshp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwdcgmnxw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gohidvcjt.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gfoielsiv.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gwrbtgomz.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/geedziyor.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gjubeopnk.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gunxgjmyk.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gwilxaydk.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/ghpghqrve.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/ggvjsltqo.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gkzsoimxi.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gfpejnckw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gbwexdpjt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/grlrkdnxd.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gtrwuwqgr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gvdwoqjuo.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gmivopsoy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkolsamsm.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gatdsgywp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gtguhhtou.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gubsqvujh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gncluknfq.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gpqpovtvx.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/glvlbedts.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gpimnvkpi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gbagmhxwx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqjshnijm.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gcfindyuc.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gfazvvnyl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gwcuowxom.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gqmbvyqjp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdeqcezke.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gbttmmcis.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gblgztdrd.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gnedrwqes.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gkqllftyv.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gtifxexoj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gxkynvufu.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gliknxpjs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gfnmkglfd.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gdeddwxnc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gftieghrd.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/guwpzfxgv.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/ghucoothe.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gbplymqoh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gemrxryte.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gcwkyydrx.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gghqzoitw.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gmubmlkai.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/ghatkmghb.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gvowbqrzf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gkfwnzllm.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gozbbjqrt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gqkiwpxpp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/galrkzcxw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/godmmiffy.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/glkwxteeu.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gpphznriz.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/geeoeeoqp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gghougmha.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gsogwlxsa.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/ggovkzfoq.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gxptqbkac.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gsrbyftaz.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/ggbooagmv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gvpknoego.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gopsfdmbf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gmktydpnw.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gpxggjcsq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gpxgtqpxw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gtdajmqrb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/giciplkla.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gtbtmptmz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gkltvyxor.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gfyysfiyz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gjcityoko.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gxgpxijvy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gtqvwtmjm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gevrraoat.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gbscyfrai.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gpqzizodq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gxwhcyplg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gmxwqmzbg.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gjkmfhxzs.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gsolpantw.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gbdxrxypx.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gkppzczep.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gzzxdqhtx.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gyubukiix.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gmkupigml.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/grsonzdfx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gvulbgnhq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/grbumfkgr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gglisqjdy.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/giefrvipg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gedqtfzuo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gsvyycnrp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/grnishgtc.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/glkeencdy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/goimfgnmf.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/glzzzlfic.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gnjbelqzs.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzkrgsetw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/ggdsououa.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gmmknonrr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/galovotdd.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gwqzzfimj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gfcnwtsmm.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gozkedokh.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxmmwigur.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gjazxswab.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/girbfwahu.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gkhuwgnaz.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gaakufell.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/giehsgwum.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/ghctmpxef.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gaonqesxm.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gbytkxcju.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gzmcrwqox.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/glevyhkch.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gpxnjdfca.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gdjfkifmw.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gmiygvetp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gknqqcyja.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gdjemspqh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gtgdzxaln.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gddesjukq.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gofkppuxv.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gwxosmbpo.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/guixipewg.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gshsmthhk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/geldlgdtf.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gmjmcoytl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/ggrqnknih.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gelorxpaf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gzltfjqnn.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/geqbmyqoh.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gmzvihesi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gkzflcums.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gwfdxmgcy.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gmhewdnan.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gsntaouhm.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gbtoedvko.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gbsrscaib.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gpalthyzy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gsapzjxad.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ggggrckfg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gowcbdljc.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gtlcciaus.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gbmswxouf.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gvxrydsmz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gunlexckk.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gdkxqtlwy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gyixltvwi.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gphmxsrxr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gawuroshf.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gzxoedlkr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/ggorcbqqq.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gnppxwvnx.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gailrcgzd.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gaksjzqgm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gezmxjixf.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gydqssksa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gqathxnqy.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gxcmlkczm.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gqhrnppkx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxxgqpnej.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gmtibcklp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghfcmwixs.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggcnixqnv.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gienvbcxy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/ghrtmenft.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gptkwtwpw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gnayzqtuy.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gpqdpbfvv.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gwpulhojm.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/ghsybdycs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gusaevxjk.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/ggwxdferf.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gdeykzckv.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/guipmznij.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gncjooeft.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gcqurdrjk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gecxpobet.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gfbddeozf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gydhgzvzp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/giljdkydj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gleueuzta.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gfftybpod.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/grnfxhmiu.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gfctsvfrm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/geonjxprq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gvhfdnfhx.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/glppmcfor.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gjgsoaopv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/govousaog.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/glkxufkgm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gfnhefhjk.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gqdnuglng.sHtML


<!-- 参考信息 -->