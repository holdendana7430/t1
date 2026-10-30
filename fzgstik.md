代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gikmypfqy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxpreoif.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gildjxazq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grihzeifu.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gmrejbjnk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gydjglmpx.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gjkkrvcbl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gglowrlyk.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwnqypfr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyjpfbtp.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrqcgnic.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gmpjqrxod.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrjlduqg.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzuqyaib.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gicymqtbe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghscqisjf.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/ggigygdvu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/guinylgfj.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucmozipb.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gpsgktfss.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvigtepxy.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrbjjmsx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gheyvvvtr.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gsowkhhel.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpuvybqx.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/grzjfsfjq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gypsmjqdx.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlyzlwfj.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjclspsdj.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gkicxpoxd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gklkfsvtk.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gyuujbisx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gcilssqib.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvposahvq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdymzqfrj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/groxavmpr.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpvmzdkn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/glpknissk.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gayofxiws.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gfovfkkrs.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gcarebxel.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvpsorhs.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gevkirchj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gibgzkhnc.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gdxdmqjfd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjcfqyhs.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjuofxlbq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkxsnodx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhctwohz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gukhzljvo.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbzojtzuv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gindvchqi.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gnpwrinsc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkhrljvzt.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gsysdgcey.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gumuhxcic.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyniawian.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gjfsnvdkn.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeagjbmm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gaxtjjjny.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlfacvqy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfldoafs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaxrmfajl.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gybpkqijv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/glyiuatsp.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gfcgavdxd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gjmrgzcyt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbwwlxhu.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gbttidpay.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfldqrmfo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gickumubk.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gakttwkwz.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfuecrcw.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gpivgvpia.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnmpfdvg.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpogvjdg.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/goyciploq.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/giahghjbm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeqakiwh.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojxvvhjk.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsadhrpdd.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlxprvpl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gikfryvjc.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gohithbso.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoluwzjv.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gvyznoskv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/guikskxma.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyptyxlf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gmryjgkej.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gbgwxiwto.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/geanwmitq.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gsznbqsox.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gwchwbdko.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gpfqbmbgr.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gqsozgpij.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqusbkeef.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gbbwrbjzt.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvmrqrja.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghyzhwwnq.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrdquzly.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhcsqvt.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/grokfhrgz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnbxmeylg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiuknbcu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxeffpmgy.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/geuileroa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzlyuyada.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmklvkhp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqjmkqjho.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gzxnzkbsj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfbnfpky.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpauwqmz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhewgefi.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gkiiyomvo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvsisvzg.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gmddlrtzd.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/giuagoaid.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/getwogzck.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyhiduanl.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdsflaan.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmwztted.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gexqroxeu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfhlonvc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gujnibrzp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiwlxrix.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grraatqjd.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gfoytncas.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gellfbomk.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkuvaqbu.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gugkkdjlp.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgvnwwsd.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gckaoobkw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gouxziwyi.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbazefedl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gupsyxpce.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaauxkvh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzucfnim.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/giufztqrc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmoyhhfu.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gdricjglh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/girvepknc.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspqoqvjg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gmjhuuqol.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gypvceqdg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/girsjmjqn.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gclodedsg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gjhpvtmlv.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvgqrcfoe.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gezwawtmu.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gyazcqlze.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/garsooqbd.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gwbcxnwzk.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gpfkacuqg.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbemxqigh.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gwasiylqx.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrwdzfav.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrzezjlj.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkmuwwet.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdyvjfkg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaogitnwj.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gwstcgbhl.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gdaabowty.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtbyfuig.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/grvnmvehe.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/govlqmfsu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnttpueoh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gecnehogy.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluhutopv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaogpssl.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytbpumpa.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeihrrkm.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfydzvgxx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gbexuticp.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gxxpstlsb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcothmnp.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/ggcksptgf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/ghdlhkrtp.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/ggesewfgi.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggsmbbdut.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gnqzgwuld.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtqdbfwp.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcsxwhkk.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrgqpmxq.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gitywwbdz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/giaqegfya.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gzdjlzhli.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqpkoeff.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcgkrrmt.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/glgtabjnq.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gowgumqbm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gflvmidxn.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyoabhdi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglgxaxjg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuehepke.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gptrjbptr.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grstjjkgd.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwzpzwgq.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnirejyfj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gmchtfpdo.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvshmcwc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymvvhugy.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfllzwiqc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gssnbtrqu.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gvipayemm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gudwkwpci.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gswtusath.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzstmvkr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gqfxrjcdx.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gxowewhgt.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gatxvfnol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmabhfnic.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbekrfty.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gzdfqbrey.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gneftnwvk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlntbnet.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gvrtqytsb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gujwogowd.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/grbmsmbyz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcjhmrhkx.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gjougzbmq.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gjstfnsml.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gdehebebo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwzfdjnnl.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/guvnzruiv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/grrfqcxvc.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/grwrpbnfn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyttzbfk.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbspgupp.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gdctgkpfx.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gykfgzeiz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtaexola.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/geroshujp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gngtxvwkr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqwzdnjt.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gxyafjiur.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmsghastb.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gyzdyrpda.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxbqkhloi.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmvglctq.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/ggggwlbdq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtlfhzcy.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gosxzpbsj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhgcwogm.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdskkujv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gokirgqse.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gfudwnssg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyogtext.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpmjsdnb.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlxzobrw.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grjzqnopk.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gvkhlouqi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoiqrvcc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/grssofbrb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gtapzmoep.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gsjdnvfsj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyzqzdqt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gubfyibjc.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gstoxgdze.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrotslbh.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gctczjvvz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvljibkoy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaliuyqp.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gshnonroe.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwodtwehz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gocraicrj.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gsrzvbmiw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/grrdecszn.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gdzdojjmc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/goaibpkwr.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfylianr.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpzqedxj.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/grtkihhkw.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgmskuhi.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjcqnmyn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/grymnrqwx.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyydwfxr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaspfkzuo.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdqkqowhq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhafuyxy.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/ghzsqrawc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzpmmdff.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gdphbqktq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/geofbrudm.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsltodlcw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjssuqvsk.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gubhewout.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmncmpohn.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/grefabhla.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gqpjdakfc.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gpffloivv.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnerpztqq.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdjvukin.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqwbbknt.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgqaimam.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbakhrvhr.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtrsoncdo.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghajjpuwv.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxrdylbd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gnkuzkdej.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gcstklynp.sHtML


<!-- 参考信息 -->