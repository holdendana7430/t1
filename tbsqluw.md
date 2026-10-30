代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeijbuwd.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gwrpyyphw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gldwrztgq.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gudbdzqrr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gueiomvdd.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gwvmwhbwr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyncvbop.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gxywuzqvy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwppovhi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbjyhfcn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhskxdqi.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyinfbgtg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmheesxwe.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/ggryguaqx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gunelikmz.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gjzhkqdio.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyjzgwbo.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlwcbbkb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvcjbrkb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gatzqcqfv.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboyrnsqf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkhviloj.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gpglguxek.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbvjyuxy.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gkusbadxc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/glzutbulr.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemandbzm.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gteoadxgt.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gduqxbxeo.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gqcykvbod.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gsmgprlxv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqydkefsv.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gkdgfixxl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdylsjcl.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gnikgilra.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbhqtlug.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqyzefam.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdbyauwg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmvvfjju.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweevuabh.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glzpcumpr.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelzmbdqr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gywuuxmvh.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmnepvuj.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzbndvgxu.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gscbjwizg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqluzdojs.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gycerafzf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gijadyiow.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyhqjzkq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibbrltir.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/glbgmczdb.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrxcmyql.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gmxiygghb.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/geopbuzsu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gphlznxaq.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gkwyapqlt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gmylvjxvq.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/guyfiwoqf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxaupxov.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gwvykmmoa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqmoznzu.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaitglejh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnxdlxafy.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdjgyocqt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grsdommoo.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmhewsov.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gofhcqjow.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqmpuhdj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkffpvmz.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbexfkfby.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glynvdqyh.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gxihqwium.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gxfmvyscy.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcyxayofl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvirvdaez.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gmovkiwob.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gbyfqiawa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekovtmir.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gumlnycpl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkljnbraw.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gshlaizmt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gayhxtdnc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrjshybn.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxciwkrnv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grubvuwkr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxcyqrge.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gncqsinbn.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnbaicvp.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqpfjamb.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvxsxqvt.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyvtalgj.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gaufcaypf.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gwdztgpmz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpaceeij.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnobckxh.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnuhshto.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gdszlngcj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdhrospk.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gakqxksik.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gubanwhbc.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtgsxpwf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzbahxni.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gytkxsdph.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gkrdwegan.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gbwulwzga.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gwhdnqhdt.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gudqwioht.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gehmfcawj.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gricwjgxj.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gipnuwasz.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gfnunrerd.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujdpbtrp.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfbhjgcl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gposgkhfe.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzckgjcrr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goktqpbvu.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gglxmgcwu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtnwhzql.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfuptwvt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gujgkzqxt.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gabnpacbl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtbhnyjlw.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gsojxkqdg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmcofqbu.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gtkjxddhb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqpohzrd.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gujikhwlf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guviyktro.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gdwhhjxkd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwbdpgigt.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxehfbzm.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsisuzjic.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxhyfnic.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyiyncll.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhttvyjx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgnwlzbo.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gqwgcxpqg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gifpuklmg.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gentuoxxs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwgawujg.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvdamwhes.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gdigtsqvc.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqtfwbdg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcwhlnzj.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqpveajh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/glhekmbxk.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/glcetmbtc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsyptwjs.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbjjajwl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/grocromtx.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdwwtymes.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiuwacus.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbfgmgfn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzpfttsyo.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gqjwsvure.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqpeopfi.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gixwawpxt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnnouypi.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/glflwehxp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gnelrmtkh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guctjmyna.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhozctiv.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdszifdwq.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdecvnbr.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gzmcdatix.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjzcszhc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gliauxwys.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gefcfzdal.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkooiadn.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gomaqmota.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwjuywkz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxykxahzd.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gwderrmya.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpqimztpm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfqxufvd.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/geztupanq.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gquwxeebi.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gstkuukcv.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gucvadhez.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhqeeuu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/geiirfayq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfovpvqwd.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnezoivw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqcfktjr.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gtvikrrgv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gawcylwnc.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgwqnjml.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/guohxfwww.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gmahxemsu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwlnrrot.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwmppqiw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmvhcrlg.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gqzxqpuaf.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbfarglwm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfthiuhq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gwxmaxezh.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gktogpfrf.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifyfhlsi.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvqzrbxo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gmviphdsb.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdyurltwl.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbrwppnu.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/grhmhafrj.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gddifkfla.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkwcwsfro.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynvfhkes.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/guzndkcfw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gfevrdshn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/guvxehfvg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gphwgkshz.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcoksxkr.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjrqtbkn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyzbthzh.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/girwlkspa.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgdysujt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqpavywo.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gszryhcxb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gauhnmhnt.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gploeypqj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/glvzkptoh.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtkawege.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gqwfcfvrx.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gazdchnie.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/grlhbrtbo.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/grgqkfknj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupkjyjrq.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxowtrnjw.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkqxsjut.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/grsxaecrp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzycgpgec.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnofdvuhf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdlwqnmk.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgskjptf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjvkumqh.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqapjvwv.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiocjbxf.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gteufbtlr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggovwaeju.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxqzirhwq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gqukzkzwv.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjnvbbsf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gindcdyng.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gppatazmd.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizkzsepo.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbreiiqje.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvimguviy.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gwgudcsok.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqxranock.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzwfntqg.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzlhlvmp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflykhgpn.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcstozioe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gystmoxxl.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghvzinvom.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gykqhevzn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gljzwxzvj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gdjxklhwn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdxqmcrh.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gmgviyegy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemrskhqm.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgrvmvrf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gohqgdmlq.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gsohkhwtk.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gaypudgcz.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gncnglxuv.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/grgxtzbeo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqelykuk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdbsggke.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxmyepnh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gminyhpch.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwprdsfr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkcmzstg.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gebjwwyvn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpbptwea.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcizworyp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrpdjzxr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlmlpmms.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwskzvcu.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grepgdjzq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gasraffsi.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrahdcus.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gxxlfbszw.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxsqqvblw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcdhzwqy.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gnytfmxxj.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gciftzdcy.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlifaakv.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gukofocot.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gizzqoynd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtkqwlrn.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gwueszhvn.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcrkhkje.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/grarosxiw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvatirstb.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gltlvmmzv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gugqoygze.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkudsrobn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxmgiwdq.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoeotjos.sHtML


<!-- 参考信息 -->