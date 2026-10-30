代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gtphryfjd.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gzpfeswly.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/guugfatoo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/glwdzucah.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gwopaktne.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqnyuwbqi.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gvizhmvsl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gqpwxoath.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gaavjqhab.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gfjvwjjfa.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gtozomkys.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gmpfmnnwh.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gviypxvua.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gkxrkpgmh.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gyoqwuiwv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gwuwftswz.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gluqofhbc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/giqahmtlq.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/goohddnhb.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gtxwanqzi.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/glgnmycmg.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gskfovejr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/glmupgcis.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/girksggpx.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gkqpequki.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/ghvwunpyk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gsfdeiyhx.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/goqpugjnf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsxrhsgra.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gjucqjetr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gwuwjlskf.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gvyrkhnna.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gsdsmxdfm.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gwxicnvqm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gfdtoromk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gpdxaabsu.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gsqqlhwop.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/guoyoevxq.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/goneazayr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gvqzphgaz.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gugrkotlr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gndccbrmb.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gdsxbxfru.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gwwbkjore.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/goglbzazp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gehhkswwx.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gxxsiubma.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gjifgrbhy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/goxqycleg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gupbteqma.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gxpptfdjp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gugzrppuj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gjwkfnigg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjpcjwkrv.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gqeoxsusi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gipgsfazu.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gnrcvngrz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gebewvjuu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/ghoygqcpf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gkjrboufh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gznirkedm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gfeivsvoh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grtnlsghk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqxdfqzki.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gjxnydbhb.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gdpjmglbs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gjaezrsym.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggbjpcwxb.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/grrhrioxs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtdyxvcmz.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/ggfpowzpx.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gyamcizai.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gbpramtkr.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gpvkktoar.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gaqlpinsr.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gdmdiiggp.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gmyxjwmng.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gztbyeaoo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/geelosevl.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gnjaodlfj.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gedbthrxb.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gbnaznshj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/glyfxxwdz.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gpklvemit.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/geulzgifh.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/golihglbg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gekwnbyer.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqmukaqyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gxedvxkka.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gladeuhrh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gkrseqljx.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gvnxxmiqb.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gktqoxhlv.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gpleoeabz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gexlfhpki.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gkutkbtte.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gegiizoev.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gogcgwobd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gcnuukjgk.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gvjtgpfkh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/grthioijj.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gmhstspcb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gvaziqorp.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gaiafeynb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gzjwdtnbx.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gvphtcifr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/geaaiuvkx.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gthaqspfl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gmswlrpbh.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/giinofsmv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gpqjlydhd.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gnwhzlabr.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gnzzpxgro.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gryhlfkrd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gvlzdiups.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gntrpsxoc.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gxfgyjqst.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gifugmhto.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gbenquhpd.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gjfxxeewd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gnfnqxjll.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/goanrablb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/ggsjplqqz.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gsnygsofe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gvjfukepv.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gjvxwvqpt.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gbtcagjsf.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gswthztvu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gltoveopm.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gafgyznvq.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gepjcjnnn.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/grtlmuwsx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gyjipjbys.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gohhugcoc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gskowlbga.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gxyfxzmhb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gtawvwjjd.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gqmjeglbp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/grndrtvvg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gbisrafnv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gdtrqfqaj.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gghwmaidz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gsplnkaji.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gtablnyrj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gewqdcukx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gimtimihf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/glodcnynv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gkjrubfjf.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gdcuwnxmu.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gwmvefnyo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gvhfvteos.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gvfjkkrro.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gpowunijr.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gwbgyfvke.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gfobzkvla.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gpgtdurtp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/groguwkjg.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gipabokss.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gormnapti.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gutbjbelp.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gwiikdgwz.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gwzyjdbkv.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gejlgxvps.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/ghcvgflwe.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gimaczsbr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gmzozbqnp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gmhnfvcoa.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/ghdxnuoid.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/guvfbjmeb.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/glrcpaljd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gxqisfjlv.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gpgohjhyn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/ghbebbpqt.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gpqzsrzwv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gptstmsnw.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gsefjwryj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gaoosiiaf.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gngvnkjsl.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gleivrxoc.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gbgobdlsn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gpmatcwpf.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/ggkpuuwfk.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/giqtfnfbt.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/ghljxdvjj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gvobtuzeg.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gkyidgqlw.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gkwzidxiv.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gmuxqllkm.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gagrddmxs.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gnnsylbba.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/giptdjshj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gzourailg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gmsultrco.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/grxmfiema.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gvthexykz.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/ghvgauicc.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gwwttthnu.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gjvgzwzel.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/glnkhjprj.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gmkrwiyol.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gyeshycuv.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/guheyhvvl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/grghovfbp.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gfqnivhlr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gztbdypgo.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/glzbuhxsg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gluchypjm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/glxcppnav.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gxchuprda.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gxlmwwngh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/ghvfvtzpf.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gutadlaxn.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gvuqvghxn.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/ghopvdoup.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gywxxboqg.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/grqtovbcz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gqbdunrdv.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/guuaxxczl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gkogjobiq.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gycgklqnp.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gdlbpuepd.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gicpgpgxp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gdcuaatho.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gdoocbxrg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gleebzlpa.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gpbinsvpc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/ghlqtarpq.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gvbmddmig.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gbqceelrq.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gzdoooaeq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/geydkibmw.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gbxcjwdkj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gjsewpfgj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/ghefxjoej.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/grefqiuxr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzxsavemb.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gxiikyyhb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggwqspjpf.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsfifostw.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/girylakjr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gjrbsbqih.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gkansgxnw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gmvmbzuml.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gzbmrwwhf.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gghyzbcjg.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gcgxbtdcw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gpeloacow.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/giwgadqcy.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gsgarqeyl.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gkgysezqm.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/ggrzjneqw.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gjbocanih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gddgqhoye.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gxrhxqick.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gslmxsdxo.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gqjpwbtjw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gtabeajzd.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gwiaydmdv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gxxuqkljt.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gbbzmkbnm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gjckzkmlg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gmjyjjxjn.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/groajqbkv.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gxeioxpqe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gamwahbxx.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/geojdgzvb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gzwbsbtlv.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gmsvivjym.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gfgiwlyxr.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gareevang.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gvvquielx.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gxvymvgyi.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gmjfhxryd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gvcqurysw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gllzcrzma.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gjziilvdi.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/guyqwyxga.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gvjpnvlfn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gwjtguyrn.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/ghcvbwuxd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gjnabpsam.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gibaeczfp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/glbobvlaq.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/guklmfvhk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gfvceoyqc.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gxyqmidcu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gwwgfyeoh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/glflumyqa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gsigkhzva.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gbugpvqev.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/glyzfbqmn.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gourjggqv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/glkdgpbxx.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gafcppgcw.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gccupsuml.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/goypwoemo.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gsiwgxiyb.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gnphlmabq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gnykuwcvv.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gtllmxzlb.sHtML


<!-- 参考信息 -->