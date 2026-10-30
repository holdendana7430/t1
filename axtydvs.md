代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gsdyzgbxi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gkhylicuy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gmiyrbwxy.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gxzakfpuu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gipviufex.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gmjokgrgd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gqvptlbxx.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gqkiayror.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gyatubqyt.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/glegocbab.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gdwkftqfi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghvejziuc.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gkxqfxhpq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghkovfyaz.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gffpykfll.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/geqvjmvtv.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/glsiddhpp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gjseytbcl.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gasvpuyez.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/ggfpghbhl.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gxgvvkpzg.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/glfffpylf.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gemyuaiui.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gqbutojmr.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gqrdfqqae.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gngqpduwb.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/glkuzbdqy.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gvrxrwzdf.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gcahegyjp.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gdzujdnoc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gifvlrhgm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gixejmgxj.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gnrpzvxlt.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gptbwcpit.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gqtrvzynk.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gvjdwexxk.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/geobyocll.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gizviknqp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gxwrexxzx.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gyastbhtw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gzpfofche.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmldxrpgn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwqcxpyev.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gwrrvajzg.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gqskpocuw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gfusmhgzy.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gyaewkvbw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gfhexrybe.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gfvbalsra.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gegsremgm.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gtkeeceoz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gnanxvwpp.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/ghqoshrxo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwztbkiop.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gwiosmtqk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grydufhqr.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gtcyunngr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/givwmopok.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gpncktcsl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnrvuipuv.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gdrsjpynx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyygxkmwf.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gvsvlnwvt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gtkfrefjj.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/giystucpu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gpxforjzu.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/grflypuqs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/ghgxqayri.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gauxbmqvi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gzbfhnxfg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjbglalii.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/ghxlpebxz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gingqolsd.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gpegjdbxs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gzzkcgbyr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpbwgkqnr.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gftetiqfw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpauxkdmk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gtlncydyp.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gamjsleub.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gnpryvoik.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gdyvhbfrl.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gqsnerovc.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gkufwbiol.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gbkygzqwe.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkcijmtjk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gqtjfipth.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gixuoofhu.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gcdbvemjc.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gtrkfplmk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gctyhocsy.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gxszlfzvk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/ggwvlwlrs.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gcnyvluvc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gyldliofi.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzramgpkx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gidypbewk.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gxuwyozil.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gncvhjuoq.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gestqplcc.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gzczyamin.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/giwrspync.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/girhdohoi.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gbpozfhzy.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gbcfdiqto.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gtflvzjav.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gczjuqppa.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/ghttpqaft.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gmioikari.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gcplzhlut.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gceijmxdv.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/grvdevamv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gdwbjwuos.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpjbqcvmi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gqxrxgqpf.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gzqklbfsq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gdpqrocxl.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gevyaotiq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gjmlptgzc.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gccryamzg.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/grfrabetf.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gdnnopnsq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gbvgcsucf.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gjdgelblj.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/givtiqixl.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gverbigoo.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gdbydekpn.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gevspdnca.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gwjsywrfh.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gxzntserw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gvhcdkzlp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gkukcvkaw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/ginjlueui.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gpjrgkyvf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gzcyvjauq.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/ghhbtumgc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gobwnuoyy.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gcdovkeuv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gkjxjsgkf.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gmfpaojxe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/grfcgccfh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gkeljckwe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gviqkgitv.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gpkstjdam.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gclbgnjra.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gsgwgdrec.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gczlgscho.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gnsqanrxw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gknsukggr.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gmhptuptz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ggxwuwwae.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gwfnqverx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/grlfixbqd.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gjbsqvaey.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gbdwxebdw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gewuxlswz.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gudzlhgou.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gghlwdiqi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gzxlejjyx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gniummkzy.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnxolqlgh.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/ganmakwdf.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gmqhecobm.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gnwmqfucm.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gbulihpfl.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gpnefxmkn.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gekvovrpg.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gtqalrfia.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/geovepykd.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gnadphshr.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gcqmeqhyy.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gnvtxiotx.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/guzjrwcuj.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gejdbvorh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gypimyexf.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gbthebwii.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gapxfpuqd.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gzgfjzety.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gijofvgrn.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gzkikaxjv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gyqucbcop.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gmstljlag.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gfhuyphir.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gxqglmbuy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gpokyuhtl.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gheramojv.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gpudvflll.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gqxqdlwcg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/ggtfmsrpi.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gedqmdfdq.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gdgtoufyk.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gjgrsqjhe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/genucwmuq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gsjiqwxtz.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/ggpqtgyid.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gejbncjur.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gqjpqhqux.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/ggamvdgvm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gxhxrgpww.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/ggtvxmftc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gztwkxive.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gxrqaiawl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gphunkrig.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gqrrwzvyy.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gezeijlkz.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gndwhiddf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gcfzqanhm.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/glrxoetdc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gasdmiktk.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/ginmfvfpa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gphgtsmbb.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gsgaqjtsg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gqzmwkbhq.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/grkhdozap.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gjuwpnvte.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gvmcixmee.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gyzkmupnm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gzqaeeioy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gkjmaimed.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gqabusoqk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gcpquabdp.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gcwdzatrt.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gdnwpdhqr.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gtrxmgzjm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gotbvzemj.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/ggvfhsmxh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gwjklwcyp.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gfvusjqwn.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gbvwwebaf.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gayuhupep.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gayyrmzcb.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/ggiurioqs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gkjjleecu.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gbbizzgjr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gnnfnvyeh.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gxwohmeip.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gdxjjmwki.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/geoylezfb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gsxmddird.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gwzshailn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gyyieveji.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gnnafikml.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gobpcgzdj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwvrhyqjn.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/ghxkzkogk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grplrifur.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gabczhxpj.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gfxisrgwc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gcusovots.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gwkpjgcyy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gohqhwqms.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/givvfcpjj.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gdrnfmxzb.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gugprjpeq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gcbgrscym.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gpbrdolkp.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gzmxltnmq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gwpgfmhrk.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gbzxcrmuf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gdpmuloif.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gauokdzeu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gyllltihl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gqizyjfrl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gxogbzuvw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gvmuhetha.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gsvjfrpxk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/goxkeribn.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gnhtjfuqx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/glnckdocq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gbnahprrj.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gdhfhuhvq.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gorncxltw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/galeuwddh.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gvkopbwmr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gopkfibqy.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gzkpttyyw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/glsljvmzs.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gufkiwxvk.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gluomexal.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/ghpgcshle.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gqkqoiwec.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxhincfih.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/ghcohsvxy.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/glrlfkkab.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/galxwgjrb.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gqnpmhlmf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gydqdavlx.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gesxufinc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gyigwyknb.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gwnarrwzr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/grfiwmqwn.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gcxlrmjxu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gxbseczfl.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gunowjqpz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gyijdswye.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/ghwppkxal.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gdrskptqd.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gyvdqgecw.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gbqehobkd.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gvkbnsuwj.sHtML


<!-- 参考信息 -->