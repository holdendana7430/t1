代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/grukhehfn.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gddpcjpmx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gnzpphlii.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtriohhg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glityubck.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmglxmkkj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gbiuvhrhe.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsszuorpf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkifwract.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/giwunisww.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbcnafja.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotguealu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gttjmzgwu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpzxstny.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfpnwkiq.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/geuesrjla.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnwpeatm.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/grlmorgqo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glnulpmhv.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzhmyhef.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqhxzhuu.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gyrpltwgm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gidxdirrw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqzilrye.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/ggmsevqgd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgylqjgc.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gqidiwucb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudgvzesw.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gggvtftev.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gseufojjw.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffqwlisn.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajegxcdj.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxrkypbz.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/ghaqillmj.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gqsilmuvc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqygplcvy.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gynupvmba.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphikjbpl.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gtvvsxbkb.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzuooopxh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmreetja.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gskpcufvf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gpeybsaqo.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gijfbjbgr.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/geyxolcsr.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzocaybm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gaqgbprfw.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gatqajkru.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcdzsawjo.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqazmewlq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gniavnoib.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvccgqoo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgfrqwsm.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfnywwzl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/golwehhbs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gsmdgncdd.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvpjibhs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gcaqftplc.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/guaybbcpb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gpudwmepu.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gkesltfet.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gnnilfozc.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gijrnnjsf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gtljjmhzw.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdvqyjou.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjnokhfrk.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqvjabhsk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrqogffq.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvtuaaqei.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gynvwoxur.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbclubbdr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grljiourw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbzuntgm.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gykuedstw.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggaifkdl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geejrqlym.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gstgbqtlj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gbamhpbzw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvuzdctmv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfcqagkn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdgnpqyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gjkpmrhii.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyshywtpe.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gcttprlja.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gbzjuogbm.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gspcdpelt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduefezjm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsubtobpr.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gsoedduwn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmnrnuao.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/govhpfcgg.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/golfhwbxo.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/golnrsdns.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gkelzsryl.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gcguoaqpc.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/ginpgxcrk.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gqaszvujv.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpemanalr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmeskuvb.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gpqhttgeo.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggfzrqayj.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/govrxsqsm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqcsnykq.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaajyctft.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gldvsxgvm.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gabdbmreq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gpclfpxbw.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gdncyzdtv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuzmkthc.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxbxejoc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/guotkytaq.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gadaolwpf.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gthzmmhjb.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbicbxclw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyutdjomj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwojyoxm.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gxwjwqvcd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdptlhrsq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzxcfejx.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghmscjgrj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gghfwseof.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcfgilfq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxjjkuha.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gepuapoko.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gevrbmvjq.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzyzkszgb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmwwgccqb.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gmtatbyyq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjskdwqct.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiduwfbq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgejpktq.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlhsfcln.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwhsvvsn.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gisocsyjo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupnljqva.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqinmegp.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlbjqbbe.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvvdyfhf.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyspqaup.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjabfveex.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicvmwpbm.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/ggrqspdqu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmfefzkb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/glavxaxfd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymivqsmx.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqslsigid.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuwxbwib.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gvnplencl.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/giouwvoon.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtllwthte.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvemrgbb.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guexxwwex.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gukdicrbs.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/glftbclcq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gfjlajwem.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxbbjppgp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glbwhrhkv.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/grrskbbyw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjlbuywgu.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gofhkcqno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwwxytlh.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxpweiwj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcdxdydz.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/guutjimnv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/glfvrvpig.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/guyqghzgy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyxbpprs.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmvkzwpg.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlnhyjbx.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gahdunmbe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdwijuwc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcnyqyuw.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gfboebpjw.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gkwmmtreg.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gydayomym.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzfrbwmt.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gvidsujyp.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhkgnpnt.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckwwdcou.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmojztks.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gthtlaaym.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gptwnvtvy.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gjhzsgfle.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gxifddysa.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gvwiudwbr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhkiuiua.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gqsuzmesn.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/guviulyej.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gywamkeoq.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gdipechhw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gftrwblmr.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/grucdbzke.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcfyruko.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/geiwlahsd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwepsqknc.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gwtqeqege.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gbtxddzlw.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/giqczadee.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnsyuhps.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gkizlcsol.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpitlcwa.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gisrbaipf.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuknvfvc.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gqbydimxl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvgblkpo.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gqvamjmnk.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gdtvoycws.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgvokpwb.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbzmcxqd.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gflszmena.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/golpfzccl.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/glanwpulw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeahizpd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/giiewmfpm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gjubmptaw.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpishdpo.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gmvfrdmsp.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzxnynueh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjdamnjx.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbdvovaf.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gesrcyymx.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuzbnxwg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gjdwwzvhj.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzsgqxfe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/ggevskyjo.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gaskwqzkb.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnavtgox.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gotmmjdkq.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/ghskbilyl.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gnuduwkdu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghgopisgy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqamrciqh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjrjyixb.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gvvqkkjmg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gpnnbjhek.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gomjaqqjt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdviwymp.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gwmyfspge.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyquavayw.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkiijtyu.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/giblypcuk.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gtvsiklyq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatbiuubz.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvdhwhhj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuflysgj.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwtdcgife.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gbimoatsf.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnqdarkr.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gyliacjoe.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxqzbvou.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcwgdfkgo.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gezicrjrh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyctziyhj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeiqsowv.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbartrom.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gftssexdn.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gtynpfqfz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyimkolp.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbtphgwdi.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/givjhhtcv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxyswsrh.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gcinffdfe.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeojlsai.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjtektnl.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppqlgxdc.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gojtrxuxj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyjncqoj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpozhrub.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gksmeuzrx.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdbtjfdd.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gooshsgfu.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/glwmakzmh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncxleskl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gbzxvmuip.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsijwgavq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gqlctpuhw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/ghrxshqqy.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhxyydvb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzdjdjwr.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnluqqmgd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/glkzraaze.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafaxjhyy.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gpntujkwe.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/giitxgqvg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtfugrzgx.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcsjjjct.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gomcxcoqc.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrglindb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbyxffew.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gebmlwiil.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gggffuljq.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqdmehje.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzppdhsny.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjzlcmjcr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskgjfoco.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfranrvii.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/grjzukqja.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/glaxwmurj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmqyvifn.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgzhaays.sHtML


<!-- 参考信息 -->