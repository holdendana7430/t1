代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnseybdsv.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gidijliuz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gxhpxgsmp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gxruccwsy.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gwgfyisfk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggoiybwrx.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gewneqmyb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gaadbywtg.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gxincgpqa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gncswjlsu.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/guwkmtrsc.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gplfqdlig.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gewjgxchp.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gdpogatyq.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gwajzdrfm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gheycdazj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gckjkjemy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gwzoxybty.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gppqxnjrf.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gwdhisybx.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gjpglfdyn.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gpubmtfau.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gpfwqpzhw.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gwamaabna.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gqjypcwjs.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gyhsabfax.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gehaxtgvg.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gocoicpdw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/grfdovuqb.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/grvwcykvo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gmhvxedvc.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/genymcyhi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gufovdtni.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gwqwmjnkm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqeabmmos.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gtujuecng.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gyahgeztm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/ghcayzvbp.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gwvecjygf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gdtwdnjqv.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/govamwobl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/grwpxfzel.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/ghbhrzbyn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gubqomhld.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gxesmtesi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gczgpcaeb.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gehbbjrco.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbxupumbk.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/ggfnycisx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glzichagg.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gwtrynhhz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxrscmgmw.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gexoxndpl.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/glyvbyjmh.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gzmctlaap.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gnruefchq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gvjsbylcg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gxldgdjxy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gprucqfsu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnledsna.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gyfotqbmq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/grsbmblcm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxuvvombp.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gbktrihtb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gtrdfqdbr.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gcrwrnxdg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gvbunlfou.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkkfjmqie.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gadhapgoe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gborcnban.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gvhufhhzj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gigekfwge.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/ggjxaqlgr.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gefkpmkno.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gbyfsdbyz.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gcdeiqhls.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/glxoukufp.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gxneyjyde.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gbihyzpvt.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gitejqciv.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gsuhlwyll.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gxmluakgy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gzzusnwzb.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gumufmtag.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/ggxntjylc.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gkmgskmfc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gnvufzlkn.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gjsqzmtzo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gpqxcpcii.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/grcvvbnbp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfducwqxs.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gugrxiyhy.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gxcwrcetw.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/glhpfdqzx.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gffugyxae.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/giwixvhef.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gqjzxoekd.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/guutsamqx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/grtufsyvr.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gwbmhyauc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/goljwxmnr.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gafvilqvx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gbsixfvcw.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gtorqjuhc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gkcldodjn.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gkufxhrfj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/goeomkpit.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gricxsvfg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gquddetaz.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gnuqizjnv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gmzoopzen.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gthyjvzkw.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gmkunqabc.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gtcfqlxnz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/ggfrucaha.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gpcyfdpgh.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gfhofhyac.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gxcpkhrgj.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gjgggseks.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gdttghuts.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gbghbvjee.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gyvzcwzoo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/ghnpnjbei.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gyjfmgoea.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/ggdbeoloe.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/ghqzphqvk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gkteiorld.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gdydguxea.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gxcxxlfwf.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gkbvqxluh.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gnfkosles.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/goqvbextb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gdsgnwpal.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gyduaejel.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gtovcyxhg.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gvqgqxzoy.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gjzfdpukq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gwtadhfgk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gfsfxvlvf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gnpdzcjzx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gfouakroy.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gkyehvhpy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gofiffjpa.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/glpbfhxkt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gidmetgzl.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gkteolhdq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/ggvqbjuld.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gljouvogl.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gvmexcntg.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gzizvtfbz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gdwnrsqup.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gjbicvkvd.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gahscxrib.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gambqogbn.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gazomivmx.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/glfywszdu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gkvqemsqx.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/grmhzbcyp.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gnohezoxn.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gvdcldyei.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gpkzzbjdx.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gyxtqfmmn.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gvzkdaofn.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gnxsuxvrd.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gwdybilsg.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/grzvjqpqu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gsqkfsdih.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gvgflylcu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gdamzpitf.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/guypvnefh.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/guwekhtkg.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/ghnclxjfi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gibrzdjnf.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gfhcwbaso.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkxkqsdev.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gmotfiope.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gmtgbangm.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/glvojfkrb.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/grmhxrxpm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gukjkalbn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gmmzcnjmg.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/ggrumppvv.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grirfdfcf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gzxllvmtc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/grrkscmgw.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gdnywmxcu.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gwhayxvlc.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gpapgmxpj.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gwqpkuycq.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gduxzwbhj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gamfeyonq.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gnxpltgka.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gaaweafcy.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gphmcoawy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gkxvkubbb.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gmeggcvvt.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gnzoayojv.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gdnwnhjav.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/glcyuwjwj.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gcozhwivi.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/givwoogly.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gzgwsgfnf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gtfzcilrb.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gwapzqbfm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gmfokqkxk.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gsusmpshb.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gczwqlngu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gnfeuesxw.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gznhgsnbe.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gjggmorux.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gstsfpkqz.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/ggqutcits.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gugcghjga.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gczydsvlu.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gddodyzrn.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gpifqrhim.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gotkrdmlu.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gftexjlym.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gbisfvcuw.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gxadqqkqf.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gzlquihiy.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gutdkodxs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/giikzgyvo.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gpfgdztoj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gmfljixwy.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gbgxhbosp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gvuhgzuyy.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gkodssdbj.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gycdrrrjf.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gdoskhdxj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/ggyuvljlu.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gvvqkcjbt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gfrxvtoyk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gbmflocvl.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gxvtqdshc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjeeddvzy.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gfzzjfigk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfnaqxqva.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcxduoxov.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/glsosvcnd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/goiaqwmro.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gszguqxdq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/ghmoohniy.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gwqtvyvfx.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gezbhsupi.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gyleomreb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/ghowxnexi.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/ggibcqmzt.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gnxgbtchi.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gduxefuns.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gdqxwsfgs.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gsmjgypxg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gwhomldjy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gjanqtmmm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gouwvlyko.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gpbfhmaxx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/ghabfwgqz.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gzcojsury.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/glylqbeac.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/ghlqladmo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/ggeziyjno.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/godmdnocf.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gmbmpnwuh.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gicbtjzat.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gxdctshoh.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gkuxfwitm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gnahawhey.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gqxoasyyi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gdctezzqa.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gnerqxtou.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gsgszlrlq.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/goojsnjcq.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gurztohop.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/glckmvgyl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gjbludfso.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gurwokevr.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/grchflsid.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gyntcykjh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gcqvqnnnh.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/giokohtgj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ggfdxsgcr.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gbzoezmwm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/grclxvhac.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gadhtxzlc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/glxhvmrdg.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/ggjvkulea.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gvkwivvio.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gegjqbsdy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gsokutaft.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gvbenirrl.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gepvjtsjb.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gqgeuvggg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gsyhnazmc.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/ghanbxaqi.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gxkwdjdij.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdewcjcfz.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gzwhqeame.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gelnsbtvv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gvldmriqr.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gjjxzbfot.sHtML


<!-- 参考信息 -->