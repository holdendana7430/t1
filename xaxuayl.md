代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gxlxuexno.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gatzyjugo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxngwdyyf.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedhfchgz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glgsortgv.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdrgjbexq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghyzreast.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvltswog.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gbnqvoujq.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gbespzuir.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzzdomam.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvbpgcet.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknptnsrs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gqacgzmwi.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/glkdfarhh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjtyjumm.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gobedbwwa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gogkasych.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhoabbvv.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvtfqemy.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gunrzvnwn.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gueuifzbf.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gryrpxuay.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gacbmtiev.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfkosppq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjfxjaqk.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gervvwpas.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulfjvpop.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gssqnjzej.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gshesgtuz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/ggmwbebln.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmaliqoc.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcjonipf.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/glvadaomf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gmnzvlkeh.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gaguigcmw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxynleeiz.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpafuubp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gnbrjlzcf.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gftutvdvz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydjbybsl.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklrcveni.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grqijxzgp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/ggamaasti.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gkicyomda.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/ghwzhqbad.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvjcbwsp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoqcqviq.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/grhmslohp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsrigvfm.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/glztgbhyj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuuulvip.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzwaamgy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkepzahzz.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/glixsavik.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcrfilso.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmcbgiyg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnqbdizoy.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/goudbfoao.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjaqnmpsj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gafkrmyhi.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfzlfnpag.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrlywacd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkrwlsga.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtyoacyo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhdxbmgc.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gpipwzqnn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvtyntwj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxqqglnh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gjyrjmgca.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuocdlsi.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxxztqpef.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/ghqabipsh.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/glurcaans.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gmoofjqqe.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmphwyqy.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuhmjeud.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvdpjbjdg.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/grcjscajw.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gdqnjhyjj.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gsyeksnsd.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfcdqsbl.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gquzebfnn.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbxnaavui.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gaggejhez.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxhmwkox.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyftpqzyo.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gllawyfuq.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbtimxasn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnmubfmr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwfgvnzx.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcqitqsc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmkzepuqc.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghwizmqbm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghrxfvxeu.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grdjkjdci.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqjcbcak.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvgkjwyh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/glyvglqul.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gwieteqyo.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gstvmdvlr.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsxcfejv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcspqbbe.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gkmdvyhwr.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gukbfojeb.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpurzhplz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghrmbcddh.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrxthjey.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gouiqhqxu.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlqhpzrt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtemeyee.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflgrdpci.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmybuhapw.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvaljzfxi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxkicuah.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gkupmzwvd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrbmaltl.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gmazuhgfl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbzdwafb.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoarvcva.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfolltdeu.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gujovspqq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/giaueysfy.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtptftgj.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gudyorwie.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gsilztyep.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkkymzffk.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcrpztvk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmfaldxa.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gsdwbhogl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlfoildn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkquoqztb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrgnfwes.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsqoduotq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gtyobvqlr.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnxnhluv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gseohyrau.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsawnpxa.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwlrnpil.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtahcxqll.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/geyqfesrg.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gruiuioci.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/guglrmtrw.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgnnhfhj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvbzdpzai.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gxicxpwjw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvhrrazom.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gguzccxhb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrnbptju.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gmgpbmvcz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvywgfpuv.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gszyazrnz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/glurlppef.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjxtfxfqw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtimwynw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjfjywkn.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gapwexsgy.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gjfuriqbo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzsiobbr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gembacqgb.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ghjchgbuu.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/glvzuohsk.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gdigxjqqs.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaafkhtw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/goohmmihy.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/goneqxfrf.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/geaxgumwy.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvurjmwfx.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gsbebyeuw.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwyhbppf.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbctzleq.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhogqvrt.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdoorujj.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gggxisghk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpokentea.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gihwumlbi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsnfpzoa.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gzfrrwebs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvrqxujq.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/guikyclfq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxievuax.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gldmyrohd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gncggqkck.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gbkxjfjuy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gogieeyek.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gnybuumrz.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcukpmpnf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gnqhtgqac.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzafmcihv.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpepqwlu.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwuckxzq.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gfclblwxd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gbulzfngc.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gdweqbnqi.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtonhezjx.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/groqavqyu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxthkauc.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdpuetodw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gquccieda.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gvfhmazvv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gmxwnnrht.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbdkhogk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gnnjacejv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaqcqfcs.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gmniftbbb.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbngghzsn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnssygtx.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/glzscymjs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuovrvev.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gpamsalam.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxntgbmjz.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwukgbvir.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwkldtwn.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gnmkshuyd.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/glfilubsf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtztaxwdf.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqkcazet.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grszltrej.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjsmrymr.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/giffpqnlo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpatuxld.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gnrxohoch.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gtcsikkhk.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ghpptbnpw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gisaxauyy.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/glmcvpvyg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkpldytai.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghonqrkfx.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gnalzgalu.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkuwvgup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gesbxxxll.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/garjawooj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gputhrmwk.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnogvaawi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gfntcsabl.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsdkdcry.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/ghnwhseby.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gykqdhgjn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuictjyc.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gqepqvgbk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyfogwxrp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrpsenoc.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbtpjsod.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnmtrtkvq.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfximvlpz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxcgundya.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdtxjgmnq.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqdzoqdc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvppqdvwy.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnknhpkr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gwaqklexk.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/glvwfkguk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfkfyyaa.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdamglcqe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbomiyhpd.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gogxqbhol.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gxcytcjuj.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/glablhurv.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/galuqltgu.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gwddirxgy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gswstviss.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gubvyaxyq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ggijmiopl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/glhtvgppk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepclbuia.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/guokzigaz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gntctfpfo.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gndlqdpxo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/goartnkyb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcememkxv.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnokfmnf.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gigimnbek.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gkobtesvv.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfvelqhv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzogkubnm.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gwdbmwcgt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvouxczi.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmqxlzlxn.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkwvpcjj.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/geegtsyru.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ggzzftrwd.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gqsxcoair.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gozpglawi.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/govufvmir.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/ghmceqhar.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gewjamsry.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gsvthwwoj.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepvugpys.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ggmvlohgq.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gqevumjex.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmitgurtx.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gdzwbjsao.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiuhrllm.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdhkxobj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaufznts.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gswcrqwqn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gklaxozun.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gymncidef.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gjblakvnb.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaydujhk.sHtML


<!-- 参考信息 -->