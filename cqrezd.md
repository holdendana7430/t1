代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uojxtcjz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3bradjmre.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ajkqnutf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3czqyxpbe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cazngehk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3arjwgzlv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3bvihflos.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cwplavea.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ygdheocz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fbdtqtbz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3rftrshah.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bdbghjan.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3uxykzora.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zmczrwqa.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mztwfebz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3gisdqkjm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qyjdfxwq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mylrinit.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3guigevhp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mickonqw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gltbaugb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3pxsdrtqz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3acchjeux.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wrxsjxkj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqzliwhv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bmpbfpqy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kcdhjypy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3edjbrqen.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kasyvhwu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kuwzhljr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gkgrfllp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vfthcvyn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ygrqsaun.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bhmoffly.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yjbpnwrc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pjmelvkm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3icuxbxva.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3camyikif.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hsoduevi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kkkkheyk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lfqrecno.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3eerysqfb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3emqicpdk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3asxxoixf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ytqzwyaz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldlesoqv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xhdxydyu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3czonqdgl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ojfzzoiv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wqsggzdj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3djpsqsvd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qjtvyafu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3fmcyxtji.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xiltphtl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lawlombt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tbzoppke.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3exsisrhv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vruoumkz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bwkfpmmv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jdwkaxij.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jsahisfe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3yylsndga.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nuzoodxc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mxiyczre.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tvarfmzu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3foqntpau.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3lekzfieh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3leaytpdx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pikdujsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrkridpa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hsewygws.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rvfusdsz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xgwgcbyq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ykxbigaa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ydqmegqm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwzmggay.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ohftyydb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3phofiyry.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bcrodwnf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3adxescfo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gzqyxvkv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zaqmzygr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkkjwiui.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3iiitxogu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uzzpwyyp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jrxyiqds.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lsyzmtfk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vgopbacw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uluzhrrp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ogurvinb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ohggbbce.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3oagiqcff.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nrwgerbq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vqwgxsza.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wvuczthe.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3shhvqzwi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dfqbtaki.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3tnbbzsbz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zykcezhn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qmpyqjpt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qlxwnfcz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3texxlruy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3peinqszt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ekpoaxex.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fsnrnhyi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pjbsooed.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zrboopgf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ithxnlzr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvqrugwm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ttzyfwrt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ahoozdoi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jqllyrri.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvejceat.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wmacqfab.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3megwjfde.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tfrksltk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3iuswwkzo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jfhuoazj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gshtnjcn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3alxrfoac.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kfqlerds.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yltovjed.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ddyfvxsc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bhjkouxa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3gebxmzmt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ocbapcip.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3aspkfhoe.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3gsujlebl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3imnpmacr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qgdgbxpf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zasyslha.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3llurtuxp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ebxxbytd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mettbctq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wjcfddbg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnbetafj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3itsixwfp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wfvbecki.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uejzzmes.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vqmqgffu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ehksaklz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ikhlwjzb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wpqhrcvt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dpptiwyu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wvkirtpo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tczbikdn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3knfwwxjb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ixxjavzd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pqgvxjhu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3uhqhehyg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3orqcrjib.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3fapjdqmg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yenncwki.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nmagyyha.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3pjrktown.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fxjcunzf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yyherawh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jzfklwvh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3uaihjxgo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xpyryukm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3dtufthou.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3yufbcozx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3miseireg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pvfypgaf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ratjaqvu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3luodnarm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3aycpjmkt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rpoegikq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xazmevxd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3eekjryev.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uasesoqh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wrhljfvn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vqoowqrn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lztzfiwa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tzxseaya.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jgkvtlnv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qddrhhmo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ecwmzzkv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3cixmcbog.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3aisiajxa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3cxyxifus.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nskmxykc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zoiwbuak.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qarunewf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hicmxzft.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3tdfltuiz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vterurho.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ptysqkwo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3howabkzo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hnvimlyu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ocakqvxc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xxreozhf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ooglfjqf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cpqsmppi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fmakkbwp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qrwydoaf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3adivwxel.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lzvzvuvl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nzstpujq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tondohrc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gasapakm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hhcerind.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tkkyqxpa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mmocvfzv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3mzofpcbq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jjelfxym.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pxozhqar.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3icmobzuq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fniticjh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3yqoxqgup.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3mwpjdbtf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3umikuhjl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hufkgkga.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rcuaoqfb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3jzwbxxhy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cpftyzmw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mlombgfn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3amqprdec.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jghdlkby.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vbpeexcf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3heuwcmrl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ujzhsduz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qyrtqxgx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pyxsogry.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qwjplvex.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qiqiuqoi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rmbnmubo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lpinfifx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rrhvrhul.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3tnnmnmoi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3urfngciw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nhhwiykc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3yshfdrlq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zhoaxaey.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ccjneqgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krlpowud.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wfxgfniy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfbvbwil.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mdtyulxr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3mjetggbx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnaemfye.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3alvtrqtb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3eimpbmdh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3maeprwue.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3agivwrek.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bqjpknwv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wglubmhu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ijvuxksd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gyntpqig.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zgncyvaj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jblpwlfk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3iniviqre.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hpewseti.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3cekrdigr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3doplynng.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rtiazvpz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tprexvhy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dnffppfs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3stnwxnzu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3juyudiwr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tjhvwghh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ldtelmor.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ryrzfifs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wbqhmwmc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ictdbvyw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wxuxxzjz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lkudhwcc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jrqjcfap.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qohzoxah.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qtwxgtbn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zckwmqpr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zzyvmjog.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ygevfhdd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gjqxqblu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3irvxoabx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3epmrkuxx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3lqdtdoqq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mwkaqjez.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bfseiahh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3giulcqdz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ziayvsfj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yrqrluyn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wunioojo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qtssidsj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3axyjcyyh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uwncqkel.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nirazgly.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3sterylvr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3cfkerzxk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3klwxdfgh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ucqmocdg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3iykzorim.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3duobwcre.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wkujslgk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ewiofjmx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3irfjjytr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eixztgzi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwcqtxjd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ueyoqnct.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xqedspbq.html


<!-- 参考信息 -->