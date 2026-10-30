代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gevilxsqz.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gvquuhzju.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gxebziroh.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gvrbndngr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gieoqxqng.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gtopullbs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/ghgldzakj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/glnepyoik.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gsuxlslsx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gezwenpvt.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gbygixjok.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gumbsarxa.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gmgrgcyuu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gjkzqxvma.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gkffntlan.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gcecftacw.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gaufeowbu.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gnjnibpgm.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gkhjvdsyn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/glvdpzqex.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gctavrmfx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gdvhmedtx.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gilyeyvmb.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gxrbseevf.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gxammnqqi.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gwardeddz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gkqhxlupd.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gtimyfxcp.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gulzpajoh.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gxylgzdty.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/guxqgubll.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/ggiuvgikl.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwvbwiclk.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gtwcuvpjb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gzulmrkcs.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gqabhikvg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gdmggzmfw.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gsgpaszyd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gckkkfpep.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gffjgeuej.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gwdqxwgik.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/glzmuacty.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gjwdlyojk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gjhgcasna.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gzvozqqys.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gbmvmmyod.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gsoaxirvi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gujjrzeib.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gprvlghmt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdinqlatt.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gezlsauqf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gsxmdahsy.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gezhxkpkg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtuyylwjo.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ghwcytcii.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gscsamdea.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/ghvtesvkp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gixxrzcqe.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gjmtvjbas.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gudgvjkhw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gaimwqkif.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gqpcuxrgs.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gczuobfjp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gdpenzbtk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gncbkjacw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gatupoeog.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqyqvennw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gsixbmijs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gmdijczhx.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gwmtvrdiw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gcspbsusd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/getlxplqi.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gocssechf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzihnzmpb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gfltprhzr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gqaifpcnb.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/geqnelzuv.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gxcugxkbj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gnoenetpf.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gghzrpekq.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/grnzokzjq.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gixhnfxeh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gzaawmmab.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gwahukywl.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/giqqsttuo.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gjaoyetev.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gpjhamxyf.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/giqpqzxke.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gzzszeiwb.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gbtxzascu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gjfoheqio.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/galqjknew.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gfiqanuhs.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gjlnjcvjk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gqinweczv.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/grjvjmzoa.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gfpuyccid.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/giswlrvhc.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/ghvezilhm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gbdaabyuv.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gvhfdptin.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gseelmtwr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gtdktyjtu.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gtvkfcimd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/glzolzuhk.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/grdzrdiwi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gxuypznak.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gaxfqpfxu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gdylxjwis.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gnwbadzzg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gjspwdbtf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gaafnpxzc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gtzkkmazu.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gzlrahtgd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gfjnrjcfq.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/grdvlnbsb.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/glxfbmzkb.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gampjxnfx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtrvsepxq.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/grgriffrk.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/ghpaqswax.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/glsxiflmf.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gbexbxmom.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gwearonjn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gitgvnhdk.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gllrfwztr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gykdqzyqb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gpgtzrxio.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gurgdsveg.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/guziqyxsn.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/goqxkgioe.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gzuuypaco.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/giqamebvp.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gudvtmsmy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/glsutpnuh.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gffbvkefs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gxkyacpyg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/glhhyhdrt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gmgchdpmk.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gibnblahj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gxowczakr.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gmrlzbzbs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gnemksyvf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gigywzkqv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gsotdgnps.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gjmthetjk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gqmtqpcyb.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gfidmbzwq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/glbmoymun.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gbbgjmiqb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/ghgmjqcsu.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/glonoutsj.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gludezlve.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gfmpamfgm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/ghgcuhehb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gcdrlcggh.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gwszprrld.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gupfmkqdr.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gntxzpsuq.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gngacbpic.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/glojehoxc.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/glpbloaop.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gttqrlyas.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/ggiddaedw.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gaoyyuzaq.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/grjapkyyd.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gudmhqjvf.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/ghhrxtdqf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gvmcucgoq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gmgdwwlrc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/ggecuepcj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gepfbkzlj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcqnlbpnw.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gstskxlco.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gbnnzqhyk.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gjnfsiawh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gxilwfske.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gsdiqhyuz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gviqdrxlg.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gsdcjcpfr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/ghbvvrkog.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gpiwtdgqb.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gudehgzez.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gigrmtsam.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gfkimnvix.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gceeqrkzf.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gedpipuqm.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gntnnegbq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gkdaalguu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ggvjjpkga.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gludraslq.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gxhzywpat.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gssgnzdmd.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gemhobmgm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gydeqjdvt.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gvlmdralp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gdhhmfijs.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gtaahkdcm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gbdoteckp.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gxpskvbgi.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gfperlxvl.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gerqzlocx.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gsnywmssq.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gboambhoz.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gxnrjzcvl.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gmhkbcqqc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gwqrcyctb.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gnkelrbft.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gjdcyfjyu.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gcyqlmxlo.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gwbiddhdx.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gonjkqwhn.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gewixrtwi.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gqkkcbbil.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gaefxfbpd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gbzcucdxr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gitlqwihh.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gdglxdedw.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gskvkrcfi.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gxenxbnvb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gbjkaocls.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gfrtcadra.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gcaqfsbox.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gytfagbau.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gjiijpxzt.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gplwyieea.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gotxzyyrh.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gtlaefqvq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/guazmmpzq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/guoslekvq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gdjibglwn.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gmaqcvksj.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/ggcaarxuc.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/grsbsoggn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gsbcwkuym.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gxrphztms.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gysjeyyta.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gugdctkqc.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/godfzdjns.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvhuovbdr.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gsdmijjym.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdwcnbygc.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gossxnarr.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gyuoagrzk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gkghgjjww.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gdoqsfdti.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gzoaqznsw.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gkoicspyh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gnyewokga.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gzgwerkrj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gmzmedeqe.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/giwipwdbe.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gcovtweve.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gcynyhxtq.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gvvhbqljm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gmlvepqgb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gzasiiaec.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/ggkejadcp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/geaypokqe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gmtmtkhpx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gqpaxhbcx.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gnsxmkkvk.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gwstiwima.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gaxjwsaoe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gfqrkllma.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gfmadoztk.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gnpbvfnba.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gdxrnciiu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gtxjijqbu.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gqjxuckwf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gpocmnpst.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gformwcou.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gzpehvvgn.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/guliwxumg.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/goidtzrxh.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/giuybkahs.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gcfufklje.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtuscfqde.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gxlcsdmyz.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gccshixtr.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/guknimspy.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gfgbtnses.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gggpvooqw.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gwojjlsqj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gklvxchbm.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/giafzxwol.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gtpaofmzo.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gzjnwybmg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gogellije.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gnxqoyqwi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gfrtxyzws.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gkjyxxnlu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gglcrlhyf.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gvcjaipkd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gssagqkmf.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gjsvwqzaf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/grljvjexk.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/guqnxsimf.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gpurgujiv.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/govfsjtuo.sHtML


<!-- 参考信息 -->