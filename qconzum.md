代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghckgzhxk.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gsabegfwn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpkgmvxa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjuftuyi.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtqolkxq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdshhbab.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gishsoesd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsblxvymn.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gmsbcuelz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gytidtsig.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjhgrucb.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gsiupqhyk.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gacgnpmuz.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggebrlceo.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcqjoxnl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktqnsflp.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gfujcjqoq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmadjyhq.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gqzbfkijf.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/goymizmjh.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gprqbguax.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gxoxbeail.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdwbdkmo.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gurrohnxx.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzylrhumv.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gndwwqhlb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/giizucxdl.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gdfyqurao.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvltkpvm.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/ggotoumbf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhnedaop.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gwjnadori.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/geaqwkxzv.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsnqpezd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtonpvvfe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixymfjxi.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gdskquhwn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvjfpaqf.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gvjxwtgrn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/giukchdxo.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlvxfdey.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gjexlkflv.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfbuvnau.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gxnfofjpz.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/ghavckqqi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmgqvlwu.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/grshxdupl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gafparnce.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gprbvxxil.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjyuukqf.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gibjxwqbg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdwvngbb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/geovkteuj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcrythgut.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyljrzgk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gntjwjjwk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gnjbzybnr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjehrgfsv.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdqygixj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggugnxfaz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmebxiknq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gieosvshq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwkxbifq.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gklsvtzbo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gsfzbcgar.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gyegrvafr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gknevmlsv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdglzymo.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgmuqhsu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gypauscyl.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gruldiujt.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtidomxp.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gdndyhhfv.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gwzyjinua.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gemuobysu.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grrsynybt.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrmeuojg.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gcexyqgeq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/ggwrwqkqw.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gdfrlxvfe.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gswwbokoe.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gktljefvd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggckkkvpm.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhqyvspd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsixgtnlu.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ggujqgdkz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gbegnwmms.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemricrug.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfefbyoe.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopvshezy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqxrvhda.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwshkioa.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsizlvge.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcjrsdca.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgmytdmi.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/giwwwtukl.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gxshmyghr.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwldwkcdm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpqexmvl.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnnxzpyx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmfeztzf.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsblbzhw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gehgnaytd.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrnyhukh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlxxlayy.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwrbohmw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehehvghy.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gifzvheti.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/goekplegv.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/geagjqvsr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqrqfzvk.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/goixeupfq.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdvvksop.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrazsefr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwanwrrfz.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpetbomn.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmqpxelf.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gjpidbdpw.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbdgudyy.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyznfhxgq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gffdpjmqb.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvbzroee.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/goygwgajs.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gdwjzukgo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsrhqngi.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gyrcvoyvr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejoqpemi.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkzvzrmm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gdxrztlwf.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gapjyekwm.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gdywtdypf.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gttnysogt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/glmzhluex.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjmifefy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabzsxfrp.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggfxstpoh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyssynwz.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoiricvu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtsefhife.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gnedlsxfe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gxqjggbki.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzixksyx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuqrttdf.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gdqvmbvxi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gfxrjvlpt.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcrwibza.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/glkhjkont.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/glnspimrm.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzojavsbi.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfqpxwhu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gganfhvlm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/glybrwmji.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwbaluhc.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gutqirmue.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/givbulowj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjabdhldk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbqxmrfd.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gmkylgnis.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqicuqxmf.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgwxqreb.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/grvcnzlyr.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyfsqigy.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/guavsxgyz.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gkgznmezt.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmnkftpp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkscqmdz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjeiizic.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbpmnvcn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggpycgjny.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawdlcsmc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gphkbuhdt.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjdkrojqm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gfvatwxxf.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujrqwuhp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grcnpefnf.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/grtqpvoti.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjvaewkr.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawcxnwrc.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxguhsry.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gipjpkavc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/giigkrudt.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giqefvgtf.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgvwjzwy.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gzahxyoed.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/goamjryjd.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmhspoxda.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gxzyzehkn.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gmstyafhc.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gvkvlgcld.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guhqxrtwu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gazcpigpa.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gghqmwprl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxkxzsgfh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqltxajwc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gdochrrhp.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgjrspzx.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gchlefhtr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/goqzwqjhx.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gsimjkjpx.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwfxonrt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gpmtqxlgb.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grtgmbhhe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gstvouqyx.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gngsuhtkj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/glvlkobxs.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcozztsu.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gbrtkzchf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/giimnwwbw.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixvcpovi.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gpvmhqqoj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnletimbc.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhqhfrwo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzkljzgs.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gqnztpdjw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/givkuluuo.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzctzxdq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqlhomms.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwktnanl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzakbxnr.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gdrnonkzo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcsdmhiy.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gkktsvgpq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gapemxltp.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gewwewdqo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwkkubaj.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gozlqvcvk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gjfynuzvq.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gatwlmcgy.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gclaqypae.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/glgsayvjc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdrfdxblq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdbtgffh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdpcktdd.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggmrqqzng.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeyllwwt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grdlpauxg.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gferpmosz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggtpgnmcq.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnacdgtg.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfwaudyo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmjuuukt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gloxlnluu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gapeoimbj.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvprjwlrq.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gzpkkxhku.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdxfwytu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gjzoilvwd.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqpoxhzr.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gyrpegcvs.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwqgurlm.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gmqcsghko.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdjnecsf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcjqbalv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gaopyjqtw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gfismmwom.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkhzblhy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gyxxxhxsq.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/grjvgsfup.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gnwrvpolj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givdpzbcc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gitzhvkpd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gycunxlfr.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmflctda.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvgutlze.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grspnmnqv.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/giojdxkvr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/giihlujni.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/grubimlln.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljhmkqqu.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gajtzzpbm.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmhnpiud.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gqfbdtlzl.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukfqzpwx.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauyssbqg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcifbtte.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gksreptal.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrnzboqq.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkfyzmcb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqvaisbd.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gcobilvvm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusvltzfo.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/glprlnzzi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgileeqg.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdfwqzcu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gpdqktzeh.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaocxbzao.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxcitjlj.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gddkabgvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwklctzfv.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmeoenxne.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihfpkwqy.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gqjpabljx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkivipiy.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiysbrbb.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxhcxinez.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvcnjior.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpasgljlx.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gehzuuvqr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkruzhcl.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gwjaasmcd.sHtML


<!-- 参考信息 -->