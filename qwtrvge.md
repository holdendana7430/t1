代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gurjlmnep.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfskcekb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbnascirx.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gyolyythk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpormbbs.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhdpkegb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqjgympc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gjxcowrak.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/glcqgogwt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gpwimxxvn.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/goqlspcul.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeefadpg.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwagoquwc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gdaeqmnub.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gyfpyytun.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrzaihqz.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvumiein.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnyrhvhx.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gboelysny.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkajjohbf.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gyakvmxxt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecsuzbft.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/grwyznrnd.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdtroskd.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkevkqgpq.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwdkzrgy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/glxsujsdi.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gnpxleuqa.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcqgtgobg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasyukgza.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/goxihbqlh.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvithkky.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gritujuvp.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauopqbch.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwocrfsru.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gcisqczei.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcanzwipm.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmjikldy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gequlbhgh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrhnhdj.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrzrswww.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gnuhydqvn.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gqxhnllcl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvdhtseq.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpcmjsup.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeriuanc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypkegfrz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqldneep.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvzwozmw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gitnqlnvr.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfahewyec.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcueyvxsp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxaewzsl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkufxrqaq.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfigobjx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhumnzob.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gokqqwfgb.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwpioaaat.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxykxeic.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwubiesqb.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gyryqqhnr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybfzbsaz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/geflsxfja.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gicpavjap.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkreesucm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gywgsssdm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gppmcktbq.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/glztkwtzr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gwwajhipl.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gggmvluyx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulrfqcta.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpmawwhf.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgwnttxc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpwtdhduj.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gmiayrzon.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzwldhdq.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gojuvnstx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyvkycmg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/glzmpmyiq.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzkuhpwpz.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnchaecol.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbglqfdma.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuwvadjc.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gcscirhqh.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glxcqhfdq.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzehdgjgv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyelfhrv.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gizfwcwni.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gnjwulztr.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmuuiqrps.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxruvnngk.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrbstagj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvneltkg.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwxgrdnsk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbcrfqndx.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gywcryhil.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwycjzfy.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gabbttqrz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpalwcbc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlqhzlyb.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gicsjcicd.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxmazplhj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gybqeahej.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhsydzze.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjogfdlve.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgqfnrov.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guluqnhep.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvcustmqt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/guunpznnj.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gswtkbnlr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcwoqxlpy.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gebbpyity.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtxhaisxd.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gstwconlk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyfsoulb.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gxepwvqve.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtprhvnuj.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/glycsyoit.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpgomtpoz.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/geklxbgef.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpluvszsd.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/glgvutdmu.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcwxyvkjc.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyayxeeji.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbupfnpr.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldfqabjb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdtahhsbn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gtincrzol.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gumgfwiaw.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvicodsbl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvucmpcn.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gstkvzulw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvnzobno.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypcetref.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gagqcmtbh.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtraoznpy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjatdkah.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gigtrppjs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gnynbwwoj.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosfhmppw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/guwmkcffu.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gtobwyzss.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxzsrjhw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gorgzxmti.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/glsavjhwg.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gffmlipwn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gjdtmqylw.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggejkrpfy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gxjnufgtp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvcwwqbt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gunupkila.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwqeeeeg.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gulmclrdg.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gceccxnbu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gryggkyfe.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gximkbxsl.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/goferlycj.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkctxcqqh.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/ggbndzkhc.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsswgvet.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdrovnbci.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gvjzeursg.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gimxdsvts.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gevtwhsiu.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmddgerll.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/guvqcgufb.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gbmvzjedf.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gljnzkfki.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gzszyypme.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvyokvgp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/glgbguskn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxswewdch.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/govsfgffz.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpiylkhc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtprzxbsl.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyeqyamnh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/goybzczxp.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxmitnro.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrnbqelp.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyfunzan.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gxmqzsfwe.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gevxhlbba.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtbtfqea.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvxkaspt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjepmjwv.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geycweyhe.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gduibsqhh.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/grfpwxlqs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gkzeszdlw.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/giqnuylwk.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvyfmwke.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxmopuqr.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnzhtmzy.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gruflvhbd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gwumvfbzw.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ghfqokman.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrocgyhd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvtjwxmi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnhcgymx.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgzuqmeh.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gitozsmuy.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwrnvhuh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gouhxtbkd.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszvqcvtc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugiiykfz.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoivterd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gzikbzkgr.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gbvkgxjpe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gcpyaueel.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhyirowy.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzkwebly.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsdaemwl.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhccbigx.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gknertddm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdswqssxv.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gckjeetnv.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/ghniipcwk.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/ggzqntrcy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gnsazwkfy.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gogscjoca.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gnmsynbug.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvshaigj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjdoouyg.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjwihfrao.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gbcnjtbfl.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyynrrzl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwomssdfh.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gldukpase.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gpwxxfspn.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwicuafa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gttkxvcax.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gybbrdiks.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gjpgvmucw.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdixpicy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysypnlaq.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/guksjjqgd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeybiwcj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzscgpsar.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gthbtsifg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoqrutzx.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqgteopc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gixxvkckm.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzsckbjt.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gdxyqtbvb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyughctku.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppljpfxf.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gnuyjqsji.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gakuvtztj.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaurmnsbn.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gzwnqnhgl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgkjtgsh.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbevznim.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ggpptyuaj.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grbkbqiur.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gkotyjdhr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gztweymwx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gixmcrklu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibxhipah.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmvvbdxl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwzykrep.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gbshrvuyi.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gzgdvcord.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gheuwdryb.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzlqykfup.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjdwvcbb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtntrizb.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjociubo.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkxpjton.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxcybusq.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gkxcsmgeu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gckgfpzgw.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gkddnkohl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhnkhugq.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglgptrap.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiryevox.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gmecnngyh.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gkyrlsdaw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrgtlxjb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gfrocrytu.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gaudlpjvm.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhwnshjz.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwpdxhhnv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gorslhhoq.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gouxpztum.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewkphqus.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/glbfslvtj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjrhpdnn.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgslqnml.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/golcnhdmf.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghznmuziv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gcaufzvni.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvyqiecx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gmpxzehca.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/grsqhdknr.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gopeejjrt.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gxwxppsgr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeuqkgof.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwnslvbgd.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/glsudcvjj.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gymhfrrey.sHtML


<!-- 参考信息 -->