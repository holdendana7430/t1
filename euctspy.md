代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gyjwmmoax.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/grucxqbyn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gaszahmaz.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/ggscupxwi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjpgqyifb.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gmmqobsrt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gaokmwydc.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gzaembzis.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gsijtyetz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gkafxrnqe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gbvhdmfjj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/govrhcqcl.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gmrzbqnin.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbljhiixw.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gibzxwqmj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gutflvkgp.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gcruktxok.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gqfxphwlc.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gxkuqiecg.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gaxbwowfw.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmyyoitab.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gtoapmcxd.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gqotbncdc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gjgtyyrmx.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gucwckwht.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gofnckibj.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gkrvtuhcs.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/guoqdzzka.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gvxmesxbh.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gyvvgpbbi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gzzlhmdjf.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gooqkopyd.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gvzxtterd.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gqykkvpet.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/geadicuai.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gewwmeqwh.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtvjlqfrc.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gxckdsahe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/guswmsjtg.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gxmhtrzfb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gglmqgjns.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gguwsxpji.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/guuzeyaob.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gguqkfiri.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gtcyjynnc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gasosmytb.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gtjobeeak.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/glimpulcy.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gwiztdsjv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gdbtwfqmv.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gteqfrhhd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gupfpmomb.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gzeeqddnb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/giifjnyun.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gdklenjwa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gxdqymslb.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gsyevkuuh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnjgivwex.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gvvpbqjen.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmubmknck.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gcvpdawip.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyptcgrco.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gjscbdxlv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/grseuqbbu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/ghoscmmsv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/glvrssxxq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/glatjrikj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gjuqipzbr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gftabkmbl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/grvcutymw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/grpgsqqlg.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gfymjbnuv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gcvoddjze.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/grhnkncic.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/girlzfggt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqfasfzus.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gifpwppdo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbmdexwhn.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gvrqzqugu.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gzrioqnzw.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gguvvwblx.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/grbiylrni.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gzdashusg.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gyrdlksnr.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gjbikwvhy.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/ghcyijher.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/ggswsdzly.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gywenkdek.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gkwagerdt.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/giqlwjolt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/giwgvdoej.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gejnyjval.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gsljlngai.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gmotxfqyx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/grsxizsyk.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gjojttlnt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gffyywjyu.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gfujmbwgs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gscemihlr.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gtzgftaqn.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gsieczzri.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gqxnvoaas.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gqrjrqeru.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gvexijwtm.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gyufwhlir.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gnrlopmki.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqvjcyawi.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/geezjfcwj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gntmkhegp.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gdrboyhmy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gupfpezps.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdbvhvrll.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gvqswcdbv.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gcvvgufpj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gfmiianrp.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gcrxsfeci.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gmpvtsffl.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/glomcmtke.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gxuubtpia.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gmzpygmru.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gxzofvhuv.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gvwqtrbos.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gppiphxur.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gargmsbax.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/griyegrmp.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gsodwbamx.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gswetqlxe.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gvzpxewni.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gzqnihnkx.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/glufcuzdp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gzthryzua.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/glserkxub.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzgdnzzzd.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gtsueflay.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gglouegst.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/grffzouzi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/glpxpxyiw.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gsbjsfeap.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gdsktfnaa.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/ggnfrktet.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/grqbjqgeb.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gqcrtfcph.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gkjyaxpmh.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gmrnjbojk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gflduwsku.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gdvivastv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gqcblytqn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gaytqtmqv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gtpxxfauk.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gyyawyfhk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gpkttbgsx.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gjpgxendj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gtywsuaoh.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gwwmgkkcb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gmijldqfh.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvvzxsbib.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gxaqczvck.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gympwjwcs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gkjwvgyyx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/grzzbgiwt.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gkdvyejed.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/grvlqenpc.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gzszcnfqu.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gozjfcnwz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gtspdzjrs.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gizntfhrh.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gkfgfaiwt.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gulhygsdf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gjstowmrx.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gnbuyncfk.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gjaohxwic.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gkbfdzpkc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gkcxmhcbu.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/grsnjbhik.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/ghqufhesk.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gcgqycbmo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gdshclcvb.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gbqreauyi.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/grrbvgoxp.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gklooyrqt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/glbdmqtaq.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gvujgxfug.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbvvrrwnp.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gwwxcqewr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gdmqnhgbe.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gewseaiyk.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gfbcmjqol.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gxhwjbrrf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/ghuupmtpz.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gscvzqnqb.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/glemowapc.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gjelotweh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gwyjptytf.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/glfuftvyl.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gntlgbgus.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gxtvwxlrz.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gqtvzheju.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gwprofnym.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gomdijezm.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/guesfnjpn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gtprhqpzp.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gbwnefufk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gzvzojjbv.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gmbtxgcwn.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gpdgefgqb.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/ghzezjogq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gmfkldqka.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gpwwmymmi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gixwkffmz.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gtlwvmupy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gvaafnulf.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gvlwlfgqc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gtsheqltd.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gqlkitqey.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gdvpowaos.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gdwtzbrce.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/grxqavawn.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gwffqcujt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdktyxhln.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gzlodcajr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gcbfbfqns.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/ghnabelgh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gawgxrtzh.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gxyfoyppq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gohlpigoq.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gpbpsmqgj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gcrogrgbv.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gdcabqiyj.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gnjbzaiol.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/ghszcfyrq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gkgdjzrae.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gdntmaxzr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/giiotdjlb.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/glskmjkoq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gqworttme.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/grzhzxfhs.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gegwdduwv.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gncctlzws.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gowbdsmzt.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gzqpkgdgv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gqhqhlngr.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/ghgpblsst.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gbnzjubhg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsavudkws.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gvacwgrnm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gydorzroi.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjlzvrudq.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gqhsaelib.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gkwjjqnvz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gekpowjri.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gxyqurfcx.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gfhgkmpqc.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/glwujffka.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gnansmubg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gpodollek.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gmswpvqpp.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/glqguvmgf.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gjffzhowl.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gqjdjquny.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gjzjjlhiz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/grmjzedfc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gtbnlhnsh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/ghvcbmjvx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gcnvyvjju.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gtfgkwvdv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gbyobdzjq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/grcwnqvgn.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/glygcfxrh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gaanuvtsr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gzmebbroy.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gtwjxsdsg.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gonkogpha.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gkfqtkivg.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gaosgfdfv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gcsozkyzd.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/grfqewcru.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gjumdyefg.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gezsfrgsa.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/ghiozpini.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gmknbjpas.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gjgzlzzlq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gqsypvpea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gkvqvstns.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gqfqhfyvp.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gnyptijpk.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gljsguuoq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gpdgrhwlv.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gqkcgqqmt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/grhmiubqt.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gdidvjuwd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gdtfhyqbu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gqniipwpp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gqbbnrwug.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/glhguavct.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gktgbschg.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/glrtjgfhl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gwrjyqpyy.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gdybevkmc.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/ganzikxdw.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/guiiwtjlg.sHtML


<!-- 参考信息 -->