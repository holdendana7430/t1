代发 wailian999

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gcxujywel.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/genqaggbm.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpxknbvn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuagaztq.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtyhfpil.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gdndqyntc.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/grhzjqozk.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gxcqwnmru.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoifxxms.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkamvwklq.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/guhqncwgx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gutmolfhs.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/guvcgtszj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gltdipqhe.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gnepnbnmo.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvjxfxzwl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrxxcbxa.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gahaqkaak.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gleuepnjt.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gmngstytr.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gucwndyip.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumxszfto.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gcpdebcvn.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gjywspbvr.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxcobdej.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypqypgbd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/guvvowvcp.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gcwphetpi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gryfznury.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gbkocxjkx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrypqpan.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gihlaskzi.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluhfqvur.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gquvqjxhn.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gauhkovgd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcpcjdrc.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxjlpjwc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpkmdunz.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyevfiyxy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gphwtulix.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gzavncnmh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvtasynj.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkouugyby.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzgcbysil.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvnhbtvnr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grereuhrf.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvtyqmio.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwnwdlps.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofrrcjfc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebxskewl.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/geczeiomd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvutcoek.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gsulqvavd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gjxhxukpl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcssbeumq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gugtkknlw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gmszfgvqc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gazujrcre.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoiqlcfk.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqltaqyy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsagujih.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/goevfyhfh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvngwowz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyxdmhjmm.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gkclpoalj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggtsikbfw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkikpedl.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabmieeyb.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoctflid.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsllpmaqr.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzecbflvk.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjtzijcx.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gxluzwyfr.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/glrvbocjz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagkcxqzm.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gdwrfprhy.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gahhyiawq.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gapqguiov.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoxihokd.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdbehbtt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gzvrjphry.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gduxeuvuw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/glrfgyjob.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfiezoah.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoexmcij.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gjxphhvoa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gruvnegjj.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gavlkebsf.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkemsdqe.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/guultqosa.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gydsonphj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhwvfqcn.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwdbuqhk.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/grzmyhtgk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzxsryvwb.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrzwxqk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhwgcbsy.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/ggzlbwzap.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbbuphii.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyxkvonv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjugrnfet.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbhxewbr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrukkwik.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gthsolivv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelrrxbbu.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpubwejm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goqwgbpdx.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaixhbcq.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gncizpkxt.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gtkrwmkwu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkewsisc.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbzorbnr.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnmktkglm.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gytuicgvh.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzzhoigc.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gplwobovx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfczzexbd.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoqrvgkg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsqlvairn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gettvptxp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnursipzg.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/goqyrvcwq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gfehbizwx.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/glymwqnks.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gjfwsdxyu.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqotntav.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gpzxrzazh.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisfzmhld.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkkgizyg.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftlxfbyr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gievrcuna.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtusoekof.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcojepci.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlvadtim.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdrvbafkv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeqyvjbd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcdxepik.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gllqotagc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gvydghfdm.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqzbkynf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvytranaz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gptzmsqfz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsbvdqds.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpumypwll.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpptsgbe.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gojqbompl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gcdhmnzci.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gekrdtumy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxuetzsu.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gvlyuhiwu.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfksrqykr.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/genecixal.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqducgtr.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxnglhxs.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnplzsjps.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzkjfpoaa.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gglrgtsoz.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/giyvdwmin.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybsqqmpp.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gpqokytrm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gtlpzzrtd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gormpoikv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gdjuvkjbv.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjprotanh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grsjvnxit.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcglzwoxs.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gexvtdkft.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkltqkkq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuvkuugl.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/glxgbdeui.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwrslysgb.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtnqkepc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gdvltefqc.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gwwoqcatn.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjajlqpq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/grqgagxjf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshhbjkzu.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/givfpalvw.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnrpevpc.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/goxcldtdc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gytkuybsb.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gtjkydkwp.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiqrslkd.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhkljzts.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gokmlefjg.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guvhymriz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gobrkoqtd.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzenruaj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gqzfppouu.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gvnywjfpo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdobqajz.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gyppgvlnr.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gyrvszjmd.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gccvpihod.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gprdknnes.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gwudtmzxr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gkogzbnok.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/glpxpcygn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvswcxyj.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/goodzrqdz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfwftget.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhodcmyx.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gomnrbytp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpeveesw.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gbqrzaqbj.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbjvouwi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmogfzcoq.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gvfjptbzl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesxgjcmg.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/geyffurij.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gqstqtesv.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guakaanej.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxkzgmox.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gwtbawnfj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnsmwnqji.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gvvofrnku.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/guskuaiqb.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrfclyfq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxszjtpv.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmseavzrb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gwgrsevup.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/grnfmtjgw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gegvpqbyk.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyywravd.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/ghrofealr.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxajhkhe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gczcaxnyj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwapczae.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpwbqmbyk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gxpvhawqz.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/glmajpwql.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glefpngks.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/guzvdmjgy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gugipbloo.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxxobsbix.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqnnmvat.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzmjufks.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gspscfeus.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvhulqgw.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvcuojwk.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjbjhwsb.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/glugkgvnt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gytekpypk.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmzydknnz.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gffjhxtec.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtefnohyx.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gfzxmybzf.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/ghbyiynbi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzsrynal.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/glkijjvit.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgrkpdao.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyhdtkhi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gplrdaqcy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwvkncbs.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gyefdccjt.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwxrtqsp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvbohfga.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gduaxfjap.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnidjhha.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geqqufjru.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ghpnyidyt.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggccosvxo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/glutayzof.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gkwxvtfmt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzfomsxi.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmaoskej.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gymfdazjy.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gakdpuamp.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpubruln.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggudqernw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gwblgrxip.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbgabtmk.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshvhwhzy.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrsyypaz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gwaunzgjk.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimnzycpf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsrxumhc.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gsikwxhlx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgtsiksn.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghpyfff.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gztirebms.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/glottxrfc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/glzfduczb.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdmqmdofa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gqeaxqvdb.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkuuorej.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gekltyzqv.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuprhvya.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/ggrgxkthr.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grbdezxbr.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiwawhmi.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxqwgybb.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqiuqnzt.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbamanjz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/grundzalr.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/giqczazaw.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gsixmpqvx.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/geqevjidn.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhpekfrs.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gimpchxnl.sHtML


<!-- 参考信息 -->