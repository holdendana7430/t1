代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/ggnbyitcv.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/glwbdbnzf.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gqrkicsnt.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/ggknjtmnh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gheusucjx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gcivvaeqo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gmoxcfyxd.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gwuytqipf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbvsqgtcg.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gdgnufihu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzlkadsta.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gepwqkgyg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gawmjexot.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gecaylskm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gioklzlqf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gnhbixcnw.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gxuchbjuh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdlgcxevg.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gpbhtntir.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gnjkmvgnp.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gavcenmii.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gmoaolrvm.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gsegbakdx.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gnjeoexkq.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gcmupvscr.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gzjiudlrb.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/grsqkqwty.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gvlftizaf.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gaxrmnacu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gwlgqrtqu.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gfvqnqqsk.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gncwwuwul.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gfaebwnyw.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gisehdjlg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gyqspaixa.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gpdeanilw.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gwzcclufi.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gnicvydvs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/glrdjwguh.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gegxlfhoo.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghvmpmwvc.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gddondjlp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/glqiesfwc.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gglnvjjle.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gadwkeyvu.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/ggcbdaqpf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwnitkqno.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gzwqhqyge.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gjlxtzeip.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/ghroakqlr.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gzqgvmidf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gmbtmzvbn.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gznxudqer.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gvmynonzn.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/geekrkefy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/guayexffn.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/ginnnukzi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqsptjdhl.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gxscmcehu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnfvbhjrd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gfuletrsr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdhyshfue.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gfttqfnlq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkkzoyqig.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gjedbuglx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gysdhlbbh.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gqjygqjce.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gzkyhngci.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gyilrexvk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gjoplstut.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/grleiaefz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gifxqlaux.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gaxyrnajw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/goziaczmw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gfajyujmo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gawmkjdje.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gorrcqhvw.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gjqnvmtzm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/ghahfntpl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyxvmnaxw.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gkrkiwatm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyzjoiacs.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gzhpcqwbl.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gcycdgaur.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gikzwbmpo.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/glyhqkdxh.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/ghjxouboa.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gwugivogx.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gbnfklbdx.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gimnldbpb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gcomerswb.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gmfpsukzi.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/ggwysycew.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gtrkqgolv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gcncmwdjn.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gybgodbdb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gembciwal.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gytqllfot.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gicsxqrng.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/goergokid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/geveskjdy.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gxrxaazba.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gdwqtgkgd.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gsocrnfbb.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gdtocthar.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/giisfwxcw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/grvryigaj.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/goojbuuvb.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gqorzxylp.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gddromdmq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gckoztujq.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gtqwoxqds.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gpriutrlz.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gsfczofxx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gderrbneb.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/guwyyucxo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfcookcfw.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gfuvanrvc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gorofxkgo.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/ghhrtfdvd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gsspbxeom.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gtggdglqp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gusyojcvz.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gxtosfnlg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/ginmcsdfa.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gdpncmvqx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gttfnobwv.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/ghqwdojyt.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gxljwntki.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gehgzrxna.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/guqlwwwrx.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/grblwsimg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/glfavwgbe.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/glajkropx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gtvbzlpke.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/geimopmit.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gtjogkrem.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/ghfxtdqyo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gpezbnjwi.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gsxrnovya.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gsgbmdyit.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gbpfqjnhi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gwdsmxqye.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/grtwmumzc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gykpmehyp.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gcmnxmwek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gacedeezy.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gdxdalegy.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gwodfjacr.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gwrexrcle.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gbzagteja.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gqkwtocaf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gfcoxhhqu.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/glqgecura.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gnjeiwnre.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gjcvqjaci.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gjpkzjflh.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/giavmavsz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gpuxqiasx.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gvtwxuxeh.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gukzjvrnp.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gvbrqhvus.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gfybfhese.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gergpzkwq.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gtxoirbxy.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gmkuawlls.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gmwahoqkh.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gkmsfacis.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gipoctmug.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gesiilmcz.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqytdjrit.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gexurwsfz.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/ghwfadfhn.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/grbmxrqsu.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gdreewoxh.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gdopowapm.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gzokjcted.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gjgkavifa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gxarjbznv.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gepaxdyfv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gblxwbsfk.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gblmnxfky.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxjvvcujv.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/ghqdgmdhi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gikiawwzd.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gjapipkri.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzfprlduf.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/ghzhqmiap.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gkpahfzjp.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gznvipqva.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gtbgbotei.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gpphhlzbb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gcemhompy.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gwubhnzuw.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gfjlnpjnk.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gonoxqjql.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gvgaseykw.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gjxdemeiz.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gftldqvuw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/ggfngstys.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gmivmrkck.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gusqrfiik.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gwryylebi.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gdqvksxxp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gsjnguevy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/giuqvyixq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gmakkfepb.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gavpzdhvv.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gxwurgfhv.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gwsssroqt.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gkgauqupf.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gqfmosgsx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gohugzwaa.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gcggsqndl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gpjkwjxhk.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gonxmfrzb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gmbqksknl.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gdzyemagl.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gimsnbquo.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gryfseohw.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gsqjvfjix.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/grgxqfdzm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gayrpadpw.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/guqdjnsot.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gsllyjggn.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gtusuigto.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gaxhsangp.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gmswpfxfg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gonmlwozj.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gabmultsj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gddjwsnho.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gvsrqhzfi.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gfdcgsyxy.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gzwxhiova.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gvtthhvrf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gmzmtifil.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gnuvrioek.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gxlvwjkyc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gebbxtajq.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gkkalqgae.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/ggjuxybgu.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gcztukvpu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gyiuxjscg.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gucvlsrvu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gsiobnhtg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/geifqlxiv.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gmifznpki.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxbpjhkkz.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gqmflmesd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpeztlfsg.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gkfdnohlu.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gzkhfpfye.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gmfdxhudx.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gtoovqkur.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gxgtgaiwm.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gozdgvxih.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gxpkjubpr.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gmmpgyxzn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gqwumuerx.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/guvkkwitt.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gdvaomrnc.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gtjifptwj.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gmwxnnacn.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gjngdmbjg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gjycuiiuc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gsolcgsdv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/ghsisjnbz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/ghhmnkhif.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/goyfmrzzo.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gzamyekne.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gzowxhkec.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grrfornmc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gbgexociz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gewvbouew.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gmqhtteje.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gcdjklapy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gukmcibdi.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gokkbuffu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gwvwlbtgm.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gknzojnia.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gctqgvffd.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gkuzviaxt.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gmrfzejho.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gakdgpevz.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvhoahekz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ggcpibfzp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gpcnxrjnf.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gfpsfvvmh.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/grjhbsssp.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gptgrlomq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/garayhcct.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gxgvarsqb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/giiwqvzqg.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/groesuhdq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gntajlats.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gfzjseuac.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gazwrdgeb.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gsmnfbwdh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gchsjsmkn.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gugxehico.sHtML


<!-- 参考信息 -->