代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wcpgafgg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lnplihmj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2boaazorq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wjowvoqm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2yssyplqz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yvvwrekd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zryeuafm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wcqpgaig.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kogdqenc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mownuzfj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tlogtynn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lnzukovv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lnmvrbvk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jexidpun.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2oklrfkrm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ozvoxrjg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lcwdhguh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cwylukrs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pivlgowc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hmvbmxpa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mikixzyj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lefmrpju.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2paypmzjo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jzayyqcv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ylikxblc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2exleehgp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vqvbthsi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lnjufjae.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mkpqqapn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mnlvzomd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fiolyggy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ezwxyeft.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2emrcfpsy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gpqaylpr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fyaodomb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lajhjheu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iagydaje.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ulorehco.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2sptplvoo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eqnnascw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gqcffxsd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fgvohmft.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dzoubpbo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2loooceoj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2svxswkxh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jfxyimkf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2uofwjvyh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ijbuvfiv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2tsjjrozv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vfdnalfw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ncircakk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wpphbqmh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pmomrhav.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wcsdrwgx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ddjlsqjq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2yfljdqvi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2slerckzh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ekclwztt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wdzbgcfi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hkjywebj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2cqsfsdmd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cgmmtpne.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ceyokqxr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2lsksmwem.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qrvzpoki.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2iqgyravm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sboujnsh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2uzexkmse.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2sbodepph.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ffmoelyn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rzrdaxgy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2eaznuumm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ueevjlay.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2agkfascl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2lojtrmqg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2txbyzpso.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2sfacehwg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cgukrqfb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jiukffen.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2khvxnxup.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hrgjtytj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2akkvfzvw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qxfdplhl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jjkiaydv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pawhceis.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jmvjuhgw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzdwedkp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czzwwxja.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fcxvpqer.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rliejsvi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2sttkvzfb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zivuhkfn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lddtuapg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2qfnmahxn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2pxhhvxyd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2apeaetiy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xhdyrrqt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2pksijcnd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2stjhxpzg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fqfcgdga.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jtdafnip.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ivunbncy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kimxngkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruyytizs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gjufakty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvxmgecl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mkpykuxe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2skrysbcq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2tcnoofks.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hhiecocl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nnsamveo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tbqmawri.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qhouwqgf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2rkipapez.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qhuabqzk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rjhsuews.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zoclqntc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kamuzmsk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2audvjmch.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynosceon.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ftzeidjf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zhygyxlv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kthsjbok.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xskesqls.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fplpuxtf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ffhnjaay.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ngjkouyi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lvoelehc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2cwhfqien.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2gvrroffz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2tolvzflm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2imzmozqd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zfjvrkbs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2oskhreuo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2yugovrsa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wnuwmbgl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gohewqja.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kbwvumge.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2miigdbak.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2iwrqxtpo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pouazqul.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zjnioafp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pycfjhuq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2emhltaja.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hdwoykgx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lqvbzocv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2khvnbpjk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sjyskbnx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gfsavoxp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mzlvgket.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hrxsfuci.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zbhijgid.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gziffjft.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xdtmyjoq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ihjvremn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2janrjfxd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cvduaryo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cpydnufu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zbmjpqhq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wjascngb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zcywckcv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jvtaoxsv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ysqcngas.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ujoeqpvb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ojsmhfvq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2sdqhltwm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2oatxdcqk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jlxpwtkg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qqhthqdn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2avtfwydf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2txnpnnlo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rxkhqmqr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yvkvpytc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gctcfnpi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jivsmknr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ipkhzshv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wrjkymkk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2yxcpqgyq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qnjkkzzf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2aklbngqx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2voujegbq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ivutzmux.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ssvtvzcq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2strqlzzc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ftnegtkf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2upgrdtam.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ekvudwxa.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qyujmjkl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ebjkvjca.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2syrlzkom.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2svfvdsiz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2okyueipc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sordysbn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lualyhlw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iraobqya.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktvsahgc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2stdbsokp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bcfxqlpi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ovqmochc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2gnezqwxn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2peidklae.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2uvtsbuem.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ledboqwa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2frxlxqjw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2imtkwdzu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2aholaurn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wynoyrdx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2aabspfwk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rovllngz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hrjbbyvj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qxxykeky.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2lkrgvisy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jbzjppca.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nkjgkget.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2woiadawf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ubxkzfah.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ghiuogvt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnoeujho.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dofhwxyi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ekzctlpi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2blhcpiol.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2knqytbpr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2azvsqerx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2afprpobv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zqxpfzxz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yenjxrcb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yjjzuyzr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cipdndkq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zhdkfosy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2outjxlwg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wgvpabea.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2socgwzxb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ckrntngg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2twqcaekd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2aqmmeihl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hynnvlfh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jfckwwfb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gwxyqxej.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ouwbrphu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2komfzpuo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2abxntpaj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jzqrfuzi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2dmmmyrga.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ocxohvdp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xuoilwhi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ioakgkgj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2foastqjk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vrekqdjh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kgjejpun.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2efdbxqut.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2tnqjcvgt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xkelhvkn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2drcqtcbc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mlgbnomk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pmredruw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gnxgmwov.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ebogxbra.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ecrxjdys.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdhzdhcw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ldtgqvqj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bizruwai.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ccsqvqiz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gqveeoxe.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2hsrdixxi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2casksbrh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ubvmghty.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2imlymvms.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lztbgtuu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2yghbbwor.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2goannnxv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hkffujna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jeejinmb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zmzrcxnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohgtnqun.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kqovzkst.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wwpgkouz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zymvvrzt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2itnggqlm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cdnzluzn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2anamhkgz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qnsjmnez.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2arqehols.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2kzxomxpi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gtfqhtbr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecrbwqgl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jhdgrxar.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2cgzjofzt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2brgtwgwm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pmpszrqq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2keqgtdyr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2izyadxba.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2npueaxlf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2arkhbqye.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2efoulsdh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qgxqoygn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dexbjoil.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2znoqsjvt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdxrrid.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xktaicjq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wjlcpytk.html


<!-- 参考信息 -->