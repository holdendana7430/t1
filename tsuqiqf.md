代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govlplnbe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gmrocuofg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdivmvrqa.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfhusbiw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gknyidpwj.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhdbmmnj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmemzxzqd.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzmikelt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzieuuwu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkdpmtot.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gecfazyai.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghptirhph.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvufecqxr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gknjioxgc.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gmxqbkdkf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gvqhuehqq.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/giprxlvad.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/giuuktgqu.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqoxwrca.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicyqblfg.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gufgjjcgb.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/ggucunybc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczpsqosh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gitnfxkid.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gdbaqldhf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gxsmzxqqm.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gocynxzqb.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycftmnoi.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdhyabgs.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gttlfjulp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwdzcbcd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngxfupva.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfsjqoev.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gllrhbecu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdtfysup.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gizkrranc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfgnltec.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/grgmiazfn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyhgiyay.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gzirpaguz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gnourdcty.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gtzyzqvgj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdgtlkbf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggufhavrd.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gsymkjxgy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwquzqyic.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlblmbuy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyqanxrj.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqrorerx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gbpnaaysp.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gknvszpjw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjbamtys.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gdfwyhanv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjkgoarml.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gyecehpjw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdelbzmy.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghoflofof.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guuutnawe.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuohefts.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggtuolxyc.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gthethdug.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggawrztpd.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gzygfgzeo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gugyfsinp.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gegikmqzm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfqtmvxf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyfsrzpsb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gtwfimdjo.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gfmhcxzwh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhodeqfj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaepxqgr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihpmgdoy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmacugzhq.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/giekbueho.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gnevvlueb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjizjqnlz.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/giozwjydo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/groradrpz.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gqltttfke.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhdfbli.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gydumutif.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdpwzpgg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqccqpjbg.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/ganqikoyz.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqqirztp.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkldogtj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghscmjfyw.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gfultwesd.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkxcssbf.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmgdkkyb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyjryiqbv.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gobpasfkp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gdusnmqff.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaescpos.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghskswupw.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqlvatlxo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/grmdkeihi.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ggfjzpkax.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjcbqlbi.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gnehrmmtx.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gqsyztevy.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnprjwxk.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtlmwmjet.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtiognlv.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gzchjokve.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gggirjbnq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/goqvmoimf.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gyatikkpq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgwkstvv.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkjchprb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjnoaeid.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdjbgcdua.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvcsyubc.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/geftyhltx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geesffavx.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggekhdxuo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gioxnvzmy.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gspigldai.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtqzrgauk.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmojwsbe.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzqzssnhl.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gyumgvweg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gacjfjjws.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwosalrx.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcsigwxqg.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhkxxzcy.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnzpgbnib.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvrlwmsh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxuqsqnx.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuqexvid.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmrlizbxz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gbvejktmi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdjfuyyf.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvowtnwgw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gbktmrkmt.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyceukbp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgfqrvwn.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebvifner.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrgygcko.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gseerckes.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzmxtrsyr.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfijkffq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouhjknlc.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grmyakvbs.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsmdttvn.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/grcifosmx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaxelbqew.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gfaetydyc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqgsvatc.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/guwrnbixn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gsjkduvtq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcafesfa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gggpiuikn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnluzmfl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gajhlhtah.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvilrtxw.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpotruobi.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gdteciztz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gjuisfuun.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gosoljpov.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ghnynuypl.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfbdhebl.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbpszyjk.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpupfchyl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ggkerwdkf.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gshinjiuq.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghegyartr.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdamyjsuf.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqllpoydo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglybaeos.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxejfzhvu.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrykajop.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieowrtwu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzmsjvtv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gfyihwjtq.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvadbtpaw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjquufmx.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/givodkfoq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxhmdwrz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gukdnsfrc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnzkvmrv.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxnxivry.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzbmhioc.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gbvmwlnht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsccfbplc.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gxhbqpsoi.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxysmlyt.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/givfyubks.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gxxkzfwjq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwevtqfgi.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/goukkzqby.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhqrdnsc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/giyhdowdv.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gkwgabpku.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gwjgggkef.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbdlzicw.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gnaxivzdj.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgchapsu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoiigzfg.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzywphgd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/grnirzqbq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyeawkan.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbtaoqkl.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqcqkshn.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gycflbuxo.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgjbznoz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gphfhcwts.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxonifrl.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gyouutscj.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgftageh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvhiaczu.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfzstina.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaigcpjt.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gunerlnat.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkpbsnqh.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gguyukkrj.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gdwajhgpq.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gsakamzuv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtfclkufh.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqizafdog.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrybzoqw.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsfvveja.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gxgwjwbht.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/grlydeswg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gwdjfcngf.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqiaomkf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqqrwhps.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjnyqyzn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkggboiz.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gvmobnknv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyyytvkd.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcblwpqvb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gaimsmzwg.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwbiznuul.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gpraevlpp.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gqwzsdonb.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjyplhza.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjggbtsm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxtvlrmh.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdrpzsmb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggzfcpbsh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gawzgcjnq.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gagvjzgiy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfzjfqcl.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gzuwotsdr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqsufpypf.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gryxfazto.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwlgkdma.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrtketsy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqugkewt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtumvlllu.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gmkcwmzue.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gcvixkdee.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmsqdnip.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcbbneib.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzaurfsxr.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfffjjgbt.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehkaimiq.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gucbjgdqu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglonsdto.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwylszrz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gfwcelmha.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/ghqumgfmw.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsxghpro.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gzbdbkyue.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/geeinaism.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnxoqiks.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjdpwnxau.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gulzgdrkf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcajmjkr.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdzlosteb.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkizddtmg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gsqjtqtul.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gvfeskorj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohndqfjm.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glwchuwbr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gakugxfzo.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/grwdbnmyg.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gohtegmmz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpisdwds.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnzuhscdc.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/grvexgbzv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxgceszx.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/grebeqiur.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ggblwiyzo.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gowxhnewx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjshmpdc.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gpirqgecv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmpjqqpf.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/glmwkphyi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gjqyierio.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gsaszrcql.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/ghkvqhdsb.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gaqkwkpvk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzznryha.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/goerpbukm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grircojgj.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvzgefzd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhkqyaak.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gaphbfece.sHtML


<!-- 参考信息 -->