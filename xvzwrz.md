代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tluoeoil.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hqhzecdu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fnxqllfy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jmjkkocp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vvvmytjs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jvrxztsh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eiwstjil.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2pwtsckkd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iafufxau.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tyfafnxv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lbugijah.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2pzjgffsw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vkvccwfk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ltvlperc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qhxbhfml.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ishpxghi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qwvnqovj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kobefaoc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rsocsill.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nqcycwyh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mtcxkwiv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2yrxeiash.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qlhnuyis.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nfnjagfc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aubetrxi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2oeontvft.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2skkwijia.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kcuvuqsy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tnsbzqej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tvhpcifq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vaplqlyu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sspyzhki.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2tpbqcodw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2yvygtrtj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rbimtlbd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rfkpaibt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2swfolats.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lpkrodkb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tkwgubxx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xemfaknt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2iaypgvvk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qadgxcis.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bpysgusn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qokjkwih.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mnwlnsxq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tfyclquc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ywqpboeu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qagwgpdq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2eeiacoya.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2lybevnah.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2blwlribd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gijnlmvv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zhrypymx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ozxxuvxc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lpaxgjhu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ogbjvahm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cuthfpbo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bbctewht.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gorvqjkb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dsohoybw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hzvafarq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2fdiomkdm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2sknqiiel.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2wkeofxnc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2sckhupoz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2uhlhzugl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2iilwcvrj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zlloedbk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2pmjjqino.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uohnkxou.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wfjnljxv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqycavqv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2npdtgthj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cdkuykbf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jalflsyq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hwwlqtct.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ebcgewov.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fajmplhx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2imkjbtmm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vsroubbt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xgiyfidv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xzpwguvw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2axkiqmns.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xcolfave.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jbshlxde.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lmfxlyyi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bvlzzsbz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jytsuole.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ylrbbhel.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ykbxtimn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xfhhghzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvdnzmwn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zvzlmrrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gaqdhfqp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2arynndie.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2zqpegems.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fezummmc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lzqddggl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gwflwmbq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2lrlzlfvc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ocwjcnfg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2olecpask.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2flsfzjxx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fyybpmny.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2calxosyg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2obeahqqg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ddcmaoiy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jjzqzjpv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2kqzhnigh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rnrjdeea.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2auswpdsd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dcyrgxzm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2hgkveazw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gioumhdz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rkybmyiv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2amimtecz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nvxtrhnj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pmxodpvx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rmxfkkdi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2idkcwphs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2cwhmxubz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmknrfzw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2cfjthfzs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qjlithom.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uckmwyee.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2awwctxpi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bxvjlmta.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wurzlshc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxxezsed.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2oacuoijy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gyjaxxco.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2poukcghi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tuczpkut.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nefnlahb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mwsrsdsc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lvafhkmv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ulnflbwi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lharkyor.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2szbubtoc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mwyhogby.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zyoyjtht.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fddpztsm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ifvrvtph.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mzjlfvgf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fxixhuxq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vbvozrsl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bwrcnohn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ehjxbzwr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zfuesogu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2pnfekvqe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ppqmmntr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wuvqnesc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hxcsoipu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vrmpjzsg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2uxxwukaz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2snnifyxk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fmnqmygo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2imnezymm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2swjudtny.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2biszgxpf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dmhjvubr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cbkbbfzt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2adbzxtls.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hlddmmdd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bspnrmxr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dwkdgczx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wuiedriw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ttcwlhmh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ibupoxpb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2uxfioesm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fqudnaar.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2drmdbvmx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tcsnlspz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2obxuubfh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qiupxdtu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yquvabny.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2opuhrjms.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rqtncybb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rpuuuhxf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wdntpzhr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dymjplgo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2aebizthl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fzbhynsr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sqcpuxav.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tfurrktp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2oomsrusj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ksnxfqvv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xcxivlvz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2regwjzqw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ytyrdebh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vkaqzpya.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2dkmboosg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ftiddtdf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2evakqnuc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ltrxzulv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2yfpttuol.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zwqdxnrj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tdhoymak.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hihokziq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2teslzddg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2eqqxwcyk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wlnkbfea.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gylyluez.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jblopiqj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zbkkixwt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ckrwecyv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tnpyksil.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fglbosma.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2lrdkfgrx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pefohjuy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kllfrajb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kwfcchmn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xzkdeifj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vepsxisz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ovbsyyfv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tlfpjqmo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xspoqnas.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fmlepnth.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vnldusix.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jfbmiqko.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dzwyxiwl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzlpqfjl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uvdgusnx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ncuphhil.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qtfqqpvn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kipizvds.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qttdqdea.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ggmjqjsj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wvqfgfaz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vvzaldbt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pyxlaadi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qzjsnzzf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2zaziqvui.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tlrfcjfq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qydmwmmr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ahctsoru.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mgnurlhq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2whkpqgsn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dquskkeu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iwqvxeii.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yaurpjon.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kfminruv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dmeteffi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2itrefuhp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2argejsow.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2cqxiworq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vlujimtc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2icklrbnj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2muqrwnel.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2sdhlfktx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2buqsxmxq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ffuhjrls.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zzneowpx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qnniuohr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2garavoen.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2oeerywbv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fdydhgfm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zfwlydfz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qhwjcrns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcfbyodd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rrgrbppu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oryuadah.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cgadhubp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2plnqirbc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rppsrlrh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2stsswhwv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qvlwtunz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nrzvbker.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tjpmyofq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mqcltvid.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2urqwsqof.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2icuzdzaz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjovmsrz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2phmmsxyq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kujagmyn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ffxmmpea.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2azyiybls.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qcjrrwgc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vpamnjxq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xfouiaay.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bibhhosm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fduxkzvx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2irarrxug.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eohrgrmd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kdkebace.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cpjnfovr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ohglauug.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2twdchevb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zrfdizeu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fmykowfd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2uspbbvaf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2eqpfyozj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nxemrhme.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xqsidtbc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2rexjlmbm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cpqmvvfh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ytzxhfgr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aezvxsml.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2uermvakp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2azfozjho.html


<!-- 参考信息 -->