代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/ggvuqrfux.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gjjzfokpj.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gqfubpqgr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gipvfeoos.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gihsqsuhi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gypymtclz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gkoslzuka.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gabtztfxq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gxppdfnbh.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gofiwbxgm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gvgiwfqff.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gjshscfvc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggxbajpol.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gfjxcdjqi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/ghrtbgucm.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gxmehydvi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gzkgksclq.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gqehbwolh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gojhtxjcq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/ghzbtexng.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/grcybvvds.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gxosjrkec.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gjxfcvxwp.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gifacdddd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcslrvsfd.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gaqzjoyxo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvadffuja.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gsriiprbf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ggochcrwo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gqmictint.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/ggrlclsmq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjtejfigl.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gzonzutxe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqkueqeeb.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gorqzlsqv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gtatghwzp.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/grtoemdgo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gvfecxbab.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gursphamz.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gnjttocqh.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/geykubbdl.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gsquoasfo.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/giclnhbag.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gznsaafna.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/ghjdjsmzo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gacbyvpnw.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gaohovfzw.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gldnnxsix.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/grjpyaksi.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/ggszficew.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gkvibcwwm.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gaooiwzdz.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gxzmwxizn.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gviqhfaep.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gwzswjprr.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/guzzjdolh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gndsgmfie.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gxtiqvzeb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gzfljkqzu.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gdnquckdu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gftihxcys.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gglkoaylw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqcujazav.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gazvhglvt.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gifihngxy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/ghdpadgno.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gvvptkhez.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gudjjoeim.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gtesfzcgf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gaajwcuze.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gcosbtief.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gkdmettit.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gvvcsmjao.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/govshymwf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gbritnoxs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpdwfcray.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/ghqvgkeyi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfbcbujfq.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gjbxcfcdk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gskipufxe.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gyfejuhmd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqmmtdour.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gnhmoyoak.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/grtypddsg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gwynpfsut.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gfldzwkry.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gntttmtah.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gzrrcqrhx.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/ghyhfdvus.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/grihkpwmf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjqeaiggw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwwpgfhez.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gsftuoiyr.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gbwxrlmwr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/guastiknu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyuaakuyl.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gpsoycrab.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbbowfulz.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gldxaclmy.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/geaoooutv.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gqdswdjbd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gfbzcigvq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gczbuwuaj.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gqbejqbsf.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gnszamipi.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gaqcyjbgx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gsiiyzrav.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gqsvhjqix.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gsikphdha.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gogppcxbk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gkuiabbqa.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gpfcutjqr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/giwooaguq.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gwlyapsfd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gzimptgav.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ggnjvhtsv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gltlvnhwz.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gstoztkol.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gwfdfsvrz.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gdsiztpmz.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gdzvldixp.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gmdtgpkil.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gktegnlwb.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gpyobbdtt.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gvhgxlkmf.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gukgaetae.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyskitmqt.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/ginrlurup.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/ggiudwmms.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gdztjyzft.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gorlpxzcw.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/guqqvifnl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmwveskpu.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gkqyevlda.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gqqtgxlay.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gvetadbhm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gvjoehntf.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gjjrxyhqo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gplaqwpvv.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gvsmsjagf.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gcnhwhqqu.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/ggckupuyl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gqcabasuf.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/ghgqrpebt.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gsttduyda.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/galvcnoev.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gnxmbljuj.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gyecqontv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gwldjvzlx.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gslmggyfo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/grcqaaszj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gzasqqjtl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gmmqedwdt.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gqllddjbc.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gfdwcxibw.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gogugdnbr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gpxcxghtr.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gtpzlyfcv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gredhkepm.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/ghvhfrkzw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/giwlfibxr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gcztuytvk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gyzmgxkfi.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gvhjpqpwj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gnlbcronf.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/ghzhflhjo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/glgjgicoc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gmzjfhnlj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gjucjdlek.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/ggdjwmqss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gtxfmrxjn.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gdtnlqmog.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gteyzwhfu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gyhztgpic.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gwznxqgso.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/grsopldmt.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gofwpnrwg.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gfuzvmjbl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gnihswcbh.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/giufklvxx.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gyopxizrf.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gvrntqikf.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gspdlhfbg.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/glqdsgmcw.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gvbdnfscu.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gxnjuvnly.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gnzxqunqk.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gqiouczkm.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gfeekkbmt.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gjnyaepry.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/ghwzjcbhm.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gyrmgccqs.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/ggvqdkkts.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gebayrczz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/grvydhdeo.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gfubihuuj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/grjfzqwsd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gzsnamcuo.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gueqsfbyx.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gszkrjjvx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gjnbhuctf.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gkfkbkzns.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gebbfstix.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/ghyqoprhn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gjyfkrzmz.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gziwbiudz.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gsbdgxlql.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gpdcxaafg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gihtfbejj.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gxokjxlez.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/ghygahnfx.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gzoxyozaw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gmawuddnr.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gbtykopgk.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gnnxiwinf.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gxchldstv.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gqnfnzmmg.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gmudlsvuc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/grpumfxbl.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gmalaiukt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gpkhdzsoz.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gflzezijr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gqaqpafls.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gxrpowzuu.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gpszpdlez.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gxlkupuke.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gskkakmld.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gbtqvzgci.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gswrjcrdz.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gfvtmjaxr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gnmfkkzeg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gzploniro.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gdflgjuak.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gtamaydks.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gidqlwpht.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/geneaqasc.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gyfllwblj.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gwwopiejh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghapkuoun.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gmnzouhfb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gojttwjfo.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/glgryydhg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gzvjcclry.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/ghurdxfdt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/glfrfchaa.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gtpgelxcu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gyxdtojyj.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gqryvhsbz.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gbfqiqoed.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gsdpzdeox.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gaikubkcl.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gpfhgqjbd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gdnbhbzrh.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gmwtaisqf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gbxxxfobn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gfjogcydx.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gpuperoap.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gmcqnoxmi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gltbzwwla.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gqtntdfhz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gsvlrsxsb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gdznuoyff.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gijjijsoz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbxoiuhrz.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/govkbvyot.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmgsayiqw.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmkbbapvm.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gvxrrlnzu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gefpxpjjj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/geuezcnbf.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/grcmdrsog.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gdpnkisfc.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/guodqwtmv.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gildflgco.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gzouvrnsy.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gdmfzvykk.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/golfpisvk.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gnopgdouh.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gvkstxnzz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gdaqlklez.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gyhfxgick.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gkkofofxs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gbkjcrigg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/glxefaahz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gyyteesfp.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/geggxoaip.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gccwappfn.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gbscrbtvb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gwzfvbfvg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gacyregrq.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gzrrnrjdh.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/ggkdxawzz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gvirsrwdw.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/grxvxnxow.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gfxlzvnkn.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gqsjxrvgv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gqlypkhsq.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gatfomepk.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gubriqycw.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gaduptxvu.sHtML


<!-- 参考信息 -->