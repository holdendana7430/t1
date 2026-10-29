代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gljiyewfv.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gacxtscxf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gahegtyqc.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/ghrtgxzrm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpcnlrzaq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/ggqrjiyqd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/guuqrjkxe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbpiqqdre.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gnqqhqfkk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gdgtifcks.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gnrjdidyj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gvmwyeuew.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gjthyohcg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gvnkbtlja.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/grhiktyll.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gdrjcmayl.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gnnhkyiok.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/giejhpvzx.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/goigfkcbj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gzrpvflip.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gwuhgvpuz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gbcvdrnpz.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gtoqylqvg.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gsmnrsibh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gsvyuvzcj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gcouryzij.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gtdxylvsr.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gouymcwxp.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gowkbzcxh.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/ginkkpjda.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gjtnpzeip.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/ggrkwokef.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glfyaksjh.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gdqeifcai.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gzokuhkaj.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gwvixyjtj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gpteizvzu.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gtyxcvlzx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcnyjfczf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gohbsxeyc.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gjqvcadpk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gecpcalfs.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gvdrvmjos.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gkyffsjcw.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/ghjvdjepg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gouixkoec.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gxtdtfoxg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gseouapbx.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/grkkbvrzr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggrjhhwqk.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gdqrshlvs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnsunvmgr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/guuzzbobt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmfczjlkz.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gwzzlpfea.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvlaelsnm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gvvrtkfop.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggeilbybi.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gxqyrobyr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gnapzxezq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gcmakgsbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gqxonhucr.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gfznstrxm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gnzhnleuy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gmkkwuwbq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gcllzsysy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwaytpasp.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gvzeeubdw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gswuecady.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gzgheasmu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbaupcl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsfwauqly.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/ggewjnufd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grsulukoo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gplwmrprs.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gtllqsoxp.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gcuydxzts.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gvzhuqnyx.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/ggptqcyjq.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gfnqdawde.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gbfqmzgwj.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/glqptckpw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gwzbwlgxj.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gdjlodjgl.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gcqemamhy.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/govzhdnxu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gbbsvpetm.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gyfbhwgtz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gyhnxoync.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gwxbhvrtp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gcptmfmph.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gtdkudpjm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gauoadtym.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gurrsuuxx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpskhbpit.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gvdrfxoja.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gdioxdepf.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/grebatwxc.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gjojwkqqj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gjlmojmyp.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gylxxsbps.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gxvikdugy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gzcwslhgt.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/glyguxhrd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmoibyjmk.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gxthfffan.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gqsmdndkf.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdprchjnw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcrioeudz.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gelvhuqww.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gkwbsyiye.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/ghaupfjvh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gtnoxumiw.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gazqwrxiu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gzwiesvzp.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gwpkppuhg.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gyzpwxobe.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gdvuwhzrv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/giztomcfh.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gwfpswwnc.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gtttkvihp.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/grbplkvmq.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gdgddwqje.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gclhueqtc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gquhptcfd.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gitcgzfgr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqsqrnaat.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/geqhgwdkn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/ghxebtwag.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/ggzsrhrlm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gfnixbkme.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gucnknvxy.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gtcwunmyr.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gslyzlqoa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gfwqhqmme.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/glzzhsofs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gdvggsuvz.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gzlzylaio.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gaylcgmyd.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gkesijedm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gwjfazyiw.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gkyrglpop.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gqnxbjkbt.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gnatpzsra.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gxjahksse.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gcwbbhxnb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gmbnxozoo.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gpmcyavew.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gkcqminna.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gcthnlzbn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gohrgbuly.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gdlovrzkk.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gaqfmccqq.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/ghoqfyggz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gxvvfrpbq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gighwztqf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/ghmdczhfm.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gihsxzjdw.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gffgtolrb.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gjnhhtupq.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gdorkfech.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gqqnjoefd.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gavdloomy.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gejmutfxq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gtjwydqyp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gbkotmjwr.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/grhhnkhod.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gjoedmsuh.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gkzuuhqrb.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gaursmlvv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gmwelnwip.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gbouclynl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gutzgkxqj.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/glowvuqrp.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gxfmlrfbs.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gvsheelcm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gnzknyils.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gsukydqpn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqlbwxhmq.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gplhmdrmc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gduktguhg.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gvboeiwpe.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqnoztldi.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gchmmlzxe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gdxtooyvl.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gckykgvrj.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gusfcfoaf.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/ggaderoeh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gxxxcvled.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/ghwtipuuv.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gtiiproxh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gcpnvkynd.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gnzkqmnzs.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbcrgmbkm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/grrfgzakg.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gugkhjgal.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gjyualloh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gyqrqeuul.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/giffxhjad.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gxzhmnjqq.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gdkrdozbm.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gtchxvoxd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/geeoweagu.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/ghwcjhtcd.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gdbtkknzh.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gqvxaktcw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/ggxsfzhwp.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gnuivrkth.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gotrivpye.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gbhobwrmg.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gqqistuks.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gfyzwfrcq.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gvhgcvimm.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gpqamgifv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gilmntjbs.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gziqjmclm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/ghqnoecti.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gyzpjhhnn.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gpdgdiwwf.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gvirxudnj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gfuwijduk.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/grmtwnjen.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/guixsadey.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gicviweis.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gsbyjfqfd.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gebzsxzae.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gwkcssjxf.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gyqmbyijf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gykdxdmee.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/grmgylgru.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gnwdnvqnv.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gualsonem.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/ghjnxwuel.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/geuaxlyxd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gihoxowif.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gfveslrfq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gcvdqipaw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gvffnpuqs.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/geypuownr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvzgbjvhs.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gbbkzfofe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsusqwbov.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/ghgdvcvwu.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/geryfmxsm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gtjxjjuqp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gboftgmkv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/ghukjvrdh.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gcjrgawdy.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gfxyiayud.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/geukokywo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gehdbjtwe.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gironfhfy.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gqanuvqkq.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gmrmflymd.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gpjbumbbq.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gwkktifcl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gwlnfmlgl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/ggfzoxnin.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gbmfxoucy.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gfsrwaahn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gsbefjzwc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gmrtgbfqx.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/ggufyafte.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gmhgeewks.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gtbiapimb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gelqvzlqh.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gpxjitdgx.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gmlzzkdmd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gcmttproz.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gphhcivyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gpwbuqprh.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gdbeltahx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gufjqaobv.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gqezobarg.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/grlvzwskj.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gkrhzrake.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gfehaydsb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gnreynghz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gexgfbyya.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gmwgsnkug.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gzbdcivml.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gipbekhrg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ghoggppkt.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/ghusgkqwt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gojstxyvv.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gzwtreywg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gkmoabcfi.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/glpetuyvz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gnmaulldy.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gxdzmcvoo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/glxtcrzaj.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gaqdmcggk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/grbukcrsg.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gnggebjlv.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/ghrkdgekx.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gtldactbu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwvfuvd.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/givwikeku.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/ggtqwgfpp.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gbpdfqtyt.sHtML


<!-- 参考信息 -->