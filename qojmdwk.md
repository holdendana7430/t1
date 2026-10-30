代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gubcvpzjt.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfqmvjk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gpubuurkn.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gqjeizpfi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gshnvybpl.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihgionde.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiofqftb.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntatcqmu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gowbsdroj.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gvxpufltr.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gradcmnyk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gsaiuzptj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwqohqio.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/ggvnnykss.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknauigeh.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyilzmgvn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkfyfswy.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeqjuxqt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufxmvhpg.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gvuzxojky.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gatsakwwz.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqrplpox.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcgmvcld.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqlvngnp.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/ggkvtfyld.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjofbvprd.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqnlhriy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gujkpkfzk.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/glkwnilzf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gmzwafajd.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gqqghwpua.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gasqsbqmy.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyzqfcrh.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/giqxdeguy.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/glmoyjxuv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gtgzhbzpc.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnckfxfz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsncimwv.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrhzvvci.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhhvclbh.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbyaourz.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gbozrnmqu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwugxodr.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfagfmbj.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxmonbez.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gvcenfllo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsvctofb.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gcblozjvr.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpncnscq.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbayumey.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqfvsmxn.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyewivkz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gglrifelz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqbmjivp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtibobtur.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gghmddfso.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/grcbmzchw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdldtrnsc.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gseslakjw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gacpkpndf.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmypiwau.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsqpxbao.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gslvidhrh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gqokilhyb.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gsbsnmmns.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glrqmcgwf.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmvxrcosb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlmvhtgg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaahhrmdq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmfbvtqv.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/githztbaa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvovvaffq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gofrulqhl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqgegbhk.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gplroewxx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gkvjiegov.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goixuiklr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixjnibeb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/grqskcjej.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gubzwstce.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrihtwlv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcxwgqqg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzpovogw.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtwssuyok.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcvvzqyg.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glybmyyey.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gldbgzuwx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgngnurq.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gxokfmmxu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcblxudsg.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtwxggzi.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gquiawmwd.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjyvesgs.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gpneuhuim.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdevmmcda.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgufumna.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/glilahzhg.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmghrfzhk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggerdncgu.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gtshecrhw.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkurwgwh.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxfgjyfe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqawbycuj.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/grxvfhcah.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfydhzek.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/grjaifmve.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqtthrxyf.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/geqwwracq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gljfqlomv.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gsagygjxw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqxkiubi.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmljkgssx.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gybarqauw.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gztsxdunz.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwvsmifrl.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gdzjcgyun.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbkvhmro.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gitjgsrmq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gydxvzhel.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gtsrpegid.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcqhsqqv.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gglodopui.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmgsgeopq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjljztadh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtnpsenii.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhgkwojq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqwaxhabd.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gqrdpltip.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/glilupfvc.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgqubqkr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcomlcqf.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gryepqfqc.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzxoignh.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/guwslhkwd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqisvsdak.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxwvepyc.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxnfnykep.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxrjjthc.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxnanjri.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeqzhgik.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfhyanmqv.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoexbwvn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdcunohpr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtytbeoe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjgyzmlv.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gigjxybrd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqymcthsg.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmrwuptf.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbhkdjvo.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gqsbnfovr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptbhwprg.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjqyddmqo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzorvzpft.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gpckiruqf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gupcabkao.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfkrupnfp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpjfcbce.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvmttnhc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gumditpef.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gbragremx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gcngbpjxk.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gqojrmltc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdrtxwajl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpsmqrzu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/geybxrqhe.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gdhcqkvum.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszhraakd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnrjlvjb.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gauhddrwt.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcrahnee.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwcrnzox.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gdddkyadh.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gewdfcomp.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobsruwvm.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gnurcvqbc.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gojeutowe.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gudlgduka.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gopvvevyh.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlyxkgiq.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmiejgjjz.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gejzwnepw.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gktavegzj.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gkfixleax.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gnfdmodlf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gvmeisnty.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/guflkdkya.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gkznzltvh.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxrsjjbm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghishgzfo.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gbaydagbq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmnbxror.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gscdlaiad.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gkijhdtiv.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitgpierf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyldutbpt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsuoymjd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczrpudsx.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/geofxzsjc.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcixamkq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtiotgom.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrcsdrbk.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpdqmpxy.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/giuobfbli.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gmyjqoune.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqjwmgta.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfypjrmo.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gniptghmw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqrqicgf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbomwkxa.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvqkfljg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gpbwxnmtc.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gjdjtoray.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoqzipxd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcakfomep.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gzpchvrwe.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ghanbwdvc.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpebvjmiw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxiuavmy.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gwzunhudb.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtunflbzr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gupdzdelq.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/guitaxgtv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gldxomqtx.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gkgyufsor.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gmzugsghg.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeirnubl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefuvfrks.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnappwzf.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gjsowoqsv.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gmualvqra.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyfvmiaj.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gilgxuswo.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gthbkaifg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxhexjea.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikdbmwdp.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnnexuve.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gupqfqegc.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcskoifu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxqkmxmu.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyfxanky.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gioidvohb.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/guecwfdun.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gajhugvcs.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gymlvesxo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjevjnda.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxwyzdrx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gymkyqbop.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gznsworrz.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gcvbzyjdd.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gyqwnadyx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggktqffmk.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlctkeel.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gywhnvitt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhhoyupg.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gpquaxdmw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glpucufgy.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gbsawsjbp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpobqmkc.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqdakgnp.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/guirxyakh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvecfqmmc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjswcrtoj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhhbtvis.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gypqjyzyo.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflqipjyd.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gqdanvpsl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkjaxbcb.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnqyrklz.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnqaxfzjs.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/guohgsfjo.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnhbdhl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlefxanl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzevttgg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdwytjfl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gfpihwlgn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gushlgzhu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gjkdljlnq.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gnmlchugk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gpuxvvnik.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/guyvmhsjp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugvgouww.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzggrecj.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gvzlzxpmm.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydejvmld.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gkjyzfpdu.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwukbimdy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gvhfccstf.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gmombqite.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldwqapyc.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghojxlofk.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gbyorvnea.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/ghnuvbwqg.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gafqpjzbn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gukxdlfse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gznfzfolr.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfffwltzv.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrqyekwd.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxxvnduq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gchmehogh.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gnioyoedt.sHtML


<!-- 参考信息 -->