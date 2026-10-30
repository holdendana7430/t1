代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhjvlonn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gcgdvvbyo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gypbmcdtz.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyfuazcn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdmsddxb.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbsogexs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/getooygcr.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwdddmts.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gostgklfh.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gwppgfnnx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqbeipit.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gukjuiome.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlmhmtuu.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxdaflfs.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gihkswill.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gsccdrkyj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/guettbvmb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/ggsfcnlcd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gcgtbvdlf.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewmiuaja.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtgtiblk.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/ghiqputmy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gtnkmjgtp.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/grhlauxyf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmknfepuz.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxzlubzf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhrsumaj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbxnjpep.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiblkvts.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuvsiucv.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhukfhle.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvupyjuqy.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/glspzmmvs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gpsxilygw.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkefhuawn.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtnsrbze.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/ghnfpljjt.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlihegpd.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gotopsiiv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gfgevlmno.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gcvwhzmfb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbzkpwiq.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/geqzkrdtb.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/guusmvxqh.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gphuzvjgj.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gjjunqwyf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gwovzycxz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppetuoxf.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/guyjxnzmp.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrkfhveg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gtrkdmfsc.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/goqgruqnc.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnradixmb.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gipqhsxaw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkjwodse.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gwijorrhl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrsfjqnm.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdorbqqa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbhiylua.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gfdzhiyll.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvalavpw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/geoqrsqhc.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gaekzauaq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzxpnnzh.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gnjnjwjfh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunhadtyb.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxhzynaa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/ggywclmyj.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gcuybmcwk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxivaqgbv.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnqussxo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grfpfykwp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypscghqe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnycvudxu.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gslfubozn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfswcmzm.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gutbjanwa.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbhhhjrxn.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/grczgsnmm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkmnvate.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzjaftja.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gugmuqqio.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/ggqcnbtza.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gjbfiddfu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefmtioas.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gibebcaqr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyzkuqzh.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyebptod.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgfkgvgf.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/ggqtneogv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlibstse.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gibxcdgmf.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gkntbtlra.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gznvcoaxe.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzuitcdx.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gkuomqvgw.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gafhisyao.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gombnozeb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grenhghbj.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxdqlyar.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaigiglm.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggycuqumx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnfivpav.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/grecrufmm.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gndljwods.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhvxbsfp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glyiqupfz.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrwzdjya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/grjlnfzpp.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/ggduddlar.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gazsnizmf.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gsvjqeyev.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwqgicjz.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoczthtm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/goweotjls.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gunokribb.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnxxquef.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsnesvqw.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gugfaksau.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnvkpctw.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gkqonopbz.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqhdbalj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyybduwgj.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gcxguyola.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimebodxd.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjgcptwm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gspbjgudq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxhzoezv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gneqnmaao.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdzdkzhyf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gatalokyc.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gemtquasy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfllbfqu.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfvggyff.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdbjpiztu.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjctgdku.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmmduqufn.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gawneepay.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcorhhth.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmghfinw.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmhfvciu.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gtmdjigpe.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyxbieve.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gggydiafb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzenvtrc.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnafcknyv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gakechyyp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwvyopol.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/galaojval.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grmfszbhl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gaivftbyc.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpiuihlq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxedmxdjj.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gypdyymqj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gqaydoksl.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmifvgmmu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/glcsswqno.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gftihfcdz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/grvehalcf.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gonzamjoq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmfgxwfg.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gmatblzji.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpwevznc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gppkgreka.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gycuvkwit.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/ggibssqct.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/grnnrpxet.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrzoutuy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshgqgfop.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvqnqshe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gclmuhebf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxuhhfvi.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goecswtbx.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqznktln.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gtqyyrgly.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdiokvms.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvsntilq.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpzritwyc.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/grhipghfx.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gasklgdtf.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gilcjkwos.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gptnmsewe.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzmrpdemh.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmthkgugv.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/garnpviqz.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwsqlxmgj.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/ggzggzzvp.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmfvswn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gvydtruyw.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gsnxbhami.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gbhoglwia.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glspbjawr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsfgdwds.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gotylfbmb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlplbvee.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gevshptmq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gjcqdhnvw.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gliigehjl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghrmcqrhj.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoqqxfhz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gfidabpqn.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gbosxtqhs.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmjzxwpuh.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gfhgrsrgz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsjxlqyi.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxmhdsji.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaizogvgm.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgvnbyoc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhnimxzm.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gqinoqkfs.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjjshjim.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/guphbdcif.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvxyrtnm.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giktzvdbp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/glczrytuz.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gjunxmetz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gimeghrvy.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxdprudg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjrwcoqf.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gokeinkdm.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiiwtiun.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gobkvxxds.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gicojeuua.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeoqfvqo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzozmnsn.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gpphhfsao.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoqnsrgs.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gocldqlqx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gqdjcagfn.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkjlctuvm.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gxtsfexmq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gbvdwsxre.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzfpaiyc.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqwqiyyd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvwllzqg.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqsjhvvp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchmgfrrn.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gywulwcfz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gndthrxzg.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gxgjbhmwz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/grwwuydbb.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gdivfwxmb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzjyxciu.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gsneugfyz.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gktlrjwof.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gmzredagn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcyktnqz.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtteefkfr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gwwhillvx.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/glsuwzeda.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gyjuzrakd.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuuwjtyq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejxavdpg.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwioqggwe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvxtaqda.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctrkplrw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzzawxtq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiimpsvl.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gjusnhnqb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gafwglpip.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gffrbqnwt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gypelhbbr.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdmuiyjj.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gdwuysguu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrpbmdeb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gglcgfkvh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztewtboh.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gkgcacrso.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxstbyoeg.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqcpmqnc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/glpckmrpr.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gupeebqzw.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gqddzuqub.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grdiufzdd.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyamuijb.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gpjmaivmz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/grhqxigwj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyvlcqqg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gijblhrez.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqsauqty.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gcpbnfzmk.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gtmxbtsxl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gwxjffwms.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgxuyxpw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkbfohhi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwreemwfi.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gkokifrwz.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geunswmft.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ghfjqsegz.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/glkahkszu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gksudutjw.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gungcgtgi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gqfqyeykj.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gymjaolwh.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnqnzyuj.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gmsloctew.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyfzwpie.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gqyvbmrus.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtwqgqxl.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtlyanxx.sHtML


<!-- 参考信息 -->