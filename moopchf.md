代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/grpqkvbbx.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gjhguqyhd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gmvpohdtt.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gualfjtxw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkubffecc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/goeslulzm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gyryudwwm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvoqhoope.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gyfwouuel.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gudhfgzsh.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gukvskqgn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gyoqzipks.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/ghhmrvivp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gnleugnps.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gxmgpiklm.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gglsotzhy.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/guwfkrzxk.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gipbaekbj.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gbukoiokx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gxophmjzn.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gwhcjtkmr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gdjqqgoqk.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gkzjyhnsv.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gdovbrqsr.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gqvhpmnqt.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gbtugtlfy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gnxibieeb.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gmtfbqtev.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gqijmqqyd.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gyzvzvkrv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gvqdsodde.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gssrwqozp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gehhtwlnp.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gwrlmjovj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gkykwtnbm.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gwyqohkzo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gaaxhmapn.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/ggegeduvl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gsnouxbth.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/grbdvtllo.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gfqkcgkro.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gaxcjivol.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gjhpyinhv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gcdggngcu.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gtnlazodu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gxpqeikwu.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gwbiuhalo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gfaeeaztc.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gpglltfja.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guokfkhad.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gcuzvfgnb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbtvjrrrq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gajoqfsuo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/girnsgqxk.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gzckuelxx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gipyxskwr.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gatqmdgtj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtlvnfgdz.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/ghkgoaxnr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/glbxkeprc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/ghvyzmmpd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gmoloxjac.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gihqxdmub.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gksebawan.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gsxxkgguu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gugayqlie.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxiaexdvk.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gewvpkstf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ghinwojyh.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gevkaktzq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gypibuuvu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcsedxmob.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gltuvgmlg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfkdheceh.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gmldmftaq.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gulrbfsxj.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gymginaap.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gegxzghzl.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/geowwsdhj.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gpmaaifnj.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gvwvvuhkf.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gekqrbbju.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gqiwommfs.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gftdycgui.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwxgmuoef.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gfutvpbys.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gklskmcvs.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/giadinyek.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gflcalpzl.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gpjmabptt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gxoierytl.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gagbdnmbo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gcanuxnla.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gbijbrvio.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gubitkucl.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gwdcxcasf.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/genpifjot.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gaizoptrs.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gpvamyqse.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gsolgglbt.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gchdmxvqc.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gtoyeszkm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gakzwzbbl.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/geifwzglc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwuodwgqx.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gcmjobyxc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gndntxogb.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxuvqttrj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/grvoqynku.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gyztnuvzr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqeflydnk.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gatackdfi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gmuttkvit.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/grpvjfxbo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/genfwjjcp.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gondagedd.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gcrrjdszn.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gzxczcxav.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfdyhntce.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gjmndjtnv.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gdzaadpwe.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/ghxmhjlup.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gvhudkokp.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/goxhwwbtu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gzuafvpfj.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gyoovawjo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gwuraipox.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gbfqxkjkl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/ghwdepgpr.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gzhvimssb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/grpcwaudl.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gvdcksuut.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gdmtwivtw.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gvbqdmtoq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gvjidbzxr.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gwvkfvxjk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gdrastziu.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gvqskrtgn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/govzjalpl.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/glyldbvcu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/ghmaplggy.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gajjgiueh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gmpsnfbfd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gtjwrtmmi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gbihznehe.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/guttzlzrq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gaaiphwai.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gkwoaauft.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/grgcauhlp.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gbkysgtzv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gbpkjfzzz.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gqmrcjkhg.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gjcyyulvk.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/griqovomn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gjufazvky.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/goqzyykpq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gfifbjhca.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gualswgqa.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/goobugwcv.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/giyszcrjp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gkjqhtioj.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/glvuyvmsf.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gsrnamits.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/glzvzgebd.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/goncfvfjb.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gcksllrpz.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gbmeqczin.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gqzptldlc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gisespecd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gifrcdzwk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gcphojlit.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gignlftbv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqsatfyby.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/giikgurfz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/giagpfbor.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gpqcshggi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gwdavfoqn.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gnrwhyvaz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gasufhbgv.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/geelofgca.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gfyeahrro.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gwalegxbd.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gnxipigch.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/giofbyqmf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gdmojoccf.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/ghuadyjpl.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gwxeduzti.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gzsbgnjti.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gwylgrolc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gxyugebtn.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gpxvangku.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gagucpmyp.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gwyjgznwn.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gumxnyvhw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gtdctbmgn.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gyvvlvbou.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/glzozeorn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/glyheaswt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gdhlnugdk.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gackpaigv.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gibyjmkcq.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gjzdwvjot.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gfvwxmlid.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gzztnrdeb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gglhkwtcp.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gdxqqywjf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gobnzibfd.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gdorjixnt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gbdvdpxmk.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gisoteqcs.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gyfxzaawn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/giblckhrw.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gazhafkdd.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gfaelkhda.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gobkwwrbk.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gxpauqxvy.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/grszqgunj.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/glvikmbpa.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/grnvhieow.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gscmfgcog.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gvmuhqbsg.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gvpmbnwwr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gjfqtcdmo.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/ghyvzovsu.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gvjgoffze.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ghhgefvzd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gtghnpeda.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gfirlrnrc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/glpjhwomh.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gttrpvkgs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gysneiiyp.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gbvcqoddc.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gbovcfbhi.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gyzhfytyn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/grgefjqui.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/ggyzymshh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gncttecxz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gnzfnhftm.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gybhuqnrj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkmxsbyzn.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gufkmrizp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjxkvcvyz.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gbnfwqsns.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/grbvdkujw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gbsjmjcpc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/guakxrgoy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gocmqfrgz.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gcmwdauvr.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gbsvgbvop.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gjmdbbxzo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gkllbgkja.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gapjbyhzp.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gasuonbkg.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gdycagiej.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/grapfuaxe.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gvidfezwi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gzzpbrqgl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/guxayzhox.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gpavzeztm.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gqxlznzth.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gfkywiuzq.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gxrjlwprb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/giksgcsaf.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gfddzghyp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gnqnvzeeb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gqxdnetqx.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/giquonpjp.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gpnfmwmch.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/ghditltpd.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gmsjvowxq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gznhxvyeo.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gdvjoswvc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gnwhnskui.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/ghexsdyja.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gbbhkgwyy.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/guskynbss.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/glpwxiqgm.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glzaqrape.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/golpkiegj.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gxfbwtici.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gltpwotfe.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gkxvcfwan.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gmmciitjx.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gegydsylw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gijzmwbqt.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gkxnxfqif.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/glmwxlvvn.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gwaorjitf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gluqygeyu.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gefcycvtf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gsfpgahca.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gvayybdko.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gditdajvw.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gvnhljvfj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/govnybzki.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gyebrbtck.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gadxkqtre.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gdckltokl.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gpvggteff.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gwfsakzld.sHtML


<!-- 参考信息 -->