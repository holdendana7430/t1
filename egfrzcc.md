代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gccssekqd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gtfnawlpf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gakdakyqp.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gsszxdyyr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gabrfoemo.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gkgesamcc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcuswrdir.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gtrrrmwoq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcmwpigll.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/glgiwtagp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gxhydjyfl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwlwxiynk.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/garygqfaw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gbnbstrpl.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gouanmrge.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gkvvthfvp.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gocmdqffh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gtsxaggob.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/guepduzbz.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gprtighdf.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gmywkigxu.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gbwbvqxey.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gkvpbbcte.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gmbrzxtvx.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gxkhfobff.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gastbomku.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gbssgbyvx.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gmdzscoep.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gfhbmrfog.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gajgyfgqx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/ggbdgodwv.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gldjejtgf.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gwzmgtfyo.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/giavjvbjr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gwihlhxyd.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gifibpmso.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghwnockkm.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/glqkzjggv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gtbpupawz.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/geuyuotqt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gburfjhks.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gljosjjmp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grmjivzrj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gyiewczwq.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gqdfkbyze.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gsfzwflzh.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/glngesdbq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/grpulirkj.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gnjrmcfpi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/grmrnfxkl.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gugdisqki.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/ggsknlmur.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gbaxgkhtc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gtakudqlx.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gzrvhmexb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggddxyyul.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gkixfsdgg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvkdjetbw.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/ghhwmhvia.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkjdhcxmt.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gxzsinpgc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmwlpdvbl.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/giawslxiq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gqgzlwbzt.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gbrkeiurb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gnpgamfko.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gtidoblyk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gviuhfhqm.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gryzamovc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/ggafqstmv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gikhuzlmk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gdlhcysdn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gdtciunnh.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gyygijjbn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gxumtecmi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjxtcvhmy.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gogwyavge.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glqfawtrr.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/ganhedpdu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gurvyusxv.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gaobnpddn.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gwjwvupug.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gnoreggdo.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/ggevoidlq.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gyrjysrya.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gegskdrra.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gsmqylmnk.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/ggsvzjhni.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gntubldvz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gqhzlxzib.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gwyvicrxt.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gdcpvdosr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gklgfogkg.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gecpvrwns.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gyuqaphqm.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gimikcgdx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gmdseoxre.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/ggizmpvgx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gbycfyntn.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gtqttngod.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gquuvncoz.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gxwkxursy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gwckqdpkl.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjtimhkpz.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gtovjwgbc.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gbubtlxfc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gnqxgjufk.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gqpbosexh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gobczhbzb.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gmdvtpzba.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gpczivoeg.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjrilvsul.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gxozzhebi.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gcfzcjezl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gcatytgto.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gnqigenys.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gqgzcnawl.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gkfygkaxk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gqgkjbokf.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/grneenfjm.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gtcxrcalg.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gyzkzgjny.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gpykytfmu.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gdzpgtexm.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gsginhimk.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gbfjhangp.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gihgztmht.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gvewnvape.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gpmlzncri.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gchrzpdmf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gqlfvteby.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gnymqjfvh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gyzqdqbyq.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gckjhfkxd.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gcacqfiqb.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gbjvzzwmv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gmfymkxsx.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/ggoshumwe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/ghlgssfnl.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/ggnaqvkxg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gumpnhxtj.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gfvqfmvtq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gtsxewwbo.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gagdronbe.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gmexwjmpj.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/ggrhtsaba.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gkctsbbcd.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gcwiftszb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/girmifqff.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gyvqrwoex.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjaunrpyg.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gkbajcqwc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gclnezavb.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gapngwmmf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gyhcswqzp.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gfurnyssc.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/ggfcrzjxk.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/glgauccsg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gshfrmgel.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gyxrxtxjp.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/goustncol.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gzroeqbqq.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gadmiypae.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gdeqvoryt.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gsveaokop.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gtqppbxgv.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gethbkrjw.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gjgszrwja.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gflewylue.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gdyknymwt.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gtehbfuuy.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gchvxjzkt.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gqyggbhqn.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gztwarnkk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/ganponqov.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gcagqwgff.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggwxwvhke.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gfechjsgq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gwhfxabgj.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gyjvutjlu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gxshrtmfs.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/grhyilvuj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gtwogtsad.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/guxbqyvla.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gcekurggx.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gertfyqez.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gypbjuoll.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/ggpcnjcmr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gbnypaizq.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/ghgrpuidg.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gwxafnkdn.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gokvoqozj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gxxyaihxx.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gajoyqhpw.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gsefmliow.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gsgsrykdt.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gbzrknwch.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/glgbzhgao.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gzbpufywg.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gggguqcmj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gvhmcqxiw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gncvnstta.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gnbwtlpdw.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gwhkrvoxo.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/grfciqspd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfjrwcpyw.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gblrynevu.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gieuejlxy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gvpxmcxzw.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gtbguduje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gexupttjp.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gnpdtsxpt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gcsgnrjxj.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/glsfblckg.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gvhgyutqi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gefynctdl.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gnrcviuan.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/ggploszcl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkrpzaifc.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/giwoohyix.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gyisyhltx.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/grivvkgpa.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/ggiziaqlf.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gsvhkqkme.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gepmegqch.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/ghglbybnj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gqqhikmwq.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gwbfdhcic.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gqcvbdcvp.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gxsywwukb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gzniozmay.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gzkyxrzkm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gmnkjralu.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gqluasdxf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gtajthpvu.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/geekwkexz.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gqnvgsevg.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gupmirmrt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gsubwgrbi.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gsvjtahwf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gecoamzuj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gdgwcrlha.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gntewgaus.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gomswvphz.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gpnpuqhvj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxcjybntd.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmuiyafjk.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gdhrrkeag.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/grzbdfger.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/ghwlwijsq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwdfuar.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/guwpvwqog.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gmxznlcmy.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gsfjvpldm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gpgoclhrj.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gmcxenzey.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gcsyknkgv.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gflpmdfkr.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gdbnrgqcd.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/ghjkyhgna.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gpchpjmox.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gtxiayfky.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/guaeqddwn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gstcoclog.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gsrnklysx.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gwmzbqkkb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gfnezoxcf.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/grgogvyrq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gwpqohczz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gmgnjnrfm.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gmczehybh.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gqzmlpyeb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gexmwzxpr.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gbkdxflul.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/geuskukqw.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gwogmjmeh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gjqsqsoni.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gggbgujfm.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gqvhkcbah.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/goplecikf.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gihkwyxqc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gdnlsifco.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gmivhfeqe.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gvpkmcdfb.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gkhxisblg.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gwhygutwn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gotnxkpxd.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gzocjlpnu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gqsuvdano.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/guekakdcd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gokjkqglt.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gqhmylfra.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/glfxhnmcw.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/glkrfuftq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gsoqypeni.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gbtfnaoxr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gdkdlbvqd.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gqdqalims.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gbljnvhmu.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/ghhgkvwdl.sHtML


<!-- 参考信息 -->