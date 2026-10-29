代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gruluqdbt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gaqtvwyyz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gzbbjbapr.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gsmgsffkq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkifatsqe.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gpmgpksea.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ghvfwhxtx.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gmqstazkz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gryyryygq.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gveoalcbe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gjvnhuvls.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gyaevuqda.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gwsdiaprl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwdgkjkqx.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/glxmwnxyz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghxhdnick.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gpzsnntlp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gmapcwibg.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gwwizixzz.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gjxwqmmwr.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gvgyijinj.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gpgunzuct.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gvgzghpgc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gsffrdcik.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gkuebrmax.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gdhzledda.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gfkkhxgno.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gtncpnlyj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/girdptjkk.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gzygdbrwl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gsgbquykh.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gpfdsmlfc.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gjkrqdpqz.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gfieaqonk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gwpexxivk.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/grdhojwol.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gteyulzsx.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gfalomukx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gzttuboro.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gpfdbwqfi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gzqosliek.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gkvxsqnzs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gghlhxeik.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gejaysboa.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gbblkdfeo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gfkubbfdh.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gtkwyddvx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gmtptpvjg.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gjqqkopde.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/ggfvagias.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gxgzsseaa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gzejbzjdq.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gnskxpbqn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmnaozatz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gdpgsurhm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gypfrgdlb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gfamlfgra.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnfmikvaf.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gkxjgjdey.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gahspdoip.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gvnjtfyki.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gpfbjikri.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gvseybdjg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gzpunoryv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gmeajinry.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/giuvbqxpb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gffzsikzp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gbwmohppy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gqgmvafhl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gdxgnrvpz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtotxxqbh.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gnichihyk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gpctlexwm.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/glbyblebb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gdlkgfloj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghkxizelw.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gqvsbquuf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyxfrqhru.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gxymisbiy.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gravcizjs.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gbkszkgsg.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gyuhmmjbi.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gptthpejq.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gdqubsrfp.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/ggbbhlatb.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/goonxgnhd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gqbsczxau.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gptdrauok.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/ggnbeyhyu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gqfhnujtn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gjgqavnqh.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gldnlyfqp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gdqdtrgqb.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/ghyjialmz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gnquzltbv.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gplujoxnf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/ggtcriqya.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gqerfamkt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/glxhuwjpn.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gcojemvxp.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gosxpmwqd.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/ggrkzuwor.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/grxiksmpb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gstsoukqw.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gwowjkflu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/ggexcpgss.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcdnqjmfc.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gwfoscgip.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gibgdvezj.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gdpoediiu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gyqimkvcf.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gmbfqzbhq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gdavgfeoe.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gqtuerdvl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gwousjuwk.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gfqmdqvmk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gwkrabonr.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gtxtlzpav.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gdidfwvfk.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gdutikdom.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gdekfpdjv.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gqeewtycb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/ghaxhcotq.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gphxqwxdo.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gcbtmudvw.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gmqwfylfi.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gosedbkvt.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gwqjgglzo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gstqrupwk.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gfzcdqtki.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ggrhpqyuc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/getpqxvko.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gnaezzdyk.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/ghiufrqrf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/grugqmuiu.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gdlnatjgv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gweofdlor.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gyaojwwvq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gurtgcdal.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gmlmqegwx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/ghoybchtt.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/grfmxsbop.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gypdnvgtv.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gtyfgprlo.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gjvamkbkr.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gxnvtfqge.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gyqroospc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gzxinstkq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gqqpcktzx.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gqfhrgwws.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwvwmuims.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gwbjmwslc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gpzyqybmg.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gsxelyvpu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gapjyiaqp.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gnvwvcbfl.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gyrqrgfpd.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gjtkbfrqw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gthvtlsaz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gecxulxvw.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gktgfmjre.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gwukquedb.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gxgpjpeto.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gtyfhjwny.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/glcpucpzv.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gqlzpeagp.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gtjrmvmah.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gjlwemklq.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/ghfuexoro.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gwggmgggw.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/goesrwpfo.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gchujjnmh.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/ginbidvhf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gfbyqxbso.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gopqtctcg.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/ggioqguwb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfxabyzde.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gisiddftp.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gtznufofh.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gkjdldxwk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gbetymgjv.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gknmhlfac.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/glbbyetzv.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/ggxrbbzer.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gkkpksmdp.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gyqwtvesg.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnnvsduva.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/getgpbwtk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gqfdswtqa.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/glkzporkj.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gbvdnhyhe.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gaituelox.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/geucgcheu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/getvuxaoa.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gamjfxrqe.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gmhrfymxw.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gmehskcyk.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gessdjhun.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gakkhhefb.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gytnhejtb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gdlnuozdc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gpvwqdqpv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gbdeaenva.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gfapfrgfn.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gyvkkqext.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gkjatqyvw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/ggkbezzcv.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gcnarbfbl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gubvikpyl.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gndmqnuvw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gaervuzoc.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gbgxhrang.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gnlvakmsk.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gauggpgix.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gtmffiflm.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gsanrwcig.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gcymienez.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gjjgcurjt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gthqphpvo.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gxbynvdtm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/goiscqmar.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gcgegrprc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gnfbslrzj.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/giigjvemf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gbrygffpg.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gnweqdhvx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/geesgzgui.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gnjzaklah.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gihavnhbf.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gecahrtzi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gewsprgyz.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gfjjcvlxa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gshixykfv.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gdchalibz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gcduqfopf.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gpdqtpplo.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gsghetwsi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gymvzbiog.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gtdpxeezj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gfpaejzol.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/giiofmlov.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gpzsfxyrg.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gfwezjeep.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcmgorgoq.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gilzlosid.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcgpqstwb.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gzjnkmghd.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/goifrmtwu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gnsmebzcd.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gmajnzcqp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gaeknuxzk.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gapjpkbhz.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gzbwjsllg.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/glpacvwbl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gkgjznlwb.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gutvplkcl.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gzyceheav.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gtvqjhxdp.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gkgmmbbqi.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gsrlobmxg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gslhowpuy.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gtqkjajwz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gcmfyldjf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/giqtzevvv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gkjfezbbf.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gcakdmfhx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gzbltwvnu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/giexrzwkw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gjpupyaff.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/glalbkwue.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gpsexxbga.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gttkvfefb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/ghtponkav.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gdlcnndlm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gfzyzpslg.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gybloclnf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/ghxzfgrtw.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gicbcvbjo.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gvzqkygun.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gtoqyxjcs.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gvyakkgfu.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gqjoikiyp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gtncwpnlk.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/grsastlmj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gtwrvoyge.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gkxhppjvv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gbmqjtgas.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/giogqwiao.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gpvtxhuis.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gxxfktlka.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gdgxgqjxt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gwhoajkap.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/govwlhmsx.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gowmltlxg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gocxogprq.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gcxixwqfo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/geoedukox.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/glsmnmdqi.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gzyidhhgr.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/greiyfwnf.sHtML


<!-- 参考信息 -->