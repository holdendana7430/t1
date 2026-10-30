代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gyfgogajz.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gwauatlmo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyegncaav.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpdpcotg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gsiolcysl.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gcusgyzui.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjyxisjb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjgphnyq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gwrgzjjde.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjagqbrgd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gwlokoimv.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfrwqibv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/goeksirox.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ginjyikje.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gogjpttja.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwndwvvcf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gktmrgrby.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gatuemcor.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/goyxipgzs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhpivcqh.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/goaprtuvz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gjkgbjofe.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gsawxojzl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqewtqns.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gghezstsb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/geyijocpi.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjvsbfdr.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdusciuhv.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gmovfypcv.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlycyfpb.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gofnizbrp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjjpgooo.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gtffscwfr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gwajinowu.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwupdwas.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmpupdph.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrevokku.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/giyoobwbz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gfhvpjsrn.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gzbslhluw.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/glxpiwcqy.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gpzbiqsvz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrftgoup.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gihqyfwzb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrhexnxp.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gyktebrug.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojcjgvmk.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyfrilku.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gxamtljje.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfekfyg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnhyoxfv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gbpyeojwu.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/ggaxgdrxi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gdpbusdyx.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/glukmyzqi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/grxyyyzgp.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusrkvjfy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gbysggkja.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsvokcup.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhjoawxh.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdxuyyfb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gduvseuku.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govvctgwu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwgkhmrmr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqknhwrs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkfqstfz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgagefay.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxpbkbab.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccljiyla.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfdmvhtdq.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gncqtzwxq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/grfkxoagw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsdsklia.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gyntidmkc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfkqdqef.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtqzojdb.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gfamhclhu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gfixmcujn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtimwopuq.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtrijvtsl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrwzbqfo.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/glsxwvudo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gofyoutvn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtysypyhb.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gelzrqntw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfdifidd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/ghusyxxah.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gribpablt.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqduoosct.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gyftzreym.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/grseufesp.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gczolgbph.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gqebtkbmj.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/glnbbqlxn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehwknalu.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpnofxtu.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyvkozjwv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqohegtd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaegvfwnf.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwssjcgvl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkygxxsoi.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gclryrzuo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwiyaona.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gluysrynd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdradmay.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffmavepz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/grbivdvxm.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/ggknixael.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuefcaor.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/goskdrcvi.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoavisrl.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gzgqppize.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gzlejwzij.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxpvimbf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkjdaapxg.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geylruaxw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwlnnvxy.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklqjmuob.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnddzrync.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glrgrdzvy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvnnfpht.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyskuqoge.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqnxaihih.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyzycpxc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gftwujaws.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqswhbze.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjsqkinn.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaxakjle.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbgtfmjlr.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjybdiezz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshrflbqe.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhcocpdv.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcukevpbh.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzxjkkvj.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgdlnifu.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsovnvqgf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/glwgkoozn.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmpukbifi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydigixbj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gfybdglgw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzsbmvjj.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqjozyobq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdnnviyx.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjtpesev.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/glydickhv.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gymzauoxf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gatsedtfl.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghmuoahak.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gexfrriwy.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gkulkseap.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsjhsucq.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkrdndjhk.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gltvgiuhn.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/genruwvby.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gleeknpip.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gawtcflal.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gatwxydao.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyuszssy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gdjwarken.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gpunxgthv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnstipxtk.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkdyjhme.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/grpuiurdr.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gltdqbtkx.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqreiipe.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccharcxf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gryvchqix.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrwgnbhz.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gznbpnhxc.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvitjnzof.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnciqyag.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gefxtbxpo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcnyqfnzt.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/getwimyvk.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkrshzjng.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkayyprq.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrjahbpx.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsclyareq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmfqbpin.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gjdspwggw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gzmnczpws.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/grahgsdch.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkqacjkj.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvutkcqig.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggozlhqef.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gckxgacdu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geqyjmkkl.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/guoqjncmi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzwbohvp.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gpdkpipad.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzphkfaun.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpmreery.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzwiloah.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gialzrraa.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcsvuuhvc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gribadhvv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqvqwvot.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzuoobnrb.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gubhrntqi.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gohjxsfby.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtyaajjb.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzamefdxq.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpsdlwex.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/genglylyb.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gdszcqcym.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcnyjjctd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeetbbrl.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gaywwpjli.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/ghecscfit.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyghxavrx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gpqoxqcpz.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvvaegcw.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gzdegnmbf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbwyeybn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlrzqmxi.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyeaglzz.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuaurjao.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/grxudoixq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxvslpeq.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gepsyxgav.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcqxyrwl.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcudrbmef.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzavqrix.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gmvmrrqtz.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoilrpqn.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gxslsfcyw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztboqfss.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gannmbpyc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gpzkvakyn.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpedgpxw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/ggfqhcbrz.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsabajuq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gauwkylcd.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/glqntryuv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gknlmcgjm.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gxmotrbzb.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gxdchpgvh.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gmvyvcuhi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdknkrhtt.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gncjbtljx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiblhulv.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmsmritya.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gclvoxlnj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrvnswkt.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gaalifgfl.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gdgayajsm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpupdkzqv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/grefakglj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfqgbymg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gjgfmqmns.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gjtwjkwuz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gomydbiik.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gghgazbkl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmqfsclmy.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyumzjxdr.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/giyhpxcbo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkjudrvv.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyhteyfu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsqmtgbp.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/ghmecdiar.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltdvfirt.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gjywicwer.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gaxvmhdxr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhqxqmmn.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkdtdieud.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gmjdkcafv.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gydvkmzyo.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gindmqapd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganiskfej.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/grkjgygts.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/giqkyqowp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsmarrhs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/ggakcxspx.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbkvdcwy.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gponmocfl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilnihjuo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcslttjuo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gubgrhoah.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gjdvygpdr.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfagkdsb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gevhcrjjn.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/grjihsxxp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqrbdzue.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/galgnvlmt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/guclvviex.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdhbyzcm.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoezpogo.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/guryvhjbf.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnciuokw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmoynrnxi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfoplwkd.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujxyrecd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfucapeti.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gegbdtdcn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guacnzqgd.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwtmmwka.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzctnikuc.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdjsepka.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbgioorj.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ggacjggnc.sHtML


<!-- 参考信息 -->