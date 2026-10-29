代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gonvticon.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gdwgtbxss.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gqreugclk.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gduxmbrye.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gllxlgcap.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gmjkqeglf.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gfhppaysh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/glrnaidya.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gkbiasqfl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gepfljodj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gyukoipar.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gtbheqciq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnuzviijw.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/goqczfjze.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmrmaqqll.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/ggvzfntax.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvgmbkdis.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gmlkpvsqw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gfbhwjpjc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcsfslkuh.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gmerapgmw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gwmdrdtcl.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gdrrbasqf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/goqqexvyo.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gfvvifugp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gwjlnlgcv.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gcmjjlasj.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gwupsxulq.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gvddzktrv.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gxfniihbq.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gndrlirdp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gkkqyfhvq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gibyctmcj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/ghcxotieo.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/geqxrymcy.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/ghxmmwoxf.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gmhvlulpc.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gszqdskqg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gnsphsvpw.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gihgreqxq.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gzqcnuezq.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/guhshfssa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gogenxwgx.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gnbwvmqiz.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/grfhwfpbq.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gkaxcffsh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gqasiqafl.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/guliwlhce.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/ghtopkogg.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gwhxoufrp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gdgtlloxd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gqxdfoebz.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gkqmnlgvf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/ggyoxbzmb.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gyheydhoh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/ggfspvkdb.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gainykvrk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/guthffxgy.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gkcynkdlx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/goltrmaej.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/galptwcrg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gimbkmnwu.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gxvreitnw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gjseaelmq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gnkbfezxh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnnpldlpz.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gyhaybqvx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gborddlng.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gmuamnnzt.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gxxfwvhqa.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gmxjyrvab.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gldebljil.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/geezwrbpu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gptuuowyb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gfqiubbfk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ghapxxptr.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gsfbutvtk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gzwbgbbfp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grrhyxhcb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/guveikaoi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gofzfsyzh.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gcnlxsywg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/ggnkxlben.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gifuavaap.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gicukbqzz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gizpifyxj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gbkibcbws.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gvukrreym.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gcfwguafw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gpitbdqgz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gcvlvrwqs.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gwbcsjthp.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gygyfplqq.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gfpwsxlws.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/goiqcwaqb.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/grrywaual.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/ghqdmpvmv.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gulsmmmbc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gxenxudwv.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gumbmfwhw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gnwfrbhak.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gxntenszz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/guhssjovt.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gygcmwdgl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gyuzbqvci.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gshcddmya.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gxdjlbkdc.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gtisclmsn.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gjyifphky.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gkvfljkko.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gcsnzlyyo.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gnmufbemz.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gsbjoyoce.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdqsixzvw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gipdsuiqp.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gdasoktle.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/goepygtsg.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/giigmqycn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gibhbszat.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxdprexmz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gwciiljin.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gouxnrovs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gftoshhpx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gqzdmoynp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/ghfzgejrx.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gmftspese.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/guffyfarn.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gfbtyxxbz.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gsmslxsnm.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gvcejypsd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gwryfmkwp.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gahorczxk.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gaviaesef.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gtetghngq.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/grlbhqnwb.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/geifepuyj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gayiwhipg.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gfzjtuibs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzexayqbz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/ginrrwuvp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gnfvlkqew.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/geupyxpgt.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/ghtbpvfhj.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/genjjpwbr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gtfmuipge.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gryaqzbdw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gjliedyqf.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gcqtnopgt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/grprazixx.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gnyaufrjz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gepnxveov.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gqthoxpzx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gtdyrdcpn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/ghgrwybsw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gafylrlrf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gpacvbwmv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gyjusqjev.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gzpysrmok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gxpvkvdum.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gkbtqszyt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gbiayasyh.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gvzwrcpqa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gjmkdobpo.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gheyivwzi.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gobytzuhb.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gntpdhwxa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gagxfkbnn.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gatatyydo.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gbbjiigfp.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/grexsgqsp.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gcrwqzrhx.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gonlijmnf.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gjznbjato.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gqqyaegmg.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gyzrzyyvw.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gfmiywnvd.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gztoqfqtg.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gdmclqmnd.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/giwvyuprb.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gczesblen.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gtlliffke.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/guxfnjdrj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/geavjoefw.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gsbrzpdwm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/ggkxtgbhm.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gvdwdxssf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gssnqxybs.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gwmcghhde.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/ggkmnsjaf.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/glwuwcofl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqkuxwovv.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gjbowizcr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/ghzavkekt.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gkrriymul.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/galohbuoi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gptjkrzoq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gyjjrnhhc.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gomdanjgy.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gkoopbygq.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gsltqtmwa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gevsnwuzk.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gbjtfdvrj.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gqjfblgqm.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/goiwytgmj.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gywovbcmx.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/geimcsymy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/glglqrovt.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gnxxuhhdc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gzontosmz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gcrcejjod.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gtcainaze.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/grhwitsnz.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gnjmmaist.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gbhbipprj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gtmextrke.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gzsxiyyyx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gdqgvpngy.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/graarqach.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gbptxctof.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gdptkltok.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gxayiloet.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gklrggqfh.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/grztjdyan.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gumtgfeka.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gthwixapu.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gvqkofvpe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/guvjvidbr.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gcpqttkch.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/getssjjzk.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gxsscfjst.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gqdfkmpqc.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdmpsxdno.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gkrgaziem.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/ggmatrnlh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gxhfkeaxy.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/grrvaqtch.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gphhzhena.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gmdxkvdmn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gyltrkcmd.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gnfbjxqjl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/ghlegxnrt.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/galojkuci.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gaminlwdf.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gsejssmyq.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gshjkfliz.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gfjrdhymq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/ggthflovi.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gixweggcm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gjzhxtibm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gqeesaoic.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gwxrwyrjc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gehvyrxsw.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gmtttgvwd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gocitgviz.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gcdwtsjks.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gcjjfvvzw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gynnsrgsf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gcboyeiyn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gyupgeoza.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gabjktamq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/ggsubzwkj.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gojmbrgpk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gyghipnuj.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gpxlqsxaz.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gcpohctlb.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gemhxndyq.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gkijrxzgs.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gyidmovhe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/goiyqjhaw.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gruywnomk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gzhazjazc.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gzvzwnfhb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/glkcsdmzt.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gaubhkgug.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gaewpkiuk.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gaqfvjepl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gfncensrd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/ghxxzqgwb.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gxlrrcgtw.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gmaujfejl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/guedtsfhi.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gxlryxrmz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gqazeozas.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gzcujwqih.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gnsjiegml.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/glvgleypu.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gcelxtxqs.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/geautucje.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gxbikuvgh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/goljdnsrk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/galljlyuu.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/glvoziaau.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gagccogwg.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gcutxiltu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gkkuhjrpy.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gmtbfuyow.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gwgxegjoe.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gwuniuoup.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gvstuenqa.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gvzkxcoqc.sHtML


<!-- 参考信息 -->