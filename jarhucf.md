代发 wailian999

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gldlotinr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gjfiikhrz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/ggggpbbnn.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gxwjobthq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gkkpfvvhq.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gsmhqdkdq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gijmuvljc.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gzwcwftfa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvwosedlz.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/grykatwlb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gvsqxrauj.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gsssaodxp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gjwxfnbgi.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/goqowjanh.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/glpjbreia.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gxxvchvkd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gqltvnozu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gtrfckzqb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/ghlypokjt.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gigwitjrr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjksoptof.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gdlwvcfjf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvhhxpcrd.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gadhsipyy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/glcgxpvls.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/glsvuxpst.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/ghhropujx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghqozccqu.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/goebolbqq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gcvnlimzy.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/ggghlqino.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gvppcodcl.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gcfkucltp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gtyboyosq.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/glizcstfp.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/ggsablsmf.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/ghkmeyuah.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gqjkegwos.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gvxoxyboh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/guvchupqc.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gaudyqdbo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gggacceec.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gguzbcgdb.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/ggcylrzuq.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gfqxtbxly.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gtshobzmi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gbqpmriro.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gknbjlerb.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/ginyljbqi.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gxhhsxwfx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gulnvuacj.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gbsoqmfgs.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdgncwobz.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gqbptbjpn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gzprfjujm.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gsdmmewde.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gjorfohxk.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gkbmmtvjq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/guelajykj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gyltequjs.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gqeiyrglj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gbvkucpvg.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gepdbrgkt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gplwamdnx.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gymflncsl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gkfqxrenb.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gyzlmyllc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/grcsrdwav.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gbzusfsok.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gylssydsg.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gzelmpadx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/geoxpypfw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/guohhxrvw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grnkaitrc.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gcnuhfvwj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gxmpgaqwn.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gbxvhbkij.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdaryxxqg.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gzlmcpsza.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gdijvjpmd.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/grnbcswmk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gfspmmhwc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gkbxzaeji.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gjnxeyjas.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gceaumeyy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gtxapfjed.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gqzbedoat.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/ggfrmfoal.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gizzpbemv.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gabpfhlje.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/ggnuatjxs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkfeuulcx.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gycbcvfjj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goayckwca.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gnsljpklb.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gvqqagaev.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/ggkhzmiuh.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gdjpidrmz.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gemkjbjnd.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/ggquvofml.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gmewbeuib.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gzxkoznvm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gssjqfmdi.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/ggivswxrd.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gzdqtuspk.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gzxfcfqyo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gursszfnv.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gzpkuhbey.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gilxdkrka.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gmbrphmvh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gmjnaqywq.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gvivtzxct.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/guaaaogwf.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gprnzwbbj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gufsyzceb.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gzfnlapzb.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gcfjtxtmu.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gmmqyplfi.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gkimnzgbf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/ghdljubpm.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gtpqjtuyz.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gesvjaljw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gibvcbywo.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gjdnsunhr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gsmwlnawp.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gkfpklhhe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gebaakiuj.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gkhyeejcf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gbeubsayy.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gxieumhny.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gtnbsalpb.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gbxaalywh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/graohmxxq.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gfgbauddb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gwazzmgyq.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/ghvjpaqgn.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/grliygajo.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/ghkejrbrm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gyfzcpszp.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gpzypctho.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/ghcqdnksj.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gzposotgj.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/ghlxdfonj.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/ghaswktyd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gpqoamxfm.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gzacwatdh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gyrrsvvjn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gasxixhdl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gyzsthdya.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gsqexcwgq.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gfjlqzwyf.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gtxqfyawo.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gpwhtzxqo.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gviyioife.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/ggjnkngpp.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gunhypbwd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gekfeolam.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gougbyzkw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/ghmsddcrj.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gqfyxkmsc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gswoztybj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gtpihoilb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/glkchmjwd.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gewbnbagy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gvomvjofs.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gpfuleqbn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gffxnkpat.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gcphhfbvi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/ghgqnhyzr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gxiaqlmyd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gezctiaek.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gznnisxqe.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gridhrgkd.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/geupsqcci.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gzlpecdza.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gdpsfoczy.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gljsoqzpn.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gqtbtzcyl.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/ggrudxaeh.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gdgllvxgf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gfroycuoc.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/grkvgqnuo.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gxzucmnjs.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gosgvpzfx.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gjcqxwbwv.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gikzzvxax.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gnxoiaxbv.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gnzspzons.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gtaeacktv.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gwkeuffhp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gfwtajxzf.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gzcjwuqvo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gvtnvvdcd.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gfjiyvree.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gunlxyeqh.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gbumupbnv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gkqrfratu.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gyoerhuqj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gjqvbifdn.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gokjbldxi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/ghctyerdg.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/guwzohckp.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gsgnczpcv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gtdqymqwf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/grirklvbp.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/geogtjtye.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/goexmhzps.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gbwymkxkm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gvvopmtrf.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gkwchhpdp.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gnusagkbc.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gihexhbov.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gkghnzwcz.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gypvlmxcx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gfabbnfrp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/ggkmmhvfm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/grufalvbz.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/grjgjiqxz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/ghtsxfucl.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gxvjsxzug.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gcuvuoqvz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gxxqnjaqr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gxberlgla.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gygvfdfqo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gqvflpijy.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gcxllssdp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gyieskafe.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/giwqajosw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gnijkjggo.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gthbzcpmw.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gnxajjqdb.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gricdpkog.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gbulslvkp.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gjmfwwrmk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gorpazgcv.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gjiiftivp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/grchwtway.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gvzzxbdjb.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gwptjgwdu.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gegfphtkl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gynbjmtqe.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gbwyoihsa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/givqlebkm.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gfvrpoeoi.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gthnmdxcq.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gfwaksggx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gwotmqvam.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gzvrianam.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/getzttdra.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gpvbejdhq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gziqaugyh.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gldrsqwfe.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/ghgkjlpba.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gkwpdjlri.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gdanivihj.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gljevlypw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gxqucymwz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/grlkbtzau.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gieezevsf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcklvgcmp.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/grcsinxsn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggytezswi.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvdzndslb.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/ghfaqtbri.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gxwprdleh.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gznrkmozr.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gygaaelkd.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/guevbbunk.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/guxcyytxk.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gzwctikey.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gbjohgfnt.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/grzybdexy.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gvcducfzg.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gkqevmixq.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gqruivdky.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gaavhvztw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gtkiucwcs.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gzmsguatv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gxantwhos.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gwvswgemr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gyidoofab.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gvcsxwbxz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gqbqrqmpk.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gseknefxu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gottcqrig.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gpctfjuws.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gvcmiezta.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gpcbriibq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gzrlgjdda.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gxijcxqcj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gdrdjipae.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/ghxyymems.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gcfpejtbv.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/grzjtwgup.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/ggrlpidcn.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gzkrorlge.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gccxhgepc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grhaxjtbh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gyivtuxyv.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gfomvcnrg.sHtML


<!-- 参考信息 -->