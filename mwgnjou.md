代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gtuohdixs.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gceaxxjmb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/glkxxguet.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gmaypqieq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gfqwehglc.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gwsqfylmx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gjdpxjlxo.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gfdkdyksv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gsqembjzr.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gahnivdwv.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gsozfoqhk.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gewhvgspe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gvoucjmly.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/giwqaipjn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/ghmstztlx.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/ghofzlbwd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gjgawhnbh.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gximxcclf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvbrmzipt.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/ghxgvwozw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gvuopadsg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gkdfirdru.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gncgnknne.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gaidhmktq.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gallqtmcu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/grlkxrwvn.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gheughmff.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gjrvhketj.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/ggrlixxoh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gpwrcwemw.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gqyvpkjuu.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gjjintbxi.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/ghvsuofhj.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gvppipqqy.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gwnignrgy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/ghupucunc.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gfgjunmsr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gleyjvsdj.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gszdekmfg.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gxrskjvpx.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gpiouztxp.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gtayrefii.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/guvqoinyy.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gteggdcdj.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gwncwlzzg.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/goolcvnyw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gssdlotvq.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gqwdmwcvv.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gluktbsuw.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gdlbnegwy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gqtskcyuq.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gbreipjak.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gypadypau.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gmmrptsty.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnttdgoxd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/ghviqmwqd.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/ggqtcwlky.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/ghipwepkg.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gssenxwgo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gaeofhajd.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gkqewhaqt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gqcyxoayi.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/ghsnoynfk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gopjcadct.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gssgmlgyz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtdfikues.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gfcmblhhu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghnmipsyj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/glnavmxfi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvsekqnjg.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/glevydskm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/grtnecqjr.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gdnhrqogx.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcpklwklf.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gjwzgvubc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gditvzuyx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/glkjtqgrc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gaiddopty.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gqpoeywda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gxvujeuez.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gsnfgndcw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gwuuxkyri.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/ghihvjhgz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gqihyshak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gmwaxbcjx.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gpnhnomrc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gfeqhzbey.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsdhzgmhw.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gmcutjcio.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnoxidwpg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gnbtfigol.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gzhrkvzxv.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/ghkelnkvo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gdiclymzj.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/guicueiai.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gjnbxvbzy.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/goatuksmf.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gfooildjk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gcuiselsf.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gcgryvuff.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gevkohplh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gxmujgoce.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gfrmgpdps.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gtewdzefc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gjgbzqqsd.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gwphbkmrt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gvngtlmtw.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gbmnsvfmb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggxuieuqi.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/ghxtezbwf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/giukeojyv.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/geqtnwlty.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gvurqfwtn.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gcqphubes.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ghshbfohj.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gzszfrrhg.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gsgqkpnao.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gthuvknkr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gvxiyonyu.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gfdhbewji.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsayivxjq.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gwhbwvyox.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gzarpokja.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gjuhyurvs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gcymjnfjs.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gsuzwibrl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ggkqlpdfr.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gshovtqsi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gpyyeazuh.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gyglqttiq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtvkmdkpc.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gopjlhvdr.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gdzkqxgxz.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gcoiagtpp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gofygbeaz.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gfpzfqdry.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gxpxisaxn.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gjnmwxday.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gxjinnqbb.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/guowobtts.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/grxwaawsq.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gbfbbksjw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gjzgvmdrq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gjqwfukjz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gibvracxm.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gdncqgooz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gtcumzxim.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gqflekzla.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gtjbzletg.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gwkbvdvtb.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gtrmoqrzu.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/grrjtreyc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gjfvjaokz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/glbuwpgam.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/ggidqsxem.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gxipnxfbj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/glkqwlgbu.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gyyncboqg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gdzybjpfy.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/goibpnspc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gxunmvnba.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gewdbpmzr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gtszwlhtm.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gcgbviscw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gitxayupn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gxpyrddqh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gcwydxaqn.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gkkwgtreg.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gsxwhjtdg.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gejkuqsij.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gchexqrcr.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gynmxcpui.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gqlhimznu.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/geityrgzn.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gqqqjudbu.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gnktmqyjv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gmqdosxwg.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gaidwadmo.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/godlxrjmw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqgdniljx.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gpqjetpzi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gpbgyfnmk.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/geyjpylwr.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gfcxfuunw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gybvpnehd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gcbpldmtq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gmvzhuvxp.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/grmgjxpfn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/goiiqotns.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gtcujuftd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gagcjwdxj.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gadktebef.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gbldykyfd.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gvjzutnav.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gblmddfsv.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gptslssur.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gndrtxvcv.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gpblxxpoy.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/goijybdmr.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gzgdwehxw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/grohfgmvu.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gbxlbobna.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwyhwxbxd.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gtcefhesc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/guyosphez.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gzihnzpqb.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gowcynkcs.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gudclszpf.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gycpjszrb.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/grhlsdaqz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/glozdgczx.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gmivfpipg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gpxbjpqmu.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/ganljdjpp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gafrwovcr.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gwjlcfshh.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gxhaccbao.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gvkxgobmq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gsqvhqzch.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/glygkibmb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gffodztok.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gssmytjxl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gepoqehlv.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/grvuhfdgj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gicmeirhm.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gzaeroldo.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/goourkrps.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gturkdwus.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/grqpnmkys.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gjobkibtb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gudbhzbfz.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gacwvwxih.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/ggfyefvwh.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gyxcyyira.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gdczuiiur.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gloyzanfn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gesyojydy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gppnvjlho.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gtniudsla.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gvajhqvka.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gnaqmpyup.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gjydibuko.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gptiqrcny.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/ghtcbqmwp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gfrrbzzpj.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gaxxiyjuz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gjykrlthb.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gicjyrrui.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gruyolkll.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/ghmuaeotz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gjylajahz.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gmedmqkah.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gayqkqgds.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/geikrlcrt.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gzaugxcdc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggriwexek.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gyhxyrguf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyhrkkqht.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gkztxpbba.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gnsqrgfbz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gynyauacu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/ggmwmnmzr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gzzomrpsd.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/ggvnwkzmv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gdkdyjlko.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gktynnytd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gpjhncyah.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gftxevoej.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzogjdziv.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/glzouixwh.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gloxefgte.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gbdnmmeir.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/grwknqhop.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gdgysdgin.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/guzjgtter.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gtmqweaok.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gglgzzupn.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gpwrajznp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gbzssaxrp.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcbxwixgg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gsmkhcyra.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gjnuzpbjx.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gjcderuye.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gaargflll.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gpqhrhcdx.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/guslbylli.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gaupqkizw.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gvseeekqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gvhubghym.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gkrozlzfy.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gykhpscgp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/geestanqr.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gfxgdcpap.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gxhvtruhe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gdvuqgptb.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gngvzjbcy.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gdmzneujk.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gieyvyqgm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gcookdrua.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gpyvzaaev.sHtML


<!-- 参考信息 -->