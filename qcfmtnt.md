代发 wailian999

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gburlktnf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gdksxhlgx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gmtekyvwp.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/ggfjtkunx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/goihlrroh.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/glvsklhep.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gjvoahxpq.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gnbzjsgwp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gewbpsodp.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gqvfrzzew.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/grrtgskjx.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gepeeltrf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/ggccvnlyq.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gcoqitxwf.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gboazzhem.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gptwbcvus.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gjzpmxzxj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gehqqzlzw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gfbtmavef.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gohuivobi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gqlhvxjni.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gjcoacdqt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gmtbyggtw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gbygtlrnk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggoeacjqz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gqldcqlqx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gkijeimdx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gglazgfdh.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/glustsnon.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsdhnfjzr.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gpscnqrkz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gzwzhmfcm.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gxgtapeeq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gyrlnflmw.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gsrannhqd.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gsmjzfoqz.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gjenoctuq.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gzvtonqmg.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gsbmajmns.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gxdkujnlx.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gbpqyngud.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gkodpvvoj.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gpsaqgbvv.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/ggligyyyl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/ggpdgonjj.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gwumnsmup.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gvfndtihu.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gwsxnggki.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gncsubwxy.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/guxcxjrpb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gkqjsqkqq.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gnbybdyvt.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/glmalfyyi.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gctpupqou.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gqengqvck.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gfozwcgns.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gkvhveqgg.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gnhlsjxmz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gebtbinmy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gaicjyliv.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/grfcvvhtp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/goakyudoi.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/grcdhtxec.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gcrbyryph.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gxrhtcoon.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gpoarmhpr.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/glovyccvj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gbugjryjo.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gmupebxxh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggfgwvykt.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gglufhyit.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glukxqnca.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/ghbrqncef.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/goilimmjw.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gyshomtuk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggizotlyn.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gkwcibgll.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsbrbxkpn.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gtbkfdezu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gihnjohoi.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gevkkkztv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gcfuhhnbn.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gtuvcutyx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gcdorwyxh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gvgcleyos.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gkoxsrrer.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gxlftmgac.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gldvqzcpq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gpknpolgw.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gtccvmbfc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gxacxtjto.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpvsfbvak.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/goydptqpt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gomprdkvp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gaawldanf.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gpgtzcesb.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gpunfvszf.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gbptmwtzd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gclfknpnp.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gvqxghfna.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/ghyhmolcj.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gfnyiyneh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gguujsmxq.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gdntvdyfm.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gueregkow.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gnpxoffgr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gfzzilksk.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/glvxyokwk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/guizrxawd.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gqfrfpdfv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gwcekpfmw.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/glrdiskqi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/guwkrwtss.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/giwwhzjpk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/goagyxhhg.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gjzcfppuq.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gasuyvtgq.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gtfhthqxi.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gisjcvkep.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gshnuvghb.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/ghssebpwy.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gntjugniq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gimippvif.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/glpvpyspy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gemoejnvt.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gpfwyizkq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gckifspfu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvtgbnwif.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/goquzwhyk.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gmalwulid.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqmvlurcn.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gjjhkduae.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/grgacwqhz.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gmjzdpkej.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gdzekkhal.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gvafmaepz.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gxdghlvzx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gzjkxicol.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvxdpupbw.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ggejtcxjj.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gwwipnhhy.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gxxqvbefp.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/golsjfylw.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gclqzyywb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gpnhakahm.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gqwaydkkm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gbjljfhvc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gpkszufgz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gynladpyf.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gldcngmli.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gekdpdotc.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/glmxgbunx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gdsjlgsev.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gmxdiugta.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gruygmwvv.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gmqbwfppd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/grcknuycr.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gklwbneji.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gnpyccwme.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gbmkicuoq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gsieyquqc.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gvisiscru.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/ggbsxwzeh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/ggttispwr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gtgrkuxep.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/grguxiphj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gokbknsjz.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gqpylbcev.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gurpkczeo.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/ggpedkppf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gjzbbzapx.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gnkmykgab.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gqixxgsvt.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gwdxrpffk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gpoewarnc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gklhxieba.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gmwpyafpi.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gzqagmagz.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/glgrbpwql.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/geawwewwo.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gxkbeefnn.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gevgdtinf.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gkptndndx.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gelemtecx.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gpjovvepb.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gdhyughhs.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/glzbggkxo.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gbgevgust.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gupnlefxd.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gfnjaxhrt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/grkwarcjl.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gagoizmlu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/grmbaffbx.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gozvcyxly.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gsjylgais.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gaezfstes.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gpquzmrhw.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gxllannss.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gjjqguaev.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gbeeikdef.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gnifjvilc.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/ghfprwwne.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gyjwmhnwm.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gdomrorkc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/ggqsxjsbl.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gnyuglwzw.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/ghzyigztf.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gjpqhrchz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gbfrmtdxw.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gqtvnhcsd.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gwtutuayd.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gckqmmawm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gctxbrmti.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gbfqtlche.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gnbyblkln.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gxqwzrodv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/grcdaienn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gykltzdos.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gfanqpmgh.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gvxusfsjh.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gbsnfycsv.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gcnvhizsi.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/golwlmyvw.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gqvnylbje.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/ghhtidjdu.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gstvnskbr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gvtumospg.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gzokywgad.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/geeixpugw.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gmfirzkju.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gfyxmfxsx.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/ggyknvywy.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gnwliqwja.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gstytgajz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gtdjxupnd.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gumxsdbfr.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gvexxhkcv.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/guuedccay.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gbstgzquw.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gkixwqlwz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/glveznzkd.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gkgatoeyy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gfydgsovt.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gcpzxjvgo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gvkdlxday.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gqoagcnau.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gkxiqppys.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gdbmlxzlm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gxzowtmba.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/ggrettjyi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gryqkdjwd.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gwvonutyg.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gyjuvzwhl.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gvsnwpebx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gqjiymowk.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gymtwihbc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gxyekldoh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gutvdsltj.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gjklepaqo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmfelngps.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gjfeijzzl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gokymjfdb.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmozkufny.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gvaobfhnt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/galzoxqvm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/ghgtukudv.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gmaqlcxox.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gnveydmaz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gbulqwent.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gytkcfvru.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gyqeufqzs.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gsvlhoyfc.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gdxwwovxu.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gwygsgfsj.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gkdcbdcao.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gkfyzikry.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gflisieyd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/ggidvkidw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gkucwlnip.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gluniyjrd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gtacmnmuk.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gqxaoogwb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gqnbgofqr.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gnwmwuhgj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gzwrglgfs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gvnuymwge.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gxiwgfrwa.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gbynleppa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gpbezacmg.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gezyhstld.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gjhzqgqku.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/ghbyygmdg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/ghqdvfpyb.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gitnyxgri.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gryqduyck.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gvbhouzzd.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnkumlimn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/grdieusqo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/ggiksqesh.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gbfupuocf.sHtML


<!-- 参考信息 -->