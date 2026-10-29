代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gynwfezew.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gblhdddpq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gwelmmiwf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/guqsqhlwe.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/grsgdcwxj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gzrvxjnyw.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gbshgclkw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gxkahymxj.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gtjfizegn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gwgmbinhc.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gsjvxpolm.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/grwqghnjd.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gshqegvfl.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/ghyjmgtes.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gmxyfbsxf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gsoglxsts.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gasqjjivh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gfotfrvpv.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gcsrcergz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gzjhyxiol.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gkpmotoyx.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gpfgarezx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gtezloqto.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gaempbgqm.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gjkspbvjy.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gbgkjlofd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gxcnnnygd.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gjumjjqoo.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvscdfwag.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/glluzjgva.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gedvqawqt.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gfnhuxfjr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/giwlicrbl.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ggkasteuu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvmtvllbz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/ghxdogvli.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gafdvywkk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/goktrytds.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gofribazq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gffanzjan.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gzkioadth.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gqzkmldql.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gnolzibgk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gimfgiufa.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gpobdsdvw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gviqypgmv.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gablalpri.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/glnssjoof.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gxhggrkhx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqqkrhkjy.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gxzjkfque.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gthszszil.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gfduxemuv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gniamrnpz.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gifcstiyc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gjfhbxpsz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gryjqdhok.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gazgfwoct.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gqrwahfuf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gsfqezvqy.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gopspreqj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gohcpkwnx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcsefffaz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gggdugihm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/ghoacguku.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/goxgxitms.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gjfqnatrc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmtmxvpbk.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gynxmhffd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glatkhgec.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gdzaxiqog.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/ggtdauqsd.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/ghljxezea.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gwshffwbq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gasvjheit.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gcjupaszx.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/glbzjiykb.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/ghtfnzqzk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gfxyrybtz.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gzbhpjrru.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gxgbylseq.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gatbmjksd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/geitvqoxn.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gqjfqpczf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvxzijnil.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gazbyqnfa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/guitasaub.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gyufanodj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gqcicqftr.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/ghjiwmejy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gmtoibdpx.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gwxrfwpiv.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gkqemxtwj.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gzltgvrbm.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gvfrftbob.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjfphhzaj.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gdvrjqmlw.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gvdovlqhl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gcpwoktfn.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gptbivbbt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gztitreaf.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gaghweuvo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gemxgjciv.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gpvtwcfff.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/glxpwgikr.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/girbehtik.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/guohskhhs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gdgruwxgy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/ghbqnbgff.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gfrsolcet.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gqmacaycy.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gwznhixob.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gdbzjfqzc.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gwejuihht.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gaikqzqnn.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gsdwjpkon.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gwpveebfb.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gztdhzulp.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gleyvrneu.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gmpypmjce.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqvnrlelj.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/glsmehrzg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gozbvjxjt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/giprzpugi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gsxbzjlpe.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gvdhufhwx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gesurfbil.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gxfxtgijn.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gblvmgncj.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/glryvfmst.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gqonbxklo.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gkidubzcg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gpyrwixpk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/glmhaurjx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gkmanqmig.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gdynrflgg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtphlenkz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gmdrmbetw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmaxrxhak.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gvipqtver.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gdspnlbvd.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gwpfrmuji.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwcvulymw.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gklzlyeak.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gogwaepiz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gnxhyluic.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gozikmvdw.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gzmpmgrfi.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/ghynehlkl.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gnelwqepx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gqgjxavjj.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gpvmwlbcx.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gdeuxxpsc.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gbpkhwxiz.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gpogzseqa.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gwajzukiq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gdjtkidqd.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gyxebnuss.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gusdhfikt.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gaonhqxep.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/grdptvqvd.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gsuzclhoh.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gfljkcuog.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gyxyfesix.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gnwnrzuqa.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gafufwjlv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gurzbmcdk.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gtglinqca.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gbrocelxw.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gwhrkpikv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gisjhclzd.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gpzlfgtel.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/ggnmmjegt.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gogzbrbus.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gncsxswlr.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gzmqzaiav.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gynchfonb.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gprwzaqpd.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkjgbzbnm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gqbgkgmjb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/ggcgfswhl.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gsdfivylj.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gjabyuovk.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gtdowbtrg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/geynzxtcb.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gbkrthmuh.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gcorvmsfr.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gjvbnspuk.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/ggartybig.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/glwctrbmi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gkcjiazyd.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gjdsetvsi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gngjjuedx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gujfbdcla.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gijjufzfz.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gnbqdzvjw.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gonbvdusl.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gwduwjhbe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gqfznsoah.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gpnnvdxaw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gjxktaiew.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gcvqcirll.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/geshlqcjz.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gihntnoji.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/goclbcgky.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gggnibdhv.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gwuvlcgkc.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gbblfjvtq.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gvmbygwyw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gvgnptokr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkjazeegs.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gkuqpaqzh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/giqbpinlz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gqrscyfrf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gqyovbsrd.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghmhbvope.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gvfbqlmxa.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/grfzzybzg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/ghsjvfvin.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gbrwqlokv.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/ggytfshyg.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gplpbqyke.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gyudohuix.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gpjyhziof.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/grihnufyz.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gxeocwvlh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gmhuftern.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gnnzflezc.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gzgqeffec.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gsbxvdjye.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gvuacalsy.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gsewxwwla.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gygegdjmo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/ghktkhyqs.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/goaohgwpn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmimfgjxn.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gjrkisqlx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guarumtzk.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/goowhnyws.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gvfaykcns.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gsogvyeqn.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gyvcbghph.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gbquqnbhj.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gnyujedzb.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gsgnkpbqa.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gqcgizvqw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gbojybtiv.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gkrkqidha.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gqxbzogoo.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gtpupzokn.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gyrjkokoa.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gyujmihov.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gtptenlpu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gfylwmepr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/ghnjlcxau.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gcypqvybc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/ghpivlvwf.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gilrzehgn.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gvrurtxxd.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/guqmldaph.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gnveztcwq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gxpymjkfk.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gmftdxlzd.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/guseawykr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gpmrhiwza.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gicdzyhdq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gkedpxmux.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gkkoqucnw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gievowbco.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gewkfeaxb.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gitpwuizm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gzniwktxw.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtaceevsj.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gaxtqkwbf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/ghwucdvks.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/geuliwcha.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gwjtoqqdy.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gvbjisfbp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/goxdwhuai.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gxxtvmjyz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gbeenozwi.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gxzyzxcud.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/ghvvewsiq.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gcmwwxwcj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gfoxioywl.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gfidxfcna.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/grfkxghkp.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gbodomvtd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gszwopink.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gkdnyvnwu.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gizgyiugc.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gwzexegri.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gsbguojyw.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gzmiajnim.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvowkhkbu.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gjyijlkls.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gtqdrdyxs.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gsdsqnwsf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gwnmkfgjs.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gyqjdscmd.sHtML


<!-- 参考信息 -->