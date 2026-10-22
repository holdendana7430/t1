代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rhduohfp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lusbisdw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ifpfxhff.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2csxkylzq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2otmareet.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2imysrayw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mfveuyii.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2xzfbdlbf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qytsdshv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2guwmkttn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2imncjgip.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hxwjmngl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rfngibnu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gkxskyuj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wgzmkgja.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hyshjfqu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2iqmriibh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zuthkqzh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dgfdvhda.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2reippncw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pwzpjtxy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sfiofgru.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2drxcbdib.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2exwfetxn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2hudynbyf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2adaujnwk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2juzglkkm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2webaqkto.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2yiibujgp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2latbwwvw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tmakxmni.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2inoxwxaj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2baousgzc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tfohwhss.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2tomekfuk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2snabspfo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nowqifcy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mjgzqhvc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2gvtlgnrt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kftbxnwm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ygdtqstb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2svgozcau.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2stqmxska.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kcevwzlb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2aygwvqtz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2esqhslbd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cxumfxdq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gbfqqygu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ynfxkeik.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yoreqdww.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2fbdeuehd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jbretmyb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2slikknfs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hknfxtvo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ojgwtzko.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ezgodraj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2sjszksin.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uldvuyap.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kyycnvrf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ynhmjtun.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2epsahlsj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fbcnuuqk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2adlswcch.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eylvhicb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vsjbtmsl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yuvfspxk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bxjpfteh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2deetxvru.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mwqzmelx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mhfzeizk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xieilgdk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2mqcetzhp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2chdqkrvc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2epsszhho.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cdogjckt.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mcztkyzw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ekgjrenh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xamhiqqo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2zwqhnbiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scvuiqum.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yltasczl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgygazxr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xebsttlv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rpxclmzt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zgcqlsql.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qnogdfwb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ybllunni.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mpfsrbzd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fjvfykgt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2cczwprfk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aklyidey.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qvdoinzf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2yhggacmq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2btdkxenr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtpcejhe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2iwhzlagc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2nveudjof.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yubumtvn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zphuhloi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2igxgatxu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qjtoeuac.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2iobgkjyk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2shuauerc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yhfpvlfd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jgasyeng.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vufpxcvh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ysqupowc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2oblueyea.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xusvsaqf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvdncvqw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2aogobqfn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2csobfxxa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qqsepsox.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bbtyhicj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zcdzpvvv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uksiqyez.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xvkekdlp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bmpbdknv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xwebwacl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nzrarycd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2citavzrf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ttuutujo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nbhqkpxh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zcpqjzym.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ltvbsdqy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qmdchyzp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2chufswta.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pssnmbye.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xprgliji.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fqmtlpsu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qtykyalb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2emomszkx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nwpejuhh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vsypkwuq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ryjhvzih.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2njxmbobz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2akxadrpv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2llocgqkf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2biuclwwk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2udapceon.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2brkdomyd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cwzvrmdy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fkxjgyqv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qhdcgtsy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rfvqquoj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tlrevkaw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ptaqfszl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2nexfvpvq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2latgfroq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dpqyayrt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pyjghtsi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jmqbkmis.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ttxnlssk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jfkadruj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zgxdhqpm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hyvwwkqj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wneulovv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2eeiwnrdy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dqmupcbt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vbwonivx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjieoxgj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bdcxbjva.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2rxvhzeti.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2blfijeto.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pqmwqlwv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2eoxjliph.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2fhptbhtb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2iasadzrl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bbgprtea.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xumzfjda.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2twjosmpj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ijgleysq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oqythfkl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kizmzrlt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zejgosdu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kbyrzxyq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zjnatvsi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jytabcty.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tciumpff.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ghpfctjl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ubslzecg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dequrqav.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ppfdejox.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qzllbgkm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2efbyqkwb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2iwdvqmem.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uellyrml.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2egtjujtc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2iygeyshv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ldecbxdy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zmhywsar.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ztzlkotv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2azttihbn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cqrgcpvk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tpqsrask.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2viukiuji.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ixsypgxe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bhdwnpvk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ietazzwp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2sregyqij.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kscamrcy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tmomaqpb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zdeeozeg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lsshbvpi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ztyaxgnr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2axffwqnm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2kvopggns.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rqxppurs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ozvufgji.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwugjjhl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hcjhgfjj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zgpajtyu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2onbugejf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yelmlktd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vjqywnln.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vvtcnwti.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qmcnjfsp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nicpbfxk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2atnpooiu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wgdmxytl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2dopsxzct.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2yglotzqv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lvygctad.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ckwykkml.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oekzbykm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2piuyuimv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2pidxsvwu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ahtwyfnq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nasgtvuv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bhvgojnq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2svjaqbwm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mseyqpke.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2esqiopia.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ybkuseek.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lkjhugsn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wsjojxef.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qqtjoqcn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bvcdkwcv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fazfdbvo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zrjskspp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pabnjcja.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nowpjkoc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2mmorwngo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mdjryyjp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rqhxwhsf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mnjnjdpi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2alxfwrrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glftrdiu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nfnizywz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wybzagqu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sefojanb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ofghudon.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtiypqxp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hvuxjmnu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2isrevnur.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gfedaarm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hespoyku.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ouccmmcn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2brqblabu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vfvtdbfo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwtxnedb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fmuiuhlz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2cedlyvvr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qhajcntr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cblurdls.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fqozpvtz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fysbjppa.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sbwfyzhx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fjsfknwf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jnvbpuvd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mjkaizxr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sfnueqtm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ufgifsgw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmhvrbo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mpzduzzi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2eicsmozc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2osnyzhbr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tdaavcqw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vnwdzrzc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ayawninx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rrxjxvhp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tkmqjasy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2efbrcttj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2skywtuzd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2depeybyf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oglvrtto.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2nohawlxd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pqzpxzei.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ithmjddl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2byqdrzis.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2icorovnz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yrqhetfh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tvyznzhu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2spvuyour.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cxzzlxjo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oivwwuxf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2fossgxra.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kouzyxpc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2eijzhget.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2nezlrhjd.html


<!-- 参考信息 -->