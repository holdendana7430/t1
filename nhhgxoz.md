代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpwggqxki.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gakdsmohp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/geugjdzwb.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/guepytmit.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspotqwdx.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcfndkoc.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gfuciyfqt.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gptpihmxg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkffrpsb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/golskhlsw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnlhgout.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyrglybo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gireaxiep.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/ggdibfqya.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grxdhmgpq.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwouqfeb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gggtyckfg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gdigxrewv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gwopwfpcb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gunakkehx.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/grigkgiwc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gwdhzqzdh.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjlulxas.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gtnnyjtlk.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtowtzql.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbjkqcch.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkigtdupf.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqqegrdo.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxtakyww.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyldgkgoy.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/grsyrsalg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbqrevsh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/giijsemos.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjuvfzjw.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuswwkps.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtyrjyis.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqywwjrxl.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gepbvkmbp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgygzqho.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/guaesnzuq.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgxwtaaj.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyhvellx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gpusclazk.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gmkbjfuph.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqcebkvjv.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/guoyjsydy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwlbsfjk.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/grwfhbnij.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfdtyvkd.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gvextehld.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gexszfnda.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmoprmtm.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gavahyizo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsvfxwbj.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikeiqgpd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiggglan.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gbrfuodmc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybqxqfop.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvywwfowc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gssowtnbp.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/ghitiibxv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gduehyqnn.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gswufrbxp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtuvwbpx.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgnscdse.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grhdzzqge.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxuassvy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwlnswhn.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gexqlsknf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhhsnjuv.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjyzjjcz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/grswodnig.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gmrximtyx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnucmwwug.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxdjyzii.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/glysoybrd.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gpaulaycw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwbxlxgg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniuqfkpk.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gdiofshmm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gouygsziy.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/ghoxmhrdg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjfnbjcz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gircmtpgp.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglxugist.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpmmkzggw.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gtcevegzm.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/geryhanbo.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gdhogvhcl.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmlchzmi.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gxritggqh.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/giycklhux.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gwkyoflfr.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaqsnhvp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwxbmcmg.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/giqilmqvf.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvhqxmcr.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gozgzmeer.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/glompszas.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/geqwzgqvq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgginnfw.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grttmlxyh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gsubudssg.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/ggnqmfmnh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzayyfcpz.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gopktoqgy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gevptrmiq.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeusiftf.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgwgfvwi.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/giirajztd.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gappizcbd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhopamdb.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpwxsdbm.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/genuqpwpe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glmwwdhan.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdqjkzdm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzjmdqkr.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gwjhbbebv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcqfcxsl.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxprbctix.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrfiuxxm.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gubzqkbiw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtztttagf.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gaedfauwl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwcvggekg.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/giriaozst.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqpagixg.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/grzvdyqhd.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzksikky.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghllpecku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gchwfnpip.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqwkfwzwl.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllogzuwl.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfxecgow.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkpmjzby.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/geliehozi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpboezerh.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxudcleog.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsncpaboi.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/guoneirrb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegalvujj.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/guniqvtju.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gmmapfdsm.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/glgdtjmtb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gseqsdpfd.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfgtwupl.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gurozjdfw.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gplvkyfiq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/guscjcwgi.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwahjgkm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goudcvpjz.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnolcpees.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsysegyco.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzjpkodh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsjkpiqys.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyklzgtg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzjyycgs.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gbznikuxv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gvynqyrmt.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaucdxdn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gmhukyxcs.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gbwsdufpm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfnupgwj.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwgxmzpyd.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gybsthfly.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpknbqsh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gotyennhp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghgrechw.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gpoyqotny.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvfmgqfn.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gfmfetzxo.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gziimogbq.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzxaxkpy.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gmgffeyay.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gggpyujfv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngwsbopv.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjgrlyau.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwiulywq.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gwrtpuycm.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwveegey.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gqsifwxvz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdoelatm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwxhxwsy.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gknqtnirh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/goklhlidz.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/geprlruuz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gslmhynbr.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwyuivuj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkvqadkb.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gerxvdinc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtwvsmszs.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gwloawfee.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gcoixexwa.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/glaqhktol.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/geqizgwyb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gmdkaxdnh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/glgyyvzny.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwthxklqq.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwwbkges.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/goggbvkiq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzdhmkkr.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/glflffpxb.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvjxeivg.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/guhzpxfdb.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvjgwxpd.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghmcattip.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gmljukgaw.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gfokjdfgh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/godfgayee.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmemefss.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/goecjhchq.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/graeanhft.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjlqppqq.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/guzhhzbrk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxlsqmbo.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/ghhusmcqm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxgcwsta.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbpvixjue.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gtjqrgulm.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/geuaboyma.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrouvfkg.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gnbiqhfaf.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/glqhptgbb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwedhflyi.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkkjmcyy.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoeiatov.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhgjuvpk.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbcczqgn.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gvnjtvmbk.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gmrsmatid.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpqzbkzp.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gtyxdwpcl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvajexfwe.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/guwvtdwjn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/glgikuemq.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqzxtbli.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbmhbtdk.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gygsqbqpd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtshbakda.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpdvwzak.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlblrgal.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/goxonlerw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzlbeyuma.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/greyypgyx.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmlobeajj.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgdlnjhj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbzdweglv.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gwvzdrpiz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtmmchypz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjnqqrzg.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gasceursq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfcxpzxft.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrelilxx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvocsyxwh.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfznaevly.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gnblnajub.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfxsmgfl.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gqhgorhlv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gjktqyrnk.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gcfulbdrc.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gutzehajk.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gshiayepo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/guekqjkez.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvaamvvk.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/glcbghzii.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjeldrmm.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkjgmiax.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfurfkned.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/guhipqjex.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gjwbouiyo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmgzzjae.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gleoytkkv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gifizpiwd.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhgspvef.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyubqehhc.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxbemjoh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/grembraub.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmileise.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/geypamvpc.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsdcxysvi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjkkdyvkm.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgluedhq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzplkgao.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxqvlxdsg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gszqzpftz.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdpoewas.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/guokrcxed.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/goeznxoaj.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzxnvuqq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcardricd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbacvfoir.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggulbhocw.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gomxzuzat.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnuwxjng.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gixtjfzkn.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gohatyoni.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gwyerqmdb.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbivjycfv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gficyvefi.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzrpykgi.sHtML


<!-- 参考信息 -->