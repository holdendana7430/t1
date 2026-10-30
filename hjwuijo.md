代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gsgqmoqih.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gossweblc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfswmnctv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxqjigwb.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gfcxfkchv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gainqysqx.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/grpbmonts.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmglibfs.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/ggqhcaivj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gbooqfhhr.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gnkivcnkf.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gngvclnto.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gajyunwtq.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjzicpce.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnttzjwp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gmxeijvzd.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbyyqvdv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuciphsn.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gajghyfvb.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/grwvaarje.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfieddfkv.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnpbfiom.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gvijrdhed.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdegvshi.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyfimljs.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gltktaldn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gekjjkhep.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavivgvbe.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/geqfqopev.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoemtfns.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gezzfmzwn.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gyjduhrwd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gngsqhfrl.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfcttmta.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/geoyktmfh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwqgrlgj.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gyhtzsdky.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbwgyjyx.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnnzlzmz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxcxummj.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxeyiqhu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnfdnqsd.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gvudjnctd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/ghytjvljr.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvhhfnzm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwrygyhi.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gebuvidkr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiygrcwz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmjfjfmvq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/goypoldfb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigylikwf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvasdbbf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaixpngtk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqwpsnnim.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavvlcxtj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxktxois.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gpppjifia.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbkkgqlm.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwzqptve.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gjyaingbj.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gdiechgmq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gjevvreow.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbeuuognk.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbgezktv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveffvxiy.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkdlhsqh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/glscgqtiq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfewdwfuy.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gpwfmfkhc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnqndsms.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkghftctm.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghomevsth.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhhspcav.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gvlfmfije.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzfmelxo.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwkbczgx.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpyrgoqj.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/geiapzqwy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuoidjce.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gusikhgfu.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdbkrtlqj.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gvlkqonwp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuvwkyvr.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbmxwmbp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrmprqjr.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gryvufweh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gespesfjc.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/grmjqhlst.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gprmzxzxa.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gmkjxqqwx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfbazpxct.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gyylvbien.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gqpbzptpr.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gymnsjfal.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/guwhtyilb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gxzcaoqnb.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gcajeeajc.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/guouaaarv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gethjuhas.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/grylwkgdf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpzadjqtr.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gcardnghf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqeliwgd.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsswyxngs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcxowywz.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gogpvxdim.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbdhlmmq.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkgmzuyg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzshtoxau.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gxbndsniy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjcvnuaas.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpmrnamw.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbzmktfel.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/guimyykwp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfvbdgrn.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtztpnex.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gclffwujv.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevufttow.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcjkmycge.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grfoymzsx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaiaumit.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqllqwatb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gshbqngcu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdveqhmp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giprappjo.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gombnlgyw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gtvactzow.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonpswbsx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/ghidwowqz.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/goaedyrng.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/giqwnyphd.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfudqolyj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gmcbfmykm.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcymmchd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gmfcqgsqi.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaaglrzf.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqqbsie.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxihawio.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxozjmkwf.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgktesey.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpgstrvg.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/goyycqxzt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gtnptetjy.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqtxvuyq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gxqgioniq.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnuyncxj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/grlviduwl.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkchjmmhj.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gblbasrgd.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtxtuxfp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/grgryqtsh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gzeafvyje.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gguqtyatv.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqgupvwl.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrgqdtlm.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gyogsmxkd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gjrofqzfw.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gahrzelmh.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzcwhtyws.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmfrkati.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkvdwjdv.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvetvtuo.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwselsad.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gmicibufz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmpqvccg.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gashgrxvi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwvsgixy.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeilnsuj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gamcvfpph.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/giffnycrf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnwftcje.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/ggqnnvvzc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gsncerfjp.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gpqqtrmnf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/govpljvcc.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnsgfxpy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gjwgrcfjc.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gdjczidft.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdbuaujgq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdtlpntj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gucpjozjw.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzkttxdes.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpifhqkrz.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhrexeox.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gcljbbhko.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gubewvxpt.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gintghnjv.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/giqmukvpi.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gwxeajnyu.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehtnevir.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/giejoktcl.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gopmbtcqt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/glskzvymh.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtrcoawbh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gulqylvys.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcapacbn.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsgwtmja.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grxlabczq.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gioplmlpf.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gejkevvtx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/ggycifgsn.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gpqkoaimq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyhbakgq.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gimmxomgw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/giwseaedh.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxsehxqr.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjxorbcc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/grrlnarnp.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/guhezroce.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gewinexap.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gybcfarjz.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gijhyqkzh.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/ggvrqakyd.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gmvcatcyo.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfnsmkrj.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gghpwvsgz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqpsozlj.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/goshormes.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvduqnzqh.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gymgkznst.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidsidqkt.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkgeljsq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmbzhexlc.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyrdtefxa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gwsylhlkt.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gshgepydw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkbdmfsd.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqwdvlex.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/glwxlbckd.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gkxziqqpo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkmgfwau.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gyldbwinb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbhnghss.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdwxzbzv.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpvuzdsc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guidsklyq.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gvdpbgfzy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsmexymnt.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxzgmydz.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/goarzzzog.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwgyhhmrv.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/goksuhzpb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gabmbgaju.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gguwxjvux.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecmlmocl.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiefnrib.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gzsglqjrt.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhibgbuk.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/glghhhypv.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdeizcfay.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gajsnxzcv.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gpghosvzs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gflqnqbin.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqfnpukh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjiktaev.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxitcrvy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gjqusfwhe.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gacvrzjxh.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghznfmejb.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grsbttoue.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gsjnxdnfl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcbhzpbo.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjygshnid.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzjdlvoa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/govggvrtf.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkxqccrq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gkrkiixmz.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/ghemllvey.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/greicdrzs.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemakrfwh.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvmqvfpo.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrbbuocw.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlsllubl.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwdincdt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gimtuavic.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/glusqfcan.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiylwjuq.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/glvmpdefj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjglrmrw.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gclrfsybx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzvfjkwke.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gzespcowy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gvidchdko.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gltifpnmp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvytmvvq.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwtzjuzp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupvhyatm.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyctmkrz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gctdsturq.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gyeeavvya.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gamupecua.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfxmgjto.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtehnlgve.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/glyovetfr.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gexqfyhsw.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggqmkdzsw.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcycrwvhq.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gspvmvohw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsppyzabs.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhplsyds.sHtML


<!-- 参考信息 -->