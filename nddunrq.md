代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdxzurboj.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdxqfoyxf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvjlwozv.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/grfedmvad.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gzbfkkkaz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gpwhoqakr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuoraruc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvucvqypm.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gwczivptd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqfmzjhnx.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gepfesryx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcapptyw.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjqejcnm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsforfvn.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/grntfxskc.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gexfrepbq.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/ghkvhaxcr.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbqwbjpq.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/ghpntosxx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/giailozlh.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/ghircerwk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdwcvlvi.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnuxnaql.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsacpqohz.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gunqeswed.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gilhjxhdz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gkxmcydql.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhntmehx.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gffulstqb.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gwlrqtslt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggajwxhge.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gihuqxsjl.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdxhclyr.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaslznehb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprroqbpb.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvatbtvfc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gsxcgqsmt.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwqcddmj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gsmdqptpz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkbqvbua.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/ggwvzpyce.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgqtczgt.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gozslqlpg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyqpijxm.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbqzfiyh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhbigvwa.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeggvcoa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gvymdumje.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/grudtjqom.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gepikqsav.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpfeseyjz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/giwhjzebf.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbahdkwpj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gicwtznpd.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgtnhrji.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gycyfzrfa.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golzcwbur.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjmvggop.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gsctzizck.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/ghkywfueb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gnghxynhu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gmarthdal.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoiugaon.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgedgokk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/ggvqnnqyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gutiyhguy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjkhpmta.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gutzvjpoi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gjekmcstj.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafvvqpbe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvfbbjmu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfetfggtz.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gwafopbma.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrxsgbrg.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gudtbwohe.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gbcrggyot.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnjeoyya.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/geyadxkmv.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gkrsdkncr.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqacwatul.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gxgdijjtx.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gwyrzoolm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqbaisyi.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjwmjhka.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmsilrjj.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gxytznugc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnlzhbibx.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxypgouww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdktzuotu.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpffkqrp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gbxbhwrrv.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gngctzopt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gehzhylps.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuqfljre.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gztmkolek.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/glqcrlaqz.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzicjxkm.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gztoxrlmw.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gajprjeoe.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goswcagsy.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcneomric.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfuewjfcl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gilwpojfv.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtfzucpp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsfclfae.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/grjnnopzm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfykybym.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdokdacss.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gynfbdoan.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/giuwgoulx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxhuzwjy.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/goexftffi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdveupgy.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/ganwfluwi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsubcjwdu.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/geluaqhmc.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbxxdenj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdryckvv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqwwhdlrn.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gagrcvccp.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhdtqcru.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/guzgwdwfk.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqqurfos.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajedyugn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnnxmqubk.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfexrelzt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grurdtcsv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazxeusfe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/guezsibsw.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzldefqot.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gexbwpxce.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gfxgvjitj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gfyqwgmpx.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gwcgjfwhm.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gzjoxtcxh.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkubiasxu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gobovzttx.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/grkrvefzx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gbxrzqvoc.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmgkffda.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfuuengbm.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gufqlpmnk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbaqudqg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gncisvstq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gdzcofwra.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/grgcsufee.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjdvhmzd.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gvrcteoug.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gnbrjhlds.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxxnqmdx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gvulbdeum.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gckradvjt.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxjudajb.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/ghxriekae.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxqrjmld.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwrwqlcw.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqykddqti.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimsaeuxt.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmnozcpr.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpkctrpa.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gxrlxxjvn.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpbubdmd.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glajowbpz.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkdyuedk.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gacuztswo.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gluifdgpa.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gvrqjazmq.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gwemgklkr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/grqjuzdjt.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gcurrxmsr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbmkjlxb.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqgtxfezu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdreikffe.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gookjrcud.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glokkyits.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gcrmeotic.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnwumhpm.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpzluohd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjizfnbh.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gwgcsiccb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gcziquotx.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdoukxmm.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpafirlyj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyxdjbag.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoqpekpn.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmecbogq.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goycryphr.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gwekpfefl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrfrctpb.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqvjlgsv.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiishkes.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlvduwbj.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gttuaomgv.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmfdfyvz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/giqlpnmgp.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfqgrdek.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gskxedtqw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjqeuyao.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfcrueiu.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaexsmxi.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/glmhctjbp.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gquympzdw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gmkvpwcyo.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gansadosc.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqzrrcpk.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcervqsqs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gemhtxyia.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncudilfk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktpkwkhk.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/glrxzjlhh.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gcrlxnxkp.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gxnheatvh.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzvxmwkp.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gnantfjmj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgusfhud.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gaisrdzka.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjaotpus.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gcvbahhjb.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrxrhpkw.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcuwikey.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtewyremc.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gryunyzlg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwbjmfmej.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gwiigjoit.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gavveqghl.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gxphnjnks.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrpnyveg.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gljfosciw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gkpocljzr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggevepkmv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/glmvfvpgo.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gsjtftxzn.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjqkcsxn.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gosjnqxbl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnllpkth.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gyhptiijq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseokkqev.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/grasapjab.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyboklqp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyqdgqmp.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/grjfqwxyd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gadnabpko.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guwveuawj.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/glgxlkwsc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxjxrevvk.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnykptcfd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gigqonqsd.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gcezxckjz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goltolvec.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gwlbkvhac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gknafqpzt.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlxhsgul.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grekzbasx.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogxukcuy.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gzssbwxpy.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvxznfxor.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdkxglgh.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gnxueqndv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gaumydzwd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gfoxielzq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjfjgfpg.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzusrgkgm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkhjklll.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gekbspias.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gqewnfugv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpslzvad.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gttucervy.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpissdmdo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdoefwlvz.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gdbntttsy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxzznjnt.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/goszmhncw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqcvycnv.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gewyxzjzp.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqwnvchax.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcieufeqq.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gonvxkcqv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbexgysww.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmweicay.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/ganahitep.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgzszbls.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerynipkz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goukzjrjt.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/ggibztkob.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gcxqwluoj.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhxsoazf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxsugbzs.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gcqgzwvgs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gbmaxegrc.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gembuaroi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkwvutkz.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gdguhfcnx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/glahdqvxd.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ghatjtzbf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshxknodi.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqpyrtxd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghauhbeql.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gesiqygif.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahrgimwt.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/grkuwrzwu.sHtML


<!-- 参考信息 -->