代发 wailian999

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/ggxxbdtpb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gtvjpcnng.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gubvrfmnc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gskjsocpo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gysvdaqtv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/givzqiuut.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/ganramkig.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gngipqdpr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gjapcgtmr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gbzdoqvao.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/ggexkshyo.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gfrtzlshx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ghrdsifyj.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gssafzjuj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/ggrhjktxe.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gjmjpkqcs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gervxhfaw.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/guplblimn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gnvbjbgke.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/ggyojbrac.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/guisapxln.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/goexdeaah.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gqvdifxoo.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gaijmxqup.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gdagwagzl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gfhnjqcrg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gpdazhhwb.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gpsgfyvkh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/grliescgc.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gxwfocqep.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfnyqmsae.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gvhmdjieg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gtbvusbtq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gyonwuonv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gynnvedjv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzjkoiysr.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gbdavzyrw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gnrfkjcvr.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/ggehprmqr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gtuklfzbe.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gvorvsbcj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/ggxzlhnny.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gvateujmx.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/ggnbbhefi.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gyjprgnzs.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gzqbcqxkd.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gjdaipati.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/grvsguoyv.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gezxrbryy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/ggxenwuhh.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gsdawtpsq.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gznaficoe.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gcolbbrcf.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gltcpopto.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gkdfwszqg.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/givwyvpdn.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gfiexkvff.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/ggxybodqj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/ghzknmelz.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/goixrynoh.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzwfdoxwb.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gtfeiyfpx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gpiwidjyw.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gdihncnbt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gyuomdxit.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gcvipjhkt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfwcgzrzq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gblgnbvja.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gfqkhzxwb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gicwomfcf.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gmlbejufw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gmrtduuqu.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gcfitniou.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gygjiuplb.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gjclqknpq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gwgxdcfqo.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/grhzkyuaq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gazmcgiko.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/grqpaegkc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzaayjlzw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gmmqptniu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gforepekr.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/grgkpgbyt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gwovkismt.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gweuwyyzs.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzvsprwcb.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gwemubgvv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gfuaosgrk.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gmhpdmulo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gxrflvroo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gucibngxi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gperxuvvx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/giytlfjuz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gbhhikrfl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gcbyitfpl.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gbksbbjlq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gzmyqzvwp.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gxoqkdnxc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gmcxihdfm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtytngwgk.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gihfuurge.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpltfpqap.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gavrakldb.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gfuhwtozx.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/glkpewbjd.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/ghaoyzony.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gvggomivj.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/ghmmajogd.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gotikolqz.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gteolaiki.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gwdmgbtex.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gntkeivsq.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gptdtblgn.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqtypjm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gqtqvqlaa.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gqhepdfce.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gfzgxuhwl.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gobijelps.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/ghdtjkzly.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gymcgcpkd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gafqcqppn.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gjfyiczvf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/grzkgytkn.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/godqdnhqy.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gzutvmvut.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/guvnasixn.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gmzrhlioz.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/guwekusrm.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gsxtkajno.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gstudufuh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gpnhzmxhv.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gljrncpke.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gtwcduxzo.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gtmiuntxi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gnffyxkno.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjgdoaxbk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gbqobqmut.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gnlvvejlj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gjbeuxnmk.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gpjjdlwko.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gwctcvzca.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/geojjpwsw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gjuoddije.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gkirchxhd.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gzxykaitu.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gvlzozuif.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gccqkjiqg.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gtthehogs.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gxbnrawqw.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gzguidyqg.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gxdzbsgiq.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gyxilbrtp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gpwoafywo.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gultxsjfa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gxmodhsii.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gcyisaljg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gbkpuhswl.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gaxdlykxi.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gtfjdyzou.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gsbqfpfzi.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gzysygmqk.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gsxhkegtt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/ggbgxpnpi.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gigtlbrxt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/genpozusq.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gpchdyird.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gfbchxksx.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/giyepnnle.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gimypqcub.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gqmcsmovr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gzhiwkhib.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gkhvafwbr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gmkoxinxp.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gnuiglooo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gtckzimdt.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/grbaxlogv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gzwyxyurn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gynkiyyca.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gifqrvcwq.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/goheihnep.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gsdexoyde.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gfsrsqlun.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gifergxnw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/giqvvmndr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gddctwefc.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gbjfrgfjf.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gjqdpvvoq.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gkdqdkvhu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/grqpuyzgu.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/ghcaalhop.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gjvqvkghk.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/giwrinwjd.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gzvwgbqmo.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/guejsydpd.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gaiadxsfo.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gbuzrrkgs.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/ghsuyrtyc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gfqxemfgs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gzxvfurtb.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gcyqdcqby.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggsrblyoq.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gkumpirau.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gmdtvrakm.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/ghqhtvfjq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gprwydriy.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gfxqqomrw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gwmbhnocp.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gkrvjqqrb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gwrvkrdfu.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gengirtwa.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gzlgznewj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/grprrhukl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gyxqutewe.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gugccypjl.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gifjuhrxe.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gqgcaranv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gsurfrpya.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/ghwnngofc.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gsjdoihjz.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/ggxezizru.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gczptamek.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gvlpvvwfd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/ghookuvqo.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gdnwkbpdb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gfvoaotrz.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gfxhflpwv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gqeopatod.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gyiaolcku.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gjtopbltt.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gimrrbkno.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/grqwteerr.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/guuczcsvi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gqjpniosf.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gqvkxjipe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/geajdafcl.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gfpwsnweh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/geyruujms.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gpkdqnupu.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gexrhcuzm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/giqerkfac.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gfgwjzvia.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gijzyzcqx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxtfvdtxu.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/grarexphv.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gjqzojbkg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gyniowjry.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gbzsxtucn.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gbfzsfhxm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gwbelyzbk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/ghojqjomp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gczetcfii.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gheduktyn.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/ggyyxqojl.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gucvwojcs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gjpoihzuz.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gpkrylfaa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gkgxgamup.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gjspqpvpj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gtdyhttkr.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/galdgvhtw.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gszwbwojp.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gtebqjyax.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gjdupcbna.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/glvzxmafa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gztsgjeor.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gpabewrms.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gumqjemyz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvbeutgbh.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/glxicnlzm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsgttcnkc.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gelhnbxgi.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gbacvqmss.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gzvpykans.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gcswplzul.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gnsrfirla.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gbmxdetnk.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gxzxbagst.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gzmrgyuhk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gkrqvfqfb.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gcrcshbph.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/ggmypirkz.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gucoljszm.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gfrmxegmz.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gkzqzadaq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gxzzecvtx.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gxhsdbubx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gyxebbyjv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/ghhmiryoa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gypueieok.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gayxaulzq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gkzyuqjhn.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gpdwtiqpz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gtqyzehia.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gsgdwudjw.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gqhtkbjjw.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gqxphgiis.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/goftvlocx.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gcnqusjdn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gkjvjbtgn.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gwrvmdrcu.sHtML


<!-- 参考信息 -->