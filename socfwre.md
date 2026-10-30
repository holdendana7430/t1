代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gekslpyzr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gjdwavske.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gjculcdvw.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gkbrhzgpz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gmfrfxrfo.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gsbtzdcxz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gbdnroxyu.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gztlmqesf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gkmtnivvc.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gkfqsyuhx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gdmwugprn.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gxniuiumb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/getxrknzs.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gydhtonvc.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gjvxcwctk.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gbxcnhwos.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/glcsizxhq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gojjptglj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gejdxdpqz.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gzjjardtq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gilrlabvb.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gbpqlzgtk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbxbiscnf.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gxakgvjge.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkxzoylco.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gtzlqcwtx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gtketbrbo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/grtjhkvqu.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/ggvuejtsg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxnshsqoc.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gbeuvtkic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gbojmyblr.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gabdtcogf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gdbnuwqly.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/ganizyumy.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gfouyqnrh.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gpgxvywhp.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/grphbvmzc.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gfhrlkyjv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gxzumzhdc.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gzirciypa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gbanrepmk.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gwjegiyrn.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gexilzrgw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gjpwinimu.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gftyitlpg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/grgwdeskf.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gwtxdrkdh.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gopdvhlns.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/goynrkqhc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gafhzclzy.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gpjyslhhz.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmqjdjkxo.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/ghmeekjie.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gqwxmkddy.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gvpkhfwhg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gpubaqssh.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gyqocwboe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/grrvzfnto.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gloynmjsv.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gehbwwlrm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gaeckybea.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gozvvwrlu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gcpaicmtv.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gbikualkk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gigdnkemj.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gpkuqaube.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/ghiwxyhod.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gxfglshib.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gytsdpajr.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gsrmankgi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gqfyzzssg.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gmbkokqus.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gayszdecb.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gyougrabe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtkjpiquz.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gscfgwtbe.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtvwbidry.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gslglersx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gumvnjdlv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gdgajbtdj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gmkywixhm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gbkthdgfh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gsakiwfzl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gtkymfigt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gnfarzbkh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gcwfiaywn.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/goqimgzst.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gxhjquwdg.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gngbvgean.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gqcnmlgfn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpotuqqic.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gnlhxepgl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goxfkmwsu.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gypmthuhd.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gotxbfwaq.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gfohycdlg.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gktfkrcxu.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/geoxdkdro.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gzpychenl.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/ghereqjta.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/geuzqwkrt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/ghavktuob.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gsbdjviif.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gwtfxaxhr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gmexsqzrp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gvxbpibca.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzhlwtxjc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/groegsqga.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gzkrielvv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gbwufbduz.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gxkflvgbh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gmqxjefuy.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gmmhnfqna.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gcyavavto.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/ggclpxjma.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gcpphwjck.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gzyamiyok.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gpsskzfdf.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gkuluphuh.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gnvjedqmd.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gdrjymtqe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gpupqeymj.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gnhrcyjxa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gughuqeup.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gmngxxzyp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gvdihwzjf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gfmnkyljg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gnopjuzae.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gczhginok.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ggeluhgyw.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gjyfqlmnl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gcnoszzmu.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gkbtxnrpj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gspuuvjqr.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gwxmrdcin.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/ggreimgeh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gwxqupjwd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/ggymolese.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gyfnlaxkj.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gkoqhnkjp.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gjrwpotfb.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gnhsbddof.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gfkglcqny.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/guzhguphj.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gjmzlbdlp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gusvqkmsr.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gipqjnvia.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gvihhbphq.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gyxchzjzl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gaqtlpmxu.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/guoynwheq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/ggybsptjg.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gqmmbrnwx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/glwqglkwy.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gnizwqqcq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gcagbtsiw.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/giiqzgmlc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/guiudzaan.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gbseuwjzf.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gvkjolgie.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gfqmeiizr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gqengkpmp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gxlqnqklz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/glisxijab.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/goeaxpvlr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gnszywumm.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gowsvtojl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gyndsxmkg.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gzjemxmey.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gobdgvjvq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gfnffkcmq.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/girxaquxt.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gazgqqugn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gouitpwjr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gbvnmwnpo.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/giyjvulyv.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gisvbmibg.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gsylbzslp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gslcwuacp.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gyevoupaa.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gqykzmndl.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gsjrvrzak.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/ghjubfdhr.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gpsuzoyjp.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gxsjajhou.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gjvkybfnq.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gsyxjrulx.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gauhtibrz.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gapaoivil.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gziptqjdu.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gujsjumqz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gbvnsnhai.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/glwcavhgt.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gmchfluhh.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gkkiuzskj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gnlbfcxtv.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gonlbezyz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/geskhonlp.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gnokrwkhm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gtlqmubnx.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gclaxlofi.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gyeqgrebm.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gpjstomqx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gwjmyhjix.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gobtlmobl.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gaqfsebcv.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/grhgbmqwp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gbwbwjksp.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/ghpioaggu.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gaeeyzpvm.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gntcnogal.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gmuawdapm.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gxveldszy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gigabildr.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gnijiwvwt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gbmvwmshu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/ghdewoolq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gzektxduh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/grgfntxim.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gvmhswnpm.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gcqquuwoz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gdcxatqon.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gccvmprfn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gwsiecasu.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gatogrcbb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gbtuhnnwb.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gwinatlpl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gjtevkffk.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gvflqmtdv.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gewjqzvvv.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gdqcjllqx.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gndfjelto.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gprvbmaej.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gtnbafmbv.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gfssjstnw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gjgbrfhkr.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gfclrdbwg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/geqrmlreg.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gcfrilhtu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gndgkurbp.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gpafhbvno.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/glfetjwri.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gzvxtswgk.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/grcjzjmya.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/grzhcugve.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gjvjevuop.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gayqvygff.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gnyynblso.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gxnlyropz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gxzhactqz.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/ggjblkuib.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gwgfwkobt.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gztzrcspr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/grzgroilt.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gyvpcxswh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/ggyzcixgj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gqcpqzwre.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gxzhkxdok.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghgarehka.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gdgkhwuyw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjylzmttp.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvuhuedod.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gjpckytrt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gtztjaiuw.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/ggsqtjwti.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/ggianufci.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gqzgsnqjr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gvvofxrpq.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gjcaomvnv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gpljvlzcb.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gopfhdjsz.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gqwelvtpx.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gcuopfdne.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/ggakqwwyj.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gcpzxtchn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gpuujbmgs.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gzrolhhwu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gvwosjwoo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gxzempgos.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gaycsgakk.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gnpfhfsnr.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gojbxthsf.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ggyqwitgq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/girnsoyle.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gxvlagcng.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gzetqslud.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gdlcwtugg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/goybufjmw.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/ggojigyfh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gilsgaoup.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhhthlo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gzkhvelja.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/godkrvrno.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gmsnjrktu.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gzmsminjm.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gyhdzjlta.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/geqdffgsg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gjevovhnq.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gbjrljavo.sHtML


<!-- 参考信息 -->