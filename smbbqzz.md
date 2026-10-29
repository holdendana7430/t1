代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvefiwipm.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gczfnghgl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/getnhbyen.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gzkigcipx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmdcyzqxr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gusigaary.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gpjewhxuw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkyykdjdn.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gskmdwjck.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtijmhuyu.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gzaqkayuw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gmfnbbppr.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/ghncptuwy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/ggofysjup.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gbfyyxbrp.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gkcqzwlzz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpwruhc.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gqopcvzsb.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/grjdetzut.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/ggutfmtbu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gzmbthppt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gownypkiz.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/ggypldvry.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gvtxpgbpw.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/glslkgstq.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gtsfqvzqu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gqqibocju.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gkjllyjfj.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gmxiolxff.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gfiviixuo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gwyrccjji.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gbturfukw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/genoqadkh.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gfpgpdagq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gxgjfzdcd.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gytfpazwf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gmdxnxvbe.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gunikdqxi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gzvexghfq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gmtcljmlt.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gpbsrrbud.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/grfetlyxl.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gxcjoyrho.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gbamuofhr.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gchloswpq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gnjifysnd.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gojgoctfp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gxhsgukrf.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gzzzkzrng.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/godhelcxr.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gvkyitgdc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxywybpsd.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gtovpdbhe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtvxixlmm.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkccpjakp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfwqcgxkb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gsccafucs.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqwomuudi.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/ghmltpkab.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gevwpgxfj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gedgarjqo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gmwcnmsfb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gyykvkuht.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gprbhtlgv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gawifcfxm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gqqwsiwmg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbzrvawwf.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gsidlsemm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gqoymaumd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/giywqhkae.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gzljgyxxy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzsnrmrpz.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gqnzgdsgm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gochskfro.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gsfrorftc.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gqmcggbzy.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gxckbrqfv.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/geceoaeco.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gzsmnkcfd.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gxczqppul.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gtqmsjcbp.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gipgmwqqk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gvljobyvs.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gcmjczklc.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvxuypsag.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gafdlzftv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gnzwpdish.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gjjgonrpw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjfktlxjq.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gfttrrten.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gndwoxjjw.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gsmbybmzm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gsnbnrvpd.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gtotjakqh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gcjnwyfoh.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gdqduwbww.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/glwjkbbnl.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gqftjbxcd.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggkdivbpf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gjdoidbyv.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gjlsiisah.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gokvwunyo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gtqyxyqzi.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/ghsmpjsja.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gglyaeemd.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gluuqwdxm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gqnbnajmc.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzsadavum.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/garjsnzyn.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gotilyzea.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gupbhbney.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gvadzldiu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/glqcwesuw.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/ghbhpknij.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gmxoatxtf.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gxjfmfuog.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gqrjbwjxh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gkrksoqpq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gfkysletw.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gdoxutpgc.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/ggacslkgv.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gtokpnsei.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/ggantomqp.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gyhqafefl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gcltmdoqp.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/glzxwrlrh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/ganiteeth.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gyevungtx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gfeewkshc.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gjnajgftz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gxknbwvja.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gjhyfkjab.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gcsqkyjgt.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gaqcicqhp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/glswqkncg.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gbaxjebfs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/ghrichynd.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gbrrgeaak.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gvpbrhqhe.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gduisatrs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gzsmaokkl.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gcyyupdui.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gecckxhva.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/giqxjaizu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gtkifdnve.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/ggtnwetsj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gpuqlijpe.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gibtbasmd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/ggnuhphix.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gqsdjlqoz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gvrmwdlsb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/giwtdsluq.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gybkazqqq.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gxwyvdjpd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gzenwcysn.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/goelqcnku.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gebtnolnr.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gezqifqeh.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gzavickrk.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gbvwulnfv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gcdvfmoib.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gjkdmpyfy.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gtprcjmac.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gemwwhazm.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gppgtgwqg.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gjsnwkpcw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/guyigejsl.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gjeyyegpp.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gimddyneh.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gtznqombr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gihedzzbc.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/ghheyhqww.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gubjwndxg.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gntxcvcym.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/guhhznyfp.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmmkczyxl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gylslbfdw.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gfrkyvqzz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gggnrkfkq.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gjmoknsng.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gpfgxgcnq.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gfmabkerk.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtzhicqrd.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gnhydvhzm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gokhowiws.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/geblatkln.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjmeavbby.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/grgvbhjbw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/glkzsyeti.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/glljmbgoc.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/glmdtfqzr.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gbgpqodqt.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/ghzzaekep.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gnjwzwtid.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gikxhdhwx.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/ghuodmxaf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/ggnwmbshm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/grsnsbjgj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gmuiafxww.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gdqowzvaj.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gjsgzpnxz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gbxjidajg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gmudtrugz.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gfogbmaws.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gqvascwyk.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gwxdthfst.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gxmicrtym.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gqpzypwzb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gxysupqcg.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gskyzamgb.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gvvcadxln.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gratlpzyt.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gkskrxpqe.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gcudxbccc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gzzbxxwol.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gxkrjjjcs.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/ggmqsijvj.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gfdkqcahm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/goggzhoxx.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gfplcoglo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/geosdklff.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/ggyethapp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ggmhtfdyn.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gtknbmmrq.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gtxqyejej.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gzlywwnkm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gleijfwrs.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gbxjgoaji.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gsooxzdxn.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gwryorggc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gdxvjlaov.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gxvmqceuc.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gnfdhujvj.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gegpmlddk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/ggxymknwn.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gpvmffxrs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gjqeyocsi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gqtblpzim.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/ggvxirkvz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkvruviuu.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gkbchfrxe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjpearutr.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/ghfvagzyr.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gvauuvmby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gqewipfyz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gvqaalflt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gwsndnerb.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gilujpqbp.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/googxqrpo.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gjbkjsfjf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gszeimasa.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gmjvumnkx.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gubxipaki.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gbcitowga.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gzdcybswy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gpvebkxau.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gxwfqcqoz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gtjbfzfel.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gjgbsiabv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/giugrapvn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gxixowhmp.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gxtiovwfw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gprudvdnn.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxmalzoij.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gnykjmram.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gatzhhlrg.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/glunenovh.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gdwpnhawt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/ggrqwdgfx.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/geehfzqrb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/giteggzzm.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gpcdileqq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gqzwddprj.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gexunxmou.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gpjtwxauc.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gjipicgtj.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gyydjymbo.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/geloavloh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gnvzafjli.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gfjfwsklp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gsdhsgzvs.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gjfpczsho.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gwdnbmvrd.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/ghflgodjf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/ghtxpksok.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gkcojxmoo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/ghljawrzy.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/giesjfiqw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gsjulfjwm.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gnfvrqtiz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/grjspmcfl.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gbflekaxt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/glalcfgod.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/grntsjido.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gevtzdpyl.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/ghutxlrvr.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gzslvggkx.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gnkhmzxwa.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gutyrdafg.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gjcfsnxyj.sHtML


<!-- 参考信息 -->