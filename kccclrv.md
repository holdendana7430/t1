代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gvyeawggb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gdbbloxva.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/guhhpmusm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/goznjaskt.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gatxzdvzx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gdkueljqo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gsdgtqykt.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gwqmiisaz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gdyqzqivb.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gwyugeqxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gnembzagi.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gylzpklet.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxcgqgfxk.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gdhzveila.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gceoosntf.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gtaluhbvb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gsyahyboi.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gajgzvvsh.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/ghltgkrtq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gpsqfgciq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gqecpwcng.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gcfmysihh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/guagczxqv.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gdwvofmdz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggwcgbchq.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gjklmufdf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gddbteadq.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gbnvzxvfx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gnfudgpep.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gecdztlzd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gaocgqlwi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gpkdfijiw.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gsrllhrnq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gsvlwtoyq.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/ggsjljjfv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gruuonggv.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gdpmftsls.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/ggvsbzaaf.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gkefkpdcd.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gtyqnkknu.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gzgvgxuvf.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gqhjefygh.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gnuznbvap.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gdxlhbngf.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gheznmyte.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gcejhrkay.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gyxogdznr.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/ggerppmug.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gsfpdevov.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/ghfsilggi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gzoxtqkny.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gjmrzpkde.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gavavikfg.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gydhaomul.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gdesxnqir.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/ghneumbvu.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gafdfgrab.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gtzycbtpv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gzmnikqaj.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gxeutmwcg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gqwrnptsn.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gbyvgmndb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxxhpitbv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gookccgar.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gbobfgiji.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gzoiqcyaf.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/ggzuqnlyq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gsbhlqsie.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gqpbhreny.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/grxhidgfm.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/glydvlbub.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gomwgkzph.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gafzaaejn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdalrkwnd.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gynfrniem.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gsxsrtxrm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gmvrabhvs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkdxdndmp.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gtokoqwij.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gzvvzsfbc.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/grutiezkx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghjqsrnqr.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gddimakrh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gkpmbiyzz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gxkufafik.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gziqgwuul.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gizefogrd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gedhmopfq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gozjhmtax.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gfxvabrtt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsxathmnw.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gunxonyxy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gtogdfvto.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gmfiysegm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gwlcmdaug.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grjkpixox.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gvjemoyjk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gohuulmji.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gixvruipo.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gukolxrtc.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gecjkuhzp.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gcgmsybju.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/grrjqlpby.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gfudzsnlb.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gaxdfnfrd.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gzmkrqcya.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gicbrvcok.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/glaskbdnz.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gzsldvudz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gbgotzlje.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gtwdftioj.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gngcyobai.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwuoucexi.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gnhgcjjze.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gsetcybee.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/ginvfweya.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gbznzrvfl.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gdehcnorh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gfbtequei.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gyrniexgv.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gytmpodtc.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gzfoeocdp.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gqjbgwxas.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gboqxdyqw.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gpybxhtlm.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gdwoftaca.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gjfleapsx.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/guwthlykz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/grbhceonf.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/grutnfryp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/guiabhgnp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gcoijgtlu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gkdmpbsoe.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gegpyhjss.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gvqvssguo.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/glhfyeeoz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gqeyzodij.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gtgmcairv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gihgygpcv.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyvoofino.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/guzsissra.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/ggpozfumd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gibzxpnay.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gdyulecyw.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gurhjvmxh.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gqrbusdwa.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gskgxrcdl.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gvirvcfpp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gbpuboqtn.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gjogfkqsc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gvcxzjqyy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gouivnejx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/ggpgremkw.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/ggryphyvc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gqkelotzj.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gdbjwdzls.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/geyrhluip.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/ghwkxkzus.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gvrkfvmna.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gvhoaxydi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gudlssqja.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gndyzezyv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gtksbmndz.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gnlxmzucv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gdknzlqjw.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gzsrdbeyk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/ggvfzvmbl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gswrzmmrz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gsvrkpaqd.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gyjzeoyhj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/guafpcwln.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gkzwgtkga.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gfiatitpn.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gvouwxjgi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/glkeqyltn.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/grckmpyme.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gxmkkzpix.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/guvumluio.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/glygfwxcx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gewmphuyz.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gkudzlcuk.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gwkmqklzr.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gqpcdrxse.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gvlbkhpmx.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gvssmnnyd.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gmcrbihgm.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/guyovafph.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gicktzvmg.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/ggsjbgiqt.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gysqrwzjf.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gsyzjpzqd.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/guxpryxyc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gxxexxuqg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gsvxglfam.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gjenecbnz.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/glhdfubco.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gctetbabc.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gqsyxpldt.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gxeyrhdvd.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/ggqljcwyo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gfwqeqtok.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gcvvskdsd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gapvovxem.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gjwkxuzdp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gjkaboemv.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gznltamdo.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/ganfeklqj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gkqtohkgk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gqunxhrzt.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gftxgdgij.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/glnrctzqh.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gnrqgtuax.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gheoezboy.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gvwzazyns.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gfrdmjyoi.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gactvxmov.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gwaernile.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gfrsajmeg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gheqphfjl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gswcvksds.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gkxyjciyg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gjdqvfvne.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gblqsnbro.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/ggpdttppa.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gujxhjzdr.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gsrjplurq.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gtzbntdfb.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gnsurjook.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gexhkrijt.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gadqrfvdm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gbpzpxxvw.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/ganlgkgmo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gdexjzqpa.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/glquskwpc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gaawtsbox.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/grmzxkqax.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/govkszdrv.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gfutfoyjw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/grxldtawf.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gydebsohk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gchywzfpu.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gmbfwfiia.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gzedbtbpg.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gjhpykqcc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/ggwmrclhy.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gfaweznrk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/guycjkisw.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gvytfrrnt.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gbjnfcqzx.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gvvhfshcu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/galolltbp.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gyholtxtx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gfdqfvbgl.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gvnjouvli.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gvrufefpo.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/githjbpba.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gltatebfu.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gycdhnuof.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/grhpwddtm.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gyrvlvati.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/ggpakbbhc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gipzjrxau.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/ggdoqddfb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyhuonmye.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gqipkztva.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gddsysdlt.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gjyjrzjcn.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gpaklnwqz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gpejnkfwl.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/glbwqedns.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gthhthtym.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gbxnqhlzk.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gzrbvunkc.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gtxkjkfzm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gnpnaeuiu.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/ggbncewtr.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyzrdrwld.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gkdhwhmib.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/grcjzuifu.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gakybmuzm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gddupqzyx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gnuklvxdt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gnqnbcnbi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gdcivenov.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gdssakjxn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gtmeywvqr.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gdguxdoze.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gtzpqxcda.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gaosnkwhg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/getppsdwg.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gekrtnrlz.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gwvzqfrle.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gxocjisev.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gdyomxjfw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gzzdvkrul.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/ghqsisoty.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gwsokdtdz.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gkrggqqwj.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gkrxhqyui.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gbqoemaqr.sHtML


<!-- 参考信息 -->