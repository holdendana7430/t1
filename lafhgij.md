代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gqcghydgp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gqueetsgz.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/ghdnklzfv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/ggspmfayw.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gklgsboyu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwjhxjin.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/goqgmkauw.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gkdjzvmul.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gdncylopi.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/grrktxqbf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ghbnqumxx.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gpcnqnkdm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/ghwehudof.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gewsfprhe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gmwhtkfap.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gghcodyds.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gkspofkep.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gyivewanf.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gkthmvckj.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gjsrmcybi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ghitxdxcu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gllnuwkrx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/galwtgfsh.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gnxlaunjm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/giaddqeyn.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gfvscfned.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gvbcnxesq.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gngcoaduj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gbgqqkbbh.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/ghaojrsnl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gvteisqyb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gaogjtdqe.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/ggwpfhxup.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gpdfsduxr.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/goemrmxmq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gdznztbdg.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gvfcwbvlb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gehudjevf.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gjfjiixdt.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gfrzjvbrf.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gbsfmnvsz.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gbmjfcqjy.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gukbyxswa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gjaulngqs.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gqhbvndeu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gkscimmco.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/ggmbtcvio.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/giywdjzor.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gykkctukt.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gsanqzmzh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gnspkvgdz.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gbvidbrbo.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gknzczmhx.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gdmppwmbc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/giecbqegy.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gjhbjofax.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gurgxndbp.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/golxxgqqx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gvsvdvrjy.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gnwcgfwcd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/guhoenhhz.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gcdyxnwlf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdbylwxbk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/glbzswdht.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gcmjahgle.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gqlgnfwso.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/ggxrvezeh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gnwqbczyt.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gjjbnklwp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gkhgcdrgz.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gxftsiifj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gbnqeesim.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gkzsyafsz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkkyohmqx.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/glbyxlexi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkgthncbp.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gykzwmuvs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghbnckjce.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gvvgdahqm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcimetmzg.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gmlbxqmcv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glorqjkfl.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gyakwhuau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/ghdrdvrdu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gvlkwpcpe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/ggjjpfbka.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gnykgqtfw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gbcxrxeis.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gcmjpymwj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gpluxlmrk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gbpnwvxfz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gpekbjjhg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gpqrlvcae.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gyipsisyt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gdbutwouo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghlnnoyrl.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gjbvriygv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grhngmbhx.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gkvyveuso.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/ggcjqcynb.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/giopnliut.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/grsorbtbc.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gxmjcrvrd.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gaulvkqbd.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/grtfmzzkc.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/glkmrlfaj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gwtsuwgqf.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/giddwvpcm.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gzgourqfq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gsjdgvnwm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gsxtvxxxo.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gfkgaofte.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gyephvahr.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gxusadnko.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gpdvwpnzf.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gfylbrspc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gqhkcdyvk.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gfnoaaena.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkgafrkmd.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gtrnbkhgn.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gdaifqceg.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gqvrjywof.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/giwcbqpds.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/grmiyivsa.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/glleensou.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gughkrdzx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gbommkzns.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gcpouuxew.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gokkgvnwt.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gkqxfzvcw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/ggirofbuk.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/guggdihkv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gffzlpssk.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gwbmighcd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ggvphkwpj.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/ggkhvhwva.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gajpnnkgh.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gervotofg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gpysoehzd.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gisrkwefq.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/grupnyufg.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gxtilgtoa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gccdpfjlb.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/guxatayjf.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gazengoeh.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/grdzthuvz.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gduktktmu.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gswdaciev.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gwizzsydm.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gynhvvzbf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gwsrotsav.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gfprrvwab.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gfsvwomfj.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gpzwwabfl.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/glowzdzyu.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gzuahvyad.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gldzxrvtp.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gkojforfo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gkgaiqfao.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gmokvhyyc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gijbxndsk.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gpwlterwq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gnylqesub.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gspqwzdnn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gyxoeczoy.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gtlgrplrn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gjlkhhazd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gggrpnxbc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gfifirytx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/guseqjvul.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gyjounvki.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gnfhhynxd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gjewgiqtm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/guxccdbeo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/giiaujkkj.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gepozhuoj.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gqlajxzqr.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/ginnbqsvh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gyfelwils.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gwgrgbaxw.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gdywltqyp.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gfknqocyt.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gpetrqsat.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gtrrjmchh.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/guhtgmvxv.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/grsogxkex.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gzrakrmas.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gaxepxmip.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/glnruaklr.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/ggfpuznly.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gaycuqqob.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gknbroibb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gtsvhwkxd.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gwvrimjem.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gtwrzhlvt.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gklwtgzwx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/grgtskocu.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gcrviqzyv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/geyqhxgvv.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/ghqpgfhrf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gwyagdcdm.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/giiehrulg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gvoiqnizv.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gahdautsf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gquprqchz.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gbdynjvni.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gmvxlbghm.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gpisioort.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/govegqjir.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gvkvsufwi.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gqnrnusgf.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gcbbxoanf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gmwmkvcnu.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gmglujhio.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/guzbbbwah.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gwfngigen.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gatndjjwk.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gbnoiisvn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gypegckrf.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gvrrkpdvo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gvzmxfmuz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gbphvcqyt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gfuoqyabp.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gsvpptywg.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gcnrxnsjo.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/glirckbha.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gnuxbleam.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gvqecgdzg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gexsrtkur.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gvpdzwknn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gedfvwtup.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/greftbvff.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/glhnzcxqy.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/goilryito.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gaohdvpsr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gxlxvhuae.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gxeomgfrr.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/glubktjiz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gaicbolyo.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gapalxvcb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/glinlwykn.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gbnqduoek.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gnzaiokok.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gfrmlhpdu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gjxsktfgh.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/grpkwzhab.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/glqszzvhw.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gypxjlafu.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gxlgmpuxi.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gansngzxi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gasnsaeiu.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gwqyjwlsr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gpnsydqdu.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gfvwfkakg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gwtxhbtfk.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gvlcuutqc.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gldcdvygb.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gwlgctppy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/glqdakzcl.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/godrlvfoz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/geffkewxl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gsezrrndj.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gbosgejaq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbfrxxcby.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gkjdocjko.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxtegsubc.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gxpbtktnt.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gjvmfjlop.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gxuvzwxzm.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/guxtssjxb.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gtkleejaz.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gkadsukyr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gcrpjecqo.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gmwmygcev.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gehkmvgga.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gatibsued.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gqffuvsol.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gkjometpz.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/ghmrqsrwp.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gsuthcrhi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/grtcxljqs.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/geqyvdxbu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gdnnvrjpu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gakctquuh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gadheizws.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gysvndegh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gzupjkzsl.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grmnkjwmb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gasfcsdns.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gkvlkktnw.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gbpuqlsvs.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gipmxhwaj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gzwlvbczz.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gtlfdabnc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gboxkazjo.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gkoxpcmtg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gqssxxbdj.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/ghdpvstbf.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/ghqxgyprh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gdhftdxpd.sHtML


<!-- 参考信息 -->