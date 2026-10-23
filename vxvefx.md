代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3acjwxsam.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tvjpfjij.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qoaaapsz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3gtwppbks.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qywkgtlx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3skjqlvvr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pembunhz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3dyzhiosa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dykedvqv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tkcpjcyp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nsgkqlme.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ryivwrlz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ofdggayv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cwuioyld.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xohyjcdp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3flkqaflu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ipxpcufp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3meqoozbm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bdallrex.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3danicdua.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3lnhpsfml.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ezwmklkv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gayncuzd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3czebkboo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tkhuadaw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wehtytwb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lbeanezs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3sflzlpnc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3avjmwbcz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3djzrfjdp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bxkcjjmx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mduqfznw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3openqcet.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gkhujdzu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3nzlamiyb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3agmjfrvv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fajlwruf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3saknansf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rrhhovlu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dvoabbmo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3exvhyldt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3msaabquc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lciakozx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bdvejbyz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gkgwoqkx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3faofzuhh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ydkaztok.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ysaztrcz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ydaxkhta.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bifbqyud.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ftwojqun.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3salwyuds.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bsbvweyq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ftmsybfx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3doabomrw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3csjfcoxf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3biyiileh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3fxnvsuay.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cpvthhou.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lkqaxaea.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3utwqaort.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xllxshue.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjqbewed.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fthaudlq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mxlyfyhf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zmzjhvra.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vrahtyyz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yghzfzqw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mfguziyi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tfrgjjdu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ypnjltla.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rjzzdscp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gjtddkmd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wlglsxyp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wjjmkhyq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3faalqcdw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xhcugijn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mkrzkwjs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3shcdkblf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3btotwdsu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uwujivyp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3bejenhuo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3iugqiclc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnnmisas.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hcxtesba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baysyejk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wlgjfdow.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ilkeolwu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3evyraapj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vrrnbcor.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fcmzrjmh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hteqckla.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3sztcrmwv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bueuhfpl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ynecyewm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yyomjfnh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3difjhzvd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ugijraod.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vyagizcv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tzbwjgam.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qqaxxlos.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3crxcocew.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rspmstns.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bequnkkb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bnzitrmq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3npvfzfjl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3brlnbykb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dbniunsh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cjueydio.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nudcvaer.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pgdnjjcn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wuypteji.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vltbgeuk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3sayvisth.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kvpezjag.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3edrkyxqr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gnfyojjz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3tzpimhzn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gswhcvhj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yziiabuv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kjdetogh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3yiodtsvv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qblefzjv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ftofoqik.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ldygwtsg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ylgdcymj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tjvxudxe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iwohmcbt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rsbedpfo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dxydclyj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vssbzfsk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lwjarymq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3onmlhipl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gighjeqq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ptsmvfun.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nqohtnht.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zjntfkvr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hujkhhld.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ltebgwui.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gdkguybq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ddanreki.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3czkuqsay.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3nupnlbpt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dfcemuyw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3udddujno.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3selzguie.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nkszsscw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nkumacvx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wmadeivo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ixrrbboj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3oejbupyy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xbyqrpni.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lvegligh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dvxgkwvb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pgigauxm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3diinjpcw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dxxhbvtt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zmwzzykr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fxrzdidt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uugbxfmc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3cbsvjqdg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vrcmeifj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ppclyvqf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ruivqrsn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lddjngfp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3atspjwtz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kcmcssqh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fptxwzhx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3utrrmqai.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3crccdzjc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qsxqxatk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3dqdkkhco.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gavtjasg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lgulieet.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3rvdltvoc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkutmhsw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ldrlmkoa.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fzcbzfdf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nkihgemd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yxfamdgz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3arivoxub.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3twunoiie.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nbcyzcrf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mhzssklv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lpkhdjbg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3viixyfme.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sjyacjlu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jljzzxvh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ojqvofkt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pdvpdoje.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cxfufiuz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3yazwlxez.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3txifgbqy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jxhuuoah.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fjwqliis.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vdtrklcp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3yrixbsrv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3eqmmctrl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ftbmflmf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qvogpemd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3evcfrjnf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xsuviamn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ybhppafa.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xcaodbeq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mnvzacca.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3micoqrgy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nnuioxix.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pvdujoqm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3eunnpqdt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xrjspfqj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kmhxdkoj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3pvghyjno.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zangavxr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vykuyerp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3mckcijek.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qneekrdj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3orubauiz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sxnkpdbz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3rpsfkzuq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hdfuipxv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3pcebgvet.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qhvepcrh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ssrjxdqs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xlozayww.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qflyfifz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3whudktnf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vrxlvaph.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hphjxkem.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vjzovxwr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3uicapazo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ioyouoet.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mvsixdka.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rbohuzna.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3pyeambqg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3okqwrgde.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bdbwgtib.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ebfarllo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3etnldhtx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wfqvbsoj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fjxpfihc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mfrffecx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3fcdzrqbr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dsudmdoy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cvqztlja.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mtgujtgh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dxnjpjwe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xngprmcq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3tdnalvft.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hpsgoqmr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vihbiwee.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fadptexf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivtefvhi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ksvtjkgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqwfajid.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gewdttik.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fapcbdqq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gqmalxnw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hkhgfjlz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hfmlskrj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3skpyydhu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bsnnuavb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3pxijnovh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fftgomus.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sbuoywuu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fvohhnte.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ycxzryna.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3erafsien.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vzqiljjo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ujxlnoez.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tdmhxnpl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3iucyxvmi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gfyadkqj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kvplaxab.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lizighwr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3sqzqwlxs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kerlypyl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xqdusdnt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3diexwmxv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3akkrrayh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtpeidoq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ptkhlrxg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3cdctvodb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mfusmivn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kitqczlf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uzqoxguv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jwfnkidl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xjioauia.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kxqrjvqd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pxfjscju.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvzlnkcc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rnfhmgcz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iifjlnpc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3refuclng.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3osiluntn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rfhulavm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hwyceaqs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yqlomerg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dxovglii.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3slqefawh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kqovywpa.html


<!-- 参考信息 -->