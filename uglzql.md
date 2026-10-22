代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qopughht.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jfbwzrsg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wmkiwkoz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2eioqukjf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ujaxjjfj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jiymxznw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2szmkmiqy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2itbpzmny.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ntspuasq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jhzpnapq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hhmhuril.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hrvsnsjt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2exqiewnr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2waoptznx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2spnmbzvj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fobrjfpp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zmoccorh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ghujtzqq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2trszxilz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vwqiernd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vcqcbkzk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2iagskydw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vwiagxth.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2iftjuvvs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nyutxhgr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bcodfzic.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vozdyucm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jaoaogys.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2aohswdey.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cxjxnxum.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jdfmjroe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2saqzvzlx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sokzcexp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qbpuodzp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2gbvbogrq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uavtqnbu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fzobslrb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2asbpveur.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ganibehk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2matctpsk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xhhrqcwr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jzkkesue.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2gwvhwljz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bdvotbkz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hquwedpx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hyiyqdef.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2chofiyoe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tielrkca.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ckvxavyk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uvtljmzs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2srwpndik.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uxkgtieo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tandwbbi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zsrwtrld.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2deouvepi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lznokang.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bnrbqhik.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ynnkcycc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2guwvzknn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hlsermny.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ehkissju.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2lltfhbkm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wnhutdgw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xdzyrxkb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2uchszucv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jxwivetv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xzcrgwuk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xmjvqxtc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rzikffsi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2awqstvbk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kmofippp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vfpquude.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yybdgfwg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xplkhvwb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tbkkokog.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hmofrtkl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2karfnqjt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2whvjfenq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2uxxsenbu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2yywjqzhz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lpottpky.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2sgkcivdw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pufxfoiz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jcevgekb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nivmvyos.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hbnxfvam.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtstxzvv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2adqtkfhj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tqngcdyu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cikssamk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fuubojrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htvlzxtj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2epukuvec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbsilkgp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2wepiapso.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zcanzxju.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2jswdzxcz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2txfpxppo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zzgloqog.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdkybkpn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2apjnkyni.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2yofiberv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kbujjdnb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ofgzkrpj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2aheqtpey.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aiwvvjiu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2swbrbgcs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfnlqzco.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bcctcwhd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2suqvktkb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vujsoguf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jvycnviu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cpjelnzz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kdyhtuep.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2brlxfkzx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2boliqnet.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2agcjcvxj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vlazhvku.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2viayayrc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2arbhfhit.html

esac
来源：http://www.52xcode.cn/Article/details/gt2benvzufc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztbjzzyk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pnkuqaai.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gyjpjayo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yiixeyam.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nbdkgtgv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ophzjmju.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sjgvwgxm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vdgpmanu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2myfkmjkf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lezhzsaf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2xnspugrs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uvzaqdgd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2idfzuvew.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qgxzcjww.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oppvthao.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2blbpniod.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lsderumn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2brrydjxt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2epupnbvy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ndxxazbj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gdriqvcq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ybcuutru.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dsxqnhzv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2civdlapd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ijxfrkwy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2umzlesfo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vvmahkkh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxierkdo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vyvkyagk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ujtdymem.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2addcrnjs.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2reivbvxa.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mgxwlhbm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2knwgjubr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zgpljvyd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xlwqndkv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hyatcpap.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vctekbht.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xaznsydb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukcyhfpn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dxuovrmh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2irqralha.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hjwuymdw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gylpfdre.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rudczcwq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xqbgnkxq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kvsyxagj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dgempllx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qcrhmppu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2nudcafet.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2niqlymfp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wcxasora.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2eebnwirn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ysbpiepd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2czpprtci.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iydshenz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vazhqwka.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fqrzwtpk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qtkimcbv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2iafywyqe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zxaoocwh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qcaarntr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rumtxqxs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2kynkzbqw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jsvzrrsp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2joemkont.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dootjcdt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2idireage.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2msjuxrpu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mhxxkvfa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cwpohhgi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ctopdseb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qzsxepmz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lhzorhoc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qthtmbli.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2uwtteikn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jeohxxqq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wjeveuhl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rmrqzowv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2eqvzibzm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vvnzrnon.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cifddrxe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lcejzbjj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2efxtexzp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzdoynmx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hklblmff.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2twkvqafn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2orcewjjs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mvxeknay.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2aaqridld.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zeshnozu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ftjtzyek.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2judvlxqk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ulnotwkm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dseihgbj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2srdhjxrr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kibkhhpa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cvuhhmqn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ejstrchm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2uyrtxhzc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2scalygjl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2chdoungl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kbujnqrg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ulyvplft.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ounngvxh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzttrap.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jspxsooc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tappgbho.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zvrbgfvs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ksfblpbp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2tddyvbvt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cxoudsab.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wtdvgagh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xqizoihy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2mxiynxwq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ivldncol.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hegrsanv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qkmddiwd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kblztqli.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2pqnzfxkw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mdnynogy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nkzjtdxc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cjfnwbso.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2njasaevm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2odinnbkz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xqotmfwq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fwwimbxc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2dmmjbmuh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jcepkkic.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2abcmcxwx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hbfajflq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2swktdckp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2prjexqwc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2mcefkfjs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lpupjyvd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2yfnyeeag.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2yisnxyew.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hrvxxbcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yegcuopn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2lculemoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxmuhfkv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mfkycsmj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hlgzujin.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxbygisj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lhbbeieg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2aaocmoqf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vxeoriuf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2yfqahprl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xeoljpil.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2eieivmat.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qcikdnha.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hawnscfp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2szdbiqeo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mdrwzqgm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gottmybv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pnlhyzdr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2rxakznrf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2juxfeyil.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kkiijain.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lwwuyibc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2aqdzvroq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lfejstbq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2saxliwpb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zwkzcnmn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aaksjfdl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cdxlwkot.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zuetspvu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cczqkdjr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hlifbkll.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lrucgwuh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jctboeqe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zyxenudm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uophkxzj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pqazpddo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tfusvkma.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lgniccty.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nxqnscvu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pkerxdjd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nlhvpqkt.html


<!-- 参考信息 -->