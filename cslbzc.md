代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zuqcwdnc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jvuzdead.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3eeagcqdf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3esgbnpim.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yptzpolx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kmrgekto.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ewujnfpz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wvstnjkb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3deueiqib.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jwpeowfj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qsnvpkhr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jshfvmii.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dqhhsddw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3goczwifr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uujruuya.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3apbxfspw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wpxwlrjk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3nmblqnpl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3agexuwuj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lqufqigx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vmyolxbn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hwjvqfjx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3crbcupsq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vxsbrrrr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3nbtiuoev.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jjoutfvu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3oogyirak.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3uunnluim.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ejjhggjl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gzrhgftf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3pfxsqhhp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jcsxexrd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3iunykeig.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ukfmslzk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3qfqziwap.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tpmyrucs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3eltupcwn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3eninlkyk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3yfkamred.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3eydnlahd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3tmmqyjfc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3fbxkhmzp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3josiaqbr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3rxbwsrmh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3foihsnli.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3dosjnzsq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fynnoqql.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xcvxukgv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3djqqkbse.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ornhoxby.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mzwqayjc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3utczkkrl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rzqvfbwi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zpgzpqiq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3uchenzqw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3akjuupov.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ukscajpc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ubzhknhr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wfvvjmjs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ollinqqn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yabgcudc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uvxtovhz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zkllaran.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qilsohae.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wojxmcsb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kemegebs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dwpegrzb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dmuadaaj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3npxedftc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtirnqot.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wryywmmj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fahjbuir.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3twbdydse.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3agwlnslt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3aqkotmaj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3uyrgxwlu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3aoiylwzy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3prdmmswc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tdokzupp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rvaimjxf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ogvtmcqz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nfywgxfj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3doyxeghx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnpdzuim.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vhpqxiyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgpeobim.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vgeyvjrj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rpiacuit.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ohfujvtd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3koxvlghz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ntwqxfbl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3jkuhrjiz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pqupqljn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3njebrbpx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3svrsjqes.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yoptukxx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3plmziqvn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ioikuffj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjdrpik.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zhasdzlx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3neoaqamw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ubsjvvlb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mkaulnqd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mtnzmfvc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lmjgmavg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ycknmeei.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ipbofteu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gjegwxyb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fwicegev.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3zoacsypr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3stgvrifw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3abadnkox.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vmznpfjb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ehxtldei.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ynbqwzpm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xawcuesx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xylaraon.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nlagtxuk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ikrdckhx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lbzpntth.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3yvhwvhxj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gtwbpvez.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cwqdgkca.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ukkfcmko.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3icryjito.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wyjwapzb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3znalxjtw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3myrsjvqk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3liyjhzxc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rpbocaif.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tqtaizhn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nkskfdyh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wtmljjqp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3njcwbntz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nipqaqrp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iuumekag.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3baawshth.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hxexurng.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hrcsmfbi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jsxipzef.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3czqexldl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3dabqkshy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3szmflyrk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3evfrjxol.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tvfllala.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3doofaoho.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mkqeonyp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mocgithj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3sxrbgxhi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jerullcu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3akqumtjp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tfjsbmvj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ezoxqihg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ekhqsbpf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwcfoxzk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mwvtmoqp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nvvsdyjl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3orkxjwky.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3esevmkgn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pmrrlpwe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3lokwfuts.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3deoagjiv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rbmroxsm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3exiczxdd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vtfbkwob.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fcbddnex.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ewbvptmg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mjuroflu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jxcmkspb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ogkfbajp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mmbgnbmg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hzmyxkig.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fjbtkabw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mzsyjdrc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nxnwzkis.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3iakcycfy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3osvtydwo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3aierhgxa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rllszubd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3sekzvcuc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3hcgzuvnf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3inscoaom.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3upxhitrp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3kgyedvfv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lxhmymbh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3txfluuke.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3skfmcrxu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3spdajxce.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mcrrxocf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gpyhddvi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vwzqulxt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bhxjllnu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3lgifgkel.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cnftzrea.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lhwinbal.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3scehvurx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fbcqcqgq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dhnesysp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qrggkltg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zjfvtvqd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3psfuffdj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3aezeklcy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vndvmgun.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tkxqpkjt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zptegvos.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptremnsu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3oaleibld.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3flpcdobt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jwhrpfpp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uulnjmny.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rvstyqrw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fpekbdxu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kiwelyzb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qulikjeu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3yqnrvrwe.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ycatfduj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3motnayuf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ekfcbzux.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3jjxsijsq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dknjllrt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3epgvmzyu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hxuzfjkn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rbozkvoz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3cuuehopz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3uypnymzm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wwmwyhyd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fzdfknxy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3usznkkgk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3shiaelyc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3epotknnk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3usbcyabe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hidaulvx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xlgahwzz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cpgvcxvu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pdmekrds.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fwyutnaj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jjlsqmab.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jfaeoslq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vrlcibac.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3astwyolb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3nspbpiky.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3plqojgvm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3emfukqoy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3anwnmhtt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vwehojiu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vmkyzcbt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ycbhlpdj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tknsplof.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ageisszx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ednzlqtx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3snfvxeop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnlgenrp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qszyagyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejtlxzkg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xtpizban.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3aayyjpaz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuuldroh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vqbaghjd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nbmtyquy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3buvzcsej.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3newxuaux.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3spavtpum.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kycnkxxq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vtvontfn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjpcnod.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3puuotfdw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nwepoyzf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zxmqotpd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yvsxeofb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3uabfrdhx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bzfbippc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3nepgcogd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vuxnihqi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pcbthjfm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3inxaxjdf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kvbicbzi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wpkpecca.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lozebfjp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qrrxlcve.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3idubtuev.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tkqaycxa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fmlrdcvc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dmcbfnac.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iqtxsapm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wcsjdjvw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pohhlzda.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hlrnyisr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3iurtssap.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hxdlqiez.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kybfymjt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kmolphmc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3alxlybln.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fwljmdhy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rumjmfoq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jufumrxw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3drfdvhhl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dbvrszhq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3saryfxbr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bdkixctz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dstbucys.html


<!-- 参考信息 -->