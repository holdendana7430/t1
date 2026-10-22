代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2daioyjpw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2yorofcsa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dxzaixvx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2xhwfsbeu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sbxlztty.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2entqhecj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bhxblluz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wnqtqode.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2eaxsppfr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2puqsmpjj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2oczsvdby.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cnyjfbkg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pltoaume.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kqtnymqd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2edeewsdf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2fulnytke.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wkuggjqx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bhqzihlf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mpawjqqx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kxmgbbgj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2comxheho.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rcqiglar.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2efugcdsy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ltqkfjsa.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dlbqkqpu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fgdeuaas.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hrniniwq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kfdugmvo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fhkxfzkz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2aicaqswa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2oqnvhloh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2irfiwhct.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2bbllecpv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qrchrrjf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2oxxzlddh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2mrsfurhd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2gmzjibmo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2piujdodj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2swszmtgj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2bgfiqiaw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zgztczdw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vpmblpvi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2rfsljxvt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zspzmoin.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hcrrgzgy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cajzjazm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2cogacgjn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ptynapmj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vlpxfikg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ywgjkbms.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ptpyjpjw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2hbmpsxvq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jbvbuqip.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ssaazwke.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2skborxkq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lmfmdirb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2zqqcbfwm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2orzfnxlf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2jssustix.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2enosjhyp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ddkgfnnu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kokeozwr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ziptccjl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tindmixm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tolgwfwp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvtvdsmi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ezrcvzjw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2owwudoha.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ejotxuvx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fbqfhxez.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lgolvfqr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ailucgnn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jvylrdnj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ulncsrqn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2awfhwfec.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vlhozfse.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2toxcshej.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2uuacrebk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tcoqrwal.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2uiuccxjq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2lthbxqms.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qlhsnbql.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cffuafhg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fjrpxcur.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yagsnyup.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2guzbrxmo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2vcdvxjzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqylzkmx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2uhzpgjfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jikssqzs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rvzpalwa.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2uudmyfhg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tpguxgev.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ioldmpff.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2prwpwuzj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2coyxxmfq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zhcqfstp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mpuheeyv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2kmhiitbb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tfcalton.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fomoghil.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bmezsdri.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kadzswcd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ylyuhlqf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ywwdicom.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qggbnbxz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2opvikcal.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2shptkxdf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2srohwksn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hwtpajau.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hvmisfky.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nplgghwu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gmpeorhi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mxzwmvlw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2lxhtgmfg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gcmwrolv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kznoisty.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tghegbhw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rgwahyxz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kqysujno.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2clzetmgo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2itjdpuub.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ysqmrimp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vtksyrvn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2icjgwlmy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2yttqsrtx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kqqhuxuw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2uwtystgf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2siuxchlr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2slegpbjs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qfooytgi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zobfyqvb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rmpmdokh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ykcystsr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbbvdrya.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ibxbyfle.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hyrzzsgq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qgrjbdtm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmkihqlw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fwmjqvbb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yvdfadau.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kvyqybch.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2iylnawix.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pzxzzcil.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fbwpnnlj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jvgyyfso.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tcrlvwgt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jkcwxluz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nfebemwp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2txnwqwqe.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xzzsfjjp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fmejenza.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jdcftoep.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bakmjspx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lqjkecje.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhdtllxw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyovagvo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2cofbbnzu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2klfexfzb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2titthpdf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rgzkabmy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2yopvnkda.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tqnessqm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rwagkhjz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zprowukq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vfmjylte.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2geuggnip.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2awvlnmyg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdiibnlf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tovlbcwh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2eewavthj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pxdicpce.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rrvkwkxp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2absuftlb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ahfjldwe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hwxjrsnh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lyzhxnfn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mchthghn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xcukrvbx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ddjvcwpq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nivpiauh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2iimduadg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2lvexbmqc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ocqcmdne.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zpgqevro.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bqsjlbiu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dkxutfja.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fauptzwd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tzjdpauw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sjnzrcsr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gacohqye.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jjfeghlq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tvogsdsp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2thlzyzse.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ajvifari.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2nktjnalr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2drdkvtgt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xopsaxfc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xafzolpv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rdnfyftg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ukljtqwy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulfphqlc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zzflbsal.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wwpwchty.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xuogxkts.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cqljudkl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zautptvm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xszdxjrz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ezwsfzvo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2aoscjuwa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kizptcxy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qmirldwc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kpdogcsx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cifzapsn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jcqergfz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2njivlhvs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lgosgolw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmmasmbl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wwikzsnj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ockribcj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2anxdrpuj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2lpgcbtnf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uuppflcx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ioyvgjth.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ymxysnzi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2owivqjft.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2yexqjhrf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wkztafkb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2fpftxkzn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2czscxwgm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nbkcfmug.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tassuriq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fflhkouu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ypbpzcqb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ouzcxlqw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uisducjl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2vlcwgskx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tnkjveqi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yqwvammj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vivavzys.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qoanlqjw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wopzrkmj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ldhdlrnm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vvtfrnak.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ctctuybm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lvkwbiyz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hpfjhnih.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2bzzqtiwu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2sjjmposs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tgavnark.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pdbpfjnt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ewaolene.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zrfmedzo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2eogcnojq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2diotvaip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhomysch.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oudjbzgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2taupykue.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2inuxkcak.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2sujbfuef.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2stytmspt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yhoggvhb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hijyykwn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qksirmxk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ajivkump.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2huvrjfbr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2btkquxkl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ufcuehqe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fszafnti.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tikrgrqn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2sqlnshmq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ejqybskj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zqcavsbr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zrxhwtdn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hmffqcvs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dszjinxk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2swytfwtx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ltxldswf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vjyinztl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gyvgzovq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2obupjhux.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tlfnfcxx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mvjbbobv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ybwafilz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lkmudeet.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ulaafcfp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2omsazldk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yghprvdk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2yyommwvz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2myxstoxs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qtbfkhgs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bgnrwcjv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ibbihtie.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfldqkae.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xxdopima.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wyyedxyj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jafhtivc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bisialcx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rckgyaop.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2iwvgynsk.html


<!-- 参考信息 -->