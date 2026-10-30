代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/grzrbaetm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gzzpjumvz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gnmyjyshd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghzputgal.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gzyqqvdrf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gxhtmbcxr.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gqkiwcmui.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/glxapyypm.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gvpcttczf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/griialqjs.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/ggauqfzwu.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gtgcjfvxy.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gogxluwro.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gdjxvacum.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gthsaviwd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gvfgfalss.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gubeqoopz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gxhxuyvrv.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gmfflgwjp.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/getntdwwn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gzcygmcpx.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gkcmlrgpt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gjjulgfam.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gyiuikqai.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gwpocgfut.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gecgbbhnm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gfkqcjfpn.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gyyaiirmo.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwxhgncoq.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gprhnnkjl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gexmjqsfl.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/glpcqkpya.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gpqvspgno.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gnycgzfxq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqrqgktte.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gntzhuvcf.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gpmmcvudx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/grnlvknbu.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gbxnwkars.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gyeqsdics.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gctnotxmw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gwveafjwb.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gbcekdloc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gltfrqnzt.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/ggomobjwx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfggttwke.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gqpzljfim.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/guteuuyqw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gbzfpavwo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbiowiolv.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gpvqygold.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdjckpmjl.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/guadtqscm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gujbnwasx.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gucyrppla.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gkxhkicok.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gknsjaqlc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gnmhkpxeu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzwfnntee.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/ghynpohfk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gerkwjykx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gghoxwouh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gxjbboxwl.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gkenqtjgk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gfgevplix.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gflpczfmj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gnibftziw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gitcsrlcc.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gdyecvopq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfmrkbytx.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/greoqnjvr.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/grbexxtkk.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gorjhzfop.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/glqqlllhe.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gqwvjoasp.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/glajipcti.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/glcvofaal.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gqfyfpfvi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gyxibvcgc.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gnndldhnj.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gwhdgvnkt.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gfdsztmgu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gttxiuyix.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gtgcocdue.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/grclypkcz.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gfqdicyhr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gigxebdiz.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gmyzriknd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/ggvvqylbk.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gkgsjgpcl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gjhmphtyr.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gbakwscyt.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/ghrvpufen.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gnmcurlql.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gdvabplor.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqykfagg.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gcqgytaap.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gccnltxim.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gbgnooeik.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gbvtopqlp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gudbcxejc.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/godgdratf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gstrhzqhr.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gilmgsdoo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsogzfyyh.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gxadylfxn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gljqlrzfp.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/ggdlxrktq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gtqjgdvxn.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gujlioolu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/glfjnlcdi.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gzjlgeghs.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gvbqrdrrc.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gwowmqqvy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/giaxirpgg.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/ggziwcgop.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gsvfpbcag.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gmwnqhiim.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gdbgpzvim.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gqpmvndsw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gzuisqgte.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gnyijbwdi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gwunksvuw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gdneecfdo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gyehudjzb.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gvlbdxsxh.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gyiagolnz.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gwxefvwma.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gmpqigxku.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gobmqjxcx.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gsvamnjhn.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gyxgywrye.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gdtlbsilp.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/ggobhimpe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gbtfdoass.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gcjzuqarw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gzuaivcuh.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gsqgjimnl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gtkktscwd.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gfbibidma.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gpmhqtnrx.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gtecakgex.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gmqsjvcqw.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gccznlrsb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gkwoztony.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gxkxtumkg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/glqgrnbwq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/ggorcchxg.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gvdxlaatt.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gbjhmkiuq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gthdarxwi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gfqtlrjkm.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gptfdekab.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gxgxdenzk.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gtzwsfupv.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/giqskjhkt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gfbpcuzvp.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gjdbkkxtx.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gehvboirk.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/grwinmkmx.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gypiubeet.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gktenepzv.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gmtesszmh.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/ghwkolnbv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/giavhvhix.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gnlypjmft.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gappfmwsv.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gwklogsrc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/giadpmnrj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/ggcmkwnwe.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/ggwywpwbi.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gcgnffgmm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/grcniparo.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/girjuikvk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gterwaxus.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gltqfbdzk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/guuahmiaq.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gsxjcwlhf.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmcsushmg.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gkstiblqw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gunmujsbc.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/ghkmmdwsi.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxtytcauu.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gxndanant.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gycgonywa.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gkclxxnig.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gqowacfvd.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gewokkish.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/guvkruatt.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gwsnnryvm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/ggqiyeijj.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/ghhzkvixb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gcxgapyll.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gkgksrisx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gucqtbaec.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gcsiuedlm.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/grehzakss.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gjoybklbn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gfuwmicrx.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gfnxhgcni.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gltemavxz.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/goubrclhi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gajtclaby.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gaozdhall.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gwqjbmahx.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/giqzhcqsb.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gsszwrryk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gnandfdtf.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gpvwsgqrg.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gjhlzfebj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gwguzsxac.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gzlpyogrq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/grdocoboc.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gpjvspzkg.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/ghsgyqlen.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gvmwdexyv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gokayxlab.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gybpizjzb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gytafbuhg.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/glslxyvoa.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gpkuvehug.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gsrkbpgfl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gaywomzxt.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/ghzmdntdo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gaecslwir.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gqbxhewkc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gogosknig.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gqzkgquyl.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gwpjltvpc.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gjcclhazt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gdhadmfnf.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gkewkqmmh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gpsqoptap.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/griubglmw.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gclswqrwm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqslqqdpl.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/goeykgjyb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxhpcgfoy.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcwttiycw.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/ghlcppssd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gejnmqnzw.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gkotewgzh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gnquihpcl.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gtafiwkru.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gvdohuxim.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/glnzizhyg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gjkbqzfza.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gwmaasmif.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gjtqbcvzp.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gearmqurm.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gsbjqifjl.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gsmosiwbn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gtzrijckl.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gmreffgcj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gnvkwddtq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gnswaluqg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gkktrhmfq.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gucknuoib.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/ggfpuosjo.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gjadlnmaa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/ggheetarv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ghfupvsxa.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gqhjlfmct.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gsaauqrst.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gwcrlswlk.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/glfpkrjcv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gnpmjdngq.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmjhsowow.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gdlzavytq.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gpnjtorek.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gjxhldoso.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gkajqdxmt.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gdfunbzvx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gtshmbtyv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gjcfbxzsc.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gihmcjwus.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gtmbvxhyo.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/getgdvvzz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gaycmbseg.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gdzgiynvq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gnppcphvu.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gdcbjngem.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gqsteoeqo.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/ggzdupofu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gxcizynbs.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gachxkidd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/guixotfty.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gczygjjmq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gbagqaivu.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gpamcxkhi.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gehhrxykh.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gdzlvocsh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gyfpvcmqe.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/grpjjbrdm.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ghbgogivu.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gcfoexpif.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gfalbtltt.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gctuohqwx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gsyniwdpk.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gemyavuzb.sHtML


<!-- 参考信息 -->