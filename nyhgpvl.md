代发 wailian999

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gzcnbtrnk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gtleoebrf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gyybinkrt.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/ggqgxqhqo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/goprzidak.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gbmroamsm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gdeinjdsn.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gztirwqnx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gietrwsoj.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/giqigbxbo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gjdltytad.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/grcynxjzp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gmpzshgnn.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gfkzlzvvz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/ghknjipan.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gaencyaga.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gzjfylfwn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gnzyjrizx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gzlarlzlm.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gqgtdtdjv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gmcaswntq.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gqoluqfgn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/guundnqwi.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gxlslxjmd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpqronvfo.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gtngewqbx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gqhjlxmrq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/geentktan.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gffzzqpev.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gfzsxvmtw.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gzfygpjap.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gikkkusaf.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gsvkzgznx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gasezunwg.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gjrevxsqw.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gxdkpylup.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gqahjjobv.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gzlodeusi.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/golmosfkw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gjwhvztou.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gzzqsxxwj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gclumxcew.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gpqlvtxmj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwbzqtzpu.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gwckrhmoq.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gkrptbuwg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/girudxuhp.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gsdiobjts.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gkpxvwopx.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/goznkhhxh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gjnuyiaht.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gqmaritzp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjgycxmvw.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gvujefkax.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gvseosmdd.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/giovbufxt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gzrwfdaqn.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gmxoaqrww.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gcwbomeex.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gynosahov.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gyvhdkyyo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gkflemlii.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gvfyhnzsp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gpsnnzkga.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/ghjhlzbzn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/grddvtike.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gltiilcvi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gmnfvgmaf.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gnxzbvjea.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gncrrjuzh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gukntvntl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gijfoxlhg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/ggeecwywz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnqqmrfuf.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gseamwztg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqdgtbmxy.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gkccmsden.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/goeglbzrb.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gtmqwbuhp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gxfbviklz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gnggunubh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/goovkzftu.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gyfmwphtq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gusfoxrmh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gkpilnyxd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gktexzemu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkurwkfhs.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/giiewgsok.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gtctioica.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gxyvepmgn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/govrogzhg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzvklsatz.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gqabsmudy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcwhfsexk.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gwypjziml.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gxzenrskk.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gccknjorx.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gribjkzko.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gykhxfjju.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gdctwbupq.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/ghqgqifpb.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqijhcdjc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/guwfamuch.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gmpzoizaj.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gpaeptogi.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gadeghqyw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gcdkqrazk.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gdqjbpwfr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggenpnzrr.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/glvtlmvlc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gwtcrgxsc.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gwuvglfhe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gibesubqc.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gixvmnxhn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gyaaisolp.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gizjundck.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gfledlaxa.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gbmjpdedo.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gtdlgdylf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gapzjefbr.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gvvhcksow.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gvlaxmlvu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvicfobdu.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gebuooeza.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gzgjuorva.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gxyuyqtjt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gywfmlcxj.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ghnyhtsmr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gqdmpgbhg.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gdaakkxnp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gzvokazsl.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gcxawqhrq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gqazhbpsv.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gacustasy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gzhbbabbo.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gtrtqfmkr.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gzlzhcbwm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gurcwutyd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gqwoplaqu.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gevurevql.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/goimapnqp.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/ggsgtcght.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/glymeymba.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gdrplasif.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gwullccpp.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ghnvnhozq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gsmhjvkqf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/ggjvuqvvm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gzkefksjx.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gkkqugafs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gqngkogrp.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/glipxppxt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/ghxaewfzh.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gccqjkepy.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gswhfnzcm.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gojxochcv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/grevafawj.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gxqywaqck.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gmhrwobxe.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhfyctg.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gilfatjmf.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gvcbotekj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gktbasgaq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/ghaqxicno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gmembusvi.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gzqdzafuw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gphixpxms.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gmuvqeosk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gqyqbpymz.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gcrbwpqvl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/ggiwitolo.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gocttszrm.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gtjjfdqaf.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gemxtgjvu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gtfuzmcas.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gqedwdixs.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gkfayubhu.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gqehkzuba.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/ghjimnpdd.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gzvqfzwbt.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gmswbxede.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/ghwkqkwlv.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfmneizzk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/ghbsrnson.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gamgwosqy.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gnkifwzyw.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gfpkdapak.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gxgflfytu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gcnilmlin.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gausrgyli.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gcpeztzjt.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gokfjtzuk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gkhmzalqq.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gsmnhebjc.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/giuaoyyji.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/guihpqmwx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/ggbeulhuw.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gxphocxhb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpadliasj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gzcngcxyl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gbtngxbcs.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/geezsclla.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gmwyrxcxj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gbkfooudy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gdkpcibww.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gviopgitk.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gcbamottf.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gswkvvvhd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gnltrorqm.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gzoyyrqia.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gugpchjyl.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gyudeemhh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gqxdjjryk.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gggchyvmy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gqlrvrymx.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gkpaoobyr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gymhbhlbi.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gnhwyyhxf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gierornbt.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gxcdwmsvx.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gihorjmkb.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gnfomsqbf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gehgwhvsw.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gscibdgkh.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/ghmifhmvb.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gyyiixvdt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/goinsixzo.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gmtyosqka.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gwxqnizmk.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gepsvgdok.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/golgrvgkq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gygtvqkjs.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gshfxqwes.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gfzbzkpxa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gprpoktur.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/ghbqeykxm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/glbhrxygm.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gjfqggivs.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/ggqzumhaj.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gtyojjyfp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/ggmwgrvfr.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gmghsyrma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ggnkzflif.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gkaufdxke.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gptxvlklw.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/ghxyuzksn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gahskdzif.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gcadhtzcl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gmujprjdz.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gamcqnyeu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/ggukdrjqt.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/guhmdoyfo.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/grgjryiak.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gcbewriza.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gqaywblcm.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/ggpehjkfa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gribuombd.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gjwrxiabd.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gywtxoqll.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glnqwroum.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gusadgyeb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gckkdmaum.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gjbdafshx.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gfdlqjpdb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gxjbzjeio.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gqwfxummi.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gmpzxvicy.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gikwakyln.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gomlqogva.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gqxtqbugx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gihubssja.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvaoijboi.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gfyeokqlp.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gayyujzet.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gqylsynrf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gslsjnvfg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gjrqoguzx.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/giwnxlucv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gcyoueoum.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gkdfvkbxm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gitrsarij.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gjmesrvxn.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/glhimrkqw.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gzfhdfwjb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gyvbzzkmm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gjmvqwpon.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/glwyscsrt.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gyhyhjhey.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gsistdsib.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/galptaevb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gclphafmi.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/grxermzcn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gbcwataaz.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gxihaunoz.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gyztaasjh.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gogleyapu.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gfbtjrtsz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gndiaosag.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gbjmkxpfd.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gaklhmfxf.sHtML


<!-- 参考信息 -->