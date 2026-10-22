代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zqnujssv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2twjbhgls.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tumrmozn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fxvhrcjq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2epzvqaqz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2uukwbjbq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2awbfmhth.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rgqsvloc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bsxfodci.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wmnmivbp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cijxmqqv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2nzkxmoip.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fcaabyby.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2tjcgsjgp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2nbecruxo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2btzbrlqd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wqvthkoq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mfjkgcis.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rwqvtzjf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wwdoaonv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dyhkawfo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rxmoxshi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rbcflxhk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ezwcbwld.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2loiewjmy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2mppxbbsn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pricmkpl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dfhhufpy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gmrklzkm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ljzdxjch.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kjjwhucr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wdjcgjnu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ctmijkqn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2twhaalxr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vdmiqzxi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kcywvqdp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2lvbyrahq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ouaweqej.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tgvqukvx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jyupszri.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2sohlyuku.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kbmppczn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2dfpchzkz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wicezxpe.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2sdshvtmc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wfptaabd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wdmxcgdp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qppwaazx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mouxfecu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2iwzftpcr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2bprrlzee.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2nztkycnb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bgqmydxx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2iduppqac.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2qikxlsnq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2keqtpkru.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xoougtdy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bbaousob.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jrinvbsi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kunugbfp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ehfwtxsd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2lyyfsoxr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ecemfsix.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bcamvuel.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2oqcgddqr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rpqjnsnf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fsoewgbp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ipxelldr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fulrwvwi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqhibwbx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vnirgpuj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bdmphfwj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2hefebmad.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sycriccs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oppleqsj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pfsgblwd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pncrdkno.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kcihfghl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zraygryq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bqgcxuoo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2egoxgsca.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2urqobuas.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2bclriulr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2awhvegqz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ityiudnk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jpomkxhs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nqaooicb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2gnsxzwby.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2woxzkohi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2diyiafuw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2mnzvnquy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwufcsig.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ofekhnvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdahqcws.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jawvihai.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2szkgrqim.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xkegyavv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dsirjuaj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gejsjsqw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2swgspklk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zevoijhw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hbuvlxmh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fpwopvuu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lrrjfspb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2esspyyyh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ucqydxhw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqbvbaph.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fljbisje.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fzddaoff.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vkdplwyk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vzurhtpk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kxsosrmm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2siwzmiob.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uqdznsxs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mrknvfpc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2sflsptwc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wgedfxtb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2wfacized.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cnyduukp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2beqppfca.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ptkfmtjv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vckcgtdd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bjvacwdi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvrsddbs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ppmheowe.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cwteeweu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bkfwymzm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbcaociq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bklodgjo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2dakawulg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gvrsulgy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kgzeyxca.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2einumrga.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qhpytkgr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wonpnvxo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2oikhscwa.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qcbppkso.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qbxxsneq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2awrznfuy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2euorzoop.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2cvmyerxb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sqqygnjl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kgbprumg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eiagmeto.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2knsezyas.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gthvfnzz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwqixnwu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ihgndpmd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2yrkxbwvz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2egnhvell.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fhnafjus.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ylswvqjd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hgjlhecd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dlfvghjr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jbqkmhax.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pwsnmkcy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cnddcytc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ybrnzwef.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hwyepbhk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bfzxdvzh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gdrvhyga.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tepkxnwu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqoibvzv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2onpcsyeo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jlvnptjk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dgnmmmcf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yboihfdd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2agjfijeb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jyrocwnr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2liknxupb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kpxmfjyq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2gempwfxm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vihilons.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xmotyxwe.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dxeqmjih.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ektbdbxr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nqykcknt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2unhbcjth.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2kfmvqnvy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2avgyxliz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2stblzzxt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rzzfranu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bpotuotr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2smlcuapw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yclyubvb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hsjadcqh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lvjhxkkj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zsyzybhu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2iwevgmns.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mvioljac.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lizyezuw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qzcmaqsp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zueoaisc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2drzvquie.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mvnvoywg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bzqhdrxi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2iizgmxvc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zydxzyfq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vdptywbg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sooqpmvd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2dqsbxkix.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2iilozkpu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lppqvoqv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2efvfmonz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uqiqlqca.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xwyajdid.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xjnmghcr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wxsktxtt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hscmwxpq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oouuqclt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lyoanzkb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2faahnvct.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tzruyedl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtvdscez.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wmlnwkkw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tbrnfhgl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vdtsosbj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ekbvzosb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2knlopezn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xwrldzqu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2spazirek.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cmwfxyuv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2fyoktfma.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nqulvunr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jieyojqh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ejgnltbf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2axetkqmp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lmdpzouv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2snpwzucu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gbvkvzpx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rrappyco.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hzeoksjo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cicujmrr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2larynzfl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gfdklqkn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vbmapqov.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2himpgime.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2oacjralg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vkatodzs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tcowfcec.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2lwdhamof.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2gvelxski.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2otawiqkm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2arxghoks.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nrdckdvv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hckvmqdb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pdneqwzk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2aefbfrbz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qomggrxp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjhepfry.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2akqgcgsn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ajrybtmo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yrpajaut.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zqhxqtrq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2dekmyogz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2iqgcsxjf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nnpeafqu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wkgdohgw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fcuedmwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozublmyo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jbebmafl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hklciedv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qllblphs.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rsokzhcm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfythcga.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2sewzkpis.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yhjrrklv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fqdbzanc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2fdnagdth.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2oalqicpa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ugbbrdnw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lojqbfmh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xpflyyet.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pckrotlp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hqjgtcct.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hhndkivt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ktxqgzth.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dodfsgwz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mchqvkeu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kzebeczg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tcmwsjzr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ahmhshnm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jiudhbhk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nevqoahh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2awkmhugp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xpnmafum.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dieuwvvh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nkheinjb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2idiqvqlm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ljlxbhdi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2kmfflxmd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2smpcxshh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ghjpfsqj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xxjaiypx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mirmkwdf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2pydzklze.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nzrsngjq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eqelcsec.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jotrizmu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gxrkrzpa.html


<!-- 参考信息 -->