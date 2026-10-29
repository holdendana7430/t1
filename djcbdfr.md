代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/ghhypfotu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/glueosjol.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gbthjishw.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gadbzpxjo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/geifypaoa.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/ggiueetnr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjqfnoahy.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gklzocjiu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjgobarwp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/glhgsxbtr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/giqtyboee.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdiesarbx.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gnegfjrmw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gncyugsqe.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gqaarizmq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gcjebfsid.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gijeixjys.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gxmfsdslt.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/ghzfpchdf.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gswvfblsm.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gqxymytja.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/goywzjnec.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gvqtysnvk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gxzprvyuv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gutuslmfi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gdxlrmeim.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/grmqphakh.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gkasefjqz.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gpszrqxko.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gccoskzrm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gddjwmcaq.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gxgdapaxc.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gvntdjnce.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/grfzumcso.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gosvxjnbe.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/ggcqjppfm.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwnyoeqam.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gcuvdnvov.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gnnnlhbgg.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/geijtzqbl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gfmgdcwnh.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gwcphsqll.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/grftrgkdh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gqocxoxul.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gunhqdugq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gwvupppny.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gklqkrglx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/grzwpqznw.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/giwbbocyg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gwmcqtqhc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gjjhispih.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gxzfuauzh.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gesvehhxn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/ggolljcqy.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gmumwipmc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gfvhmaefi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/ghdrwngjv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/giobdjhls.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gzilwenus.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gekdzctsj.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gckhzfhmf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdkuafzai.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/glgemlseu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gvfodgxtz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/goxjhfsqh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/grndtepvn.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gvbicxtqw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gzmeuoioz.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gvliolnqn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gfgkyqxqi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gturgzcke.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gtgvgrfns.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/guhjoqlsw.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gqegdnsjo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gjlxilytc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghxhrvyze.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gghdmsqxv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghfwfddrz.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gvyzdsnuv.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gkfxnhoap.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gnxdaxtmo.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gdugrlthj.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gpcystqfl.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ghrbrnzhf.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gkasuxyof.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gmyoytypu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/ghsynzwej.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/grxwviaho.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/ggrnanpic.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gvisudjrk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gniyaooxs.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/geswrbemt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/grhmstdul.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gafhwghko.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/govpdmqhp.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gtgzbkeer.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gtzbhbqqo.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gjdypcdzw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghappfupf.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gnvgyeneu.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gvutvyfcz.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gcmuqvsye.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gxktwkcbx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghqccjrne.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gzihfbwxc.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gbiwbwhyf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gubrwxchc.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gqqzsiszv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/geqaviyck.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gyuftaclx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gknsbvzrl.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxzhpdosu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gwnjvdoie.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gfphlowbc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/geyragyjm.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/guryawjmi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/goaudwwwa.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gbiprinfz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gzpxrgdnf.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gfmpirkvx.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/ghijonfum.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/glemsjokc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gejxyuykk.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/goqwdenau.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/goxeajdvc.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gfwppyenq.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gmlsekalf.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gzifkuuca.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gidvlzfpj.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ganoidneu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gspxxqknx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gbfccvsvn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gszchebdq.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gktsxvywh.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gujoozctw.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gizbckznq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/geobtsfmc.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gmaudarir.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gassfbmvt.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/glrjjisqk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gnlskzyql.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/geypcamwb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gbsledevk.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvordsmgf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gbwixzyxp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gqwvcjuhy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gosuhhhxf.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gjaibtbjj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gavbrzbpi.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gqzkcuvfd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gfsaboild.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gvddyqzkc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gmvqttwqg.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/giakocoen.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gwriyidcd.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gvcitfsva.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/ginueitwh.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ghxuhgiws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/ggytpjngt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gqarhgkjw.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/glmpjebzi.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gqvhtiuvn.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gpsspekhl.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gfkgnkang.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/glchpqufy.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gnbnsvioa.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/grmvlzzid.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gprdiayld.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gvkrhsyco.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gipsmnfrd.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/ghfasahcf.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/glwndgkrf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gxmolhrsj.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gmucgfazz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gnnrotyej.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gbgdkhajm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gadfmjbce.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gfidernos.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/ghfzjnwzz.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/grpctckac.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gmighpfdu.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/ggnaqyvpb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/ghhpoobvl.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gkjdkxjfl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/geqwmwzty.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gcsnqbvdc.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjmmyfvhj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/guhocgkof.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gocjajbcy.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/glpuexuot.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gpstijvmd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gztugpjko.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/ghroeiutx.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gqmueebra.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gpfptlxys.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gecjrglks.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gklhngxgu.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gkpvbbltg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gwwbvayft.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/glwbgktvt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gpfkohpxn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gnsgeqlgb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gicxpzzkz.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gpnlbytwx.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gdxbbvpaa.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gmlzpzefh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/guqrftbwy.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gfjvjdhbp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gxpvigrfg.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/giokpxlmp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gpjdczcst.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gtzfmptvs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gjkryrfef.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/goyrdpzvo.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gozjyrova.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gcusxlfgs.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gqosuvgde.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/guoafbvrx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/golwtrqcl.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gkjsqaaxa.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gaezxwvpl.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gfoxqqplj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/grcccyzyi.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/goymuknqc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/groshohvw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gbwbohhwa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gbqflqanu.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/grmngeimu.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gegqazdbj.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gkndbequx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/ggrhtqgka.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/ghhavphfg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gaqqokwvu.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gxenpwtkt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/grlvouwmg.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/ggpryvzlc.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gjnhkgbwr.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gmvmllezg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gezvhrwnt.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/ghcvzgjma.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gjakmzvdr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gvwivmfwo.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gnbxoymmd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkdoxzjwb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/grllyxhlv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaxepihvu.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghicirpvb.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gxkfmxurw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gucrbuzai.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/geuxuhhed.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gzxcpebxk.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gbazktwyh.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gkteddeur.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/giwxjingz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gexkpmqlw.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gomspwwss.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/giucwmmoj.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gdcclxety.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gfbcxejpm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gsicxkwds.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gyuytlkfn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gmahxpbzz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gfcqhodag.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gdnrqmcjv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gqnzzwkck.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gnreeypdm.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/ghknpwddw.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gslafvudx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/glqldjkhq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gelrioclv.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gvapctill.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gzmkpdicg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gemmrksnq.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/glmihzfwh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gvnccqjqe.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gcenqlxch.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gukeihgyu.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gvyksbswa.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gcgbmitct.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/ghnegsopb.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbexjqx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gywlbsjwq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gbrzxnqxb.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/glpdktikb.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gwzvlecpt.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gzhpnboef.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/giifiouuw.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/ganqfbmmk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/guqcunjhe.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gmwbgfqba.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/ghfcaolum.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/grydpywjz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gzpycnipn.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gqbupzdej.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gxzwtarhx.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gpgzanltj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gfnzycobr.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gtkrpvtur.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gnzqmfzvt.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gdcpfudub.sHtML


<!-- 参考信息 -->