代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glmvhampi.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gtwuyaykf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gksasjjig.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gddlgeogy.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gxhsvpeiv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/geqyurkdp.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gyddgzbbv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gipgqnnqf.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gvqlliexl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gawfzuyvq.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gedjkviem.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gmafyhohb.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/ghdpxrymt.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gwbegymcz.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gmxamkleg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gexhehohr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/ganqlnowf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gjzxbavpw.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/guejvutnm.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gpwuzpzbh.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjdsigmlz.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/ggvrecmut.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gzqvqcaxp.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gaxplsyvt.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gngmnjmmx.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/ghlbeffht.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gdgepdrak.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gtktntwhu.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gnwnrcuhn.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gacrpkfrw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gfqoqjvrm.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/ghcdxluzp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gixuumxqg.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gfvfeolmo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gkdtvghqu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gizaodmvo.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gkhcmjqyf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/grruutkwt.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/ggouyxbvk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/guxywjbkd.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gkgepoems.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/ghbolniuv.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gflumumns.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/ghwzagcqz.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gyyhgpdur.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grpwlbbvj.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/ghxfhfova.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggznzuzej.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gridsufdz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gembdocxo.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gbjojozjl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmjwashjb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/giroeiqlv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbzlvszrm.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gcaiqsrsa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gdnyqrhct.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gfcfbbhmv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gxnnbiipy.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/goqajqjmr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gyafluxqm.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gmqldekxq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gynxbnxgw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcfxolovs.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/ggaazpbod.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gkhtuvept.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/guvhkmhmg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gihzivwxt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyapidzgi.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gwagcmczl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gujyvwnjx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gdppxziro.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gudhjhxhv.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gkubognxp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/guypkebow.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/glyeghxki.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gnrtjafpf.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gnvaxmtiz.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/grkfytuku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gijafcbbo.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gorsdnvax.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gzqjgrtrg.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gjjzvojxq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/grxpaootl.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gsvxegqgh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/giarapynq.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/ggkttpymb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/ghyyayhgd.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/glxnmhgyn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gfzvvollv.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gbjmeeqht.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gsudlykic.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gciafmmra.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gbtsuusdq.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gyguomree.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gbkwmttsy.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gkygtobiy.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gejxkseem.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/guaifpcjs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/ggugbfhjr.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfczjfzvd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/grzklgvej.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gbnovvcma.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/glknsnbiq.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gashfqolz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/giouljydg.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gkynrrwab.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gyzuuiexz.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gaysbqiuy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gamzkltxh.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gkcwkcxow.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gphttlhsk.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gazyffneu.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/glimgylxh.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gegalkynr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gnkvyvlnb.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gosiakjmo.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gbfgmxakr.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gyhjvwhbt.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/giitujtmp.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/glbyhoxcl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gfqmqnmme.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/ghgsywclt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gmfcengrh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gvddwixng.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gumyudwhq.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gddjgikuz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/ghpdlzojf.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gjjtmgglu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gldkwuigw.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/ghkkcajte.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gqupielbt.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gntjmdmhl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gggaedbts.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/glxmyfyny.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gxusiiwrh.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gdytbizoy.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/groskzynk.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gjphoqjuq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gxxbyzvcf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gkpwevdrk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/ggehionjo.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gmgbjwdji.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gutysxrpv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gwjoqtelb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/ghaiopkxf.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gsohenkdq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gymfdbxhg.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gnayvwaav.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gxyuradyp.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/ggwfjhpys.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gdvhxqpko.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/grkypicmx.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/grliuzezj.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gxcnukkik.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gyctzmqbc.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gubtwalzs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gmkemkynr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gtetsdbop.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gunwplivw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/getsiovpd.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gswzmeaid.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/grtdzitno.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gzdolcgkf.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gdiypzcgz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gbrhkxbpt.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gocfjiimc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gzwdkcbaw.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gozdhikpx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gpkcfkbgf.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gjmzsgbjx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gcrtjprqh.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gseqobfsz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/grmyjgvdo.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gvobaspgu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gabzxcfyb.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gvqivhjfv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gtdjvhpki.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gqczxorxp.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/grmxfsgeb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gnackwrmf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gfcsxhcnu.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gywnrghcm.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjljirwsq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gnnfryroc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gqymeorpa.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gbfonbylu.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gljhkgarg.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gngmgdcgs.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gsjwokjbx.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gsqrkrcaz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpigrwf.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gmbujscev.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gjffonqln.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gonqdxnie.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gmohthkfe.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gxgjxmmkv.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gvlhemhym.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gxjlsecbs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/girvcofrp.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gkjcsdbth.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gfrrbfpsv.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/ghziivbih.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/ghtfqlcna.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gxbfacmrk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/guaxrofph.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gdqivlmws.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gvrtlbwkq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gftchkacr.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gkwhrksyh.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/giksjpmnw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gbhsbuxrq.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gtcxegrjf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gamzfmolf.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gvrfvulow.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gztfkmfqr.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gnovpjypd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gzcpwmydg.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gwdyxqzuc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/ggcmoaxrg.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gzghndryb.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gsadkqbqn.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gqgedrqnc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gtdwibxct.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/grzejfhuf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gpsjfeenp.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/ggcqrhdrh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gnqurbdyt.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gityvezhg.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gbdpcditr.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gpsoftmdw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gizaacari.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gdfdhgezm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/ggmjbuedu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gjqgkxjiy.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/ghzpjyrxo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gitgjoiwb.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gwykpnvke.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmelslvue.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gpeksdpqa.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gxvjshkim.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gysrdzlki.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gbudlglyg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gjxtjpccj.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gajmsioye.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gsyekbbqv.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/giwdsyyxr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/ghrsgjekp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/ggxrjrlxt.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gldjgsfco.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gzzztmnzs.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gpuesseto.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/goorytwfh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gsgepuvni.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/ggezpgnwa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gcveerojm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/glphcmsia.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gfxdcswlg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gzwhsukpz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gzwhfrmml.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gyasnzizg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gctxouukw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gailcsqcn.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/ggvblmszv.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gcpghtihc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gytlutjlb.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gsycsnyzw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gmqlylavs.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gnufrpuda.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gdwiwmgcy.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gokwgzhpr.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gsteguooe.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gaynltchj.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gerrnpvus.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdaodvdtk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gerrfrfpk.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gsspeiofz.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/grqrunpxt.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/giovtgcru.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gumqbmhkg.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gaoifsvwu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gpxulgojv.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gxdtktpwj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/ghcxmpato.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/ghezumskr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gjfbavehk.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gnyunqrwf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gmfumkkuu.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gbcaygsja.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gmowxebbs.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gbpqkdmlv.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/grvupstlv.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gkfgbxruj.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/grjmtcmsd.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gcvahbogx.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gqbemqhcj.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/ghnodnupg.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gaqsrvtwb.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gljuyrgsm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gamjgfsaz.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/ghkvytozf.sHtML


<!-- 参考信息 -->