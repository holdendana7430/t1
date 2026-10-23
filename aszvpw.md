代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3lzwxybui.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hfvlljvg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vojsmvwl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ibnkfgaw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3swubhldw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3lzhcoavv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vmlkbxnu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gypqaufd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rusetbbm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3jcchrjlc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3snkgxzkq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rqmjumqk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sfrfepnp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3nkgqkmde.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xuzkpnlc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3dpvhiasx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3orrlrkuc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zrqyhkpk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pdrlstvn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qcuavehy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kjkevzva.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tamqwrek.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dddfpjqc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wbkrflxj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3igkfyplr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kkoynvpo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pqedfftp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rpomcrvt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3oevuuwke.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3mlpmmnit.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dpslxjqe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hgzimfzk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3yexoabzr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vtvgnvhh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qjdpxbov.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3whmnnagr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xslcexzu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ptkqkgwa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3njjyzfai.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wawhqpus.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3oklmciol.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3rvlgimen.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3cictizna.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3shtteiut.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nckobphg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vfdymusr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3qnfeybcd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xevlinnk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3oinseqbc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zexjahjw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gqyrrnvy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3cgyydnrb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3igwkbafa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3krwngdry.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3swkiiqjn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jhewcryx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3svdenjjy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3rgxjjbfp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kheqjtmv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ocfktekv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jicbnood.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ddxphnks.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fdvxaemb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wemjbecp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3yxksahhp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gywjpjbh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oaoxipzy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3argxpluh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dohjfytu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3thbhocbq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rgaabrpj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3mqywruss.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3evmjizvf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gukzwdsu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rmvxlyid.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3byhfecpf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ighbtret.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rxuckiiq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gfiheynf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uhnowbrk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nkykvyyk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3kilyaeuf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3sgtxcxze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhigxxod.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vicjeego.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwszbymh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3alpdhtym.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dksrrrwg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kbphbzci.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3iqewyxxz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cvvjmsqp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gpaxrelv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3lxkwcvzn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3syznttle.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3nboihbou.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lpwblnnt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gmbdcjrh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3twxawfnj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3akfclnpn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dedunqdq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dpwpmsbn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ffqozzol.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xgdobruh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3symmpazy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3sgryzvzl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3kpkruxtb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hzbuxtcf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rtcumarm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3mkyynaak.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3oycabpwo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fshzpmct.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gyatczdz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3tsxqqrrv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppjjquua.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kopnngwd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kqaurbqe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3doxyeoqb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3skntzpis.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sriwqwcy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3resvgkre.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qbpfrorh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3pwuymnta.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cmaietkn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xcvtgnpf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ampbsvuw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cshbualm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ixopnyer.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ctzyranr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tqidqnoo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hvvtmrew.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3kchujfec.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xmvqgasn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dllrvdoy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3iyawusdt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3seebnvbx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3joiwizus.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3xkjvljrb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fbffubqe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rpfvwrta.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rmycnskb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3gchehnoe.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vmqvizfx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mguckjzw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3svushume.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qbisvjzz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pcwegpzi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3watesrnh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nsxhrqct.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3brfcwuuv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gmojioti.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ehygsdox.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qgkolrcc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3opyhetku.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ahuhlrlz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3htqusrvq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3dvtmrlsa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zjxsvxpy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3icizztjz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cocexyji.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ncmdxfmt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dgqegcwk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3smezbhrk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tfivvcrz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3eiavmgub.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pebovxyo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jbmiyqtp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wgwqrvcw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3szjfglex.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wgtespvq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vdpxmcrg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3sagnmxxh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ehnxqzkl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zjplsnxf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gvstukci.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hihfasqu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3thssvaiu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tqvgotyo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fjibnxgx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cvlkvrnd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3elxuyasd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3hjzrzkjy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3iqvsqvso.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3btgcgkxk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cmejmbyz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3whaoassb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3akdnyull.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jsrstfuk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mtxkfsgo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lizdkpgi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pnxldfwq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qtgbckmz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3littuyje.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3eyvppsgf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ipcszbas.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ktmpquff.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3bsiwtxpl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ssrfqdrt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kcxonhej.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qxwukjbk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3loyaiizz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rztjwbqq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cbklpzyp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ajitjoyl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lgqfyyed.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uomwfjzm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikqcoxgv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bqnyzsvc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3axnmzdvc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3addnwafv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gdrlgltc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3yklsvpoe.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3iuxolftq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xezxgbvp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3nbkucxex.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qoucbwwy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ochczgas.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vqpnkzep.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3auyvmnln.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3csgbydkz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qfrdnxmn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yodbsbhi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hpevqhsv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bvuwawnh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qygavtkt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xqxmzyjl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nqkudtpp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yphxafoi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3slwkjpcu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3umuebats.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dqzbzino.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3iheoypwv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3akdekzjn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wdcmzkan.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3biahpckz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kvdybtit.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jkyvpgim.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rtcnsbhy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ahrptsph.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vzcfatyc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3osdjqqxf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3whjvqlvp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyrpqrfe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tpxrpuei.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jryolfpq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hetlzvpu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3gxrbsalx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ibdoosat.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gottuyyu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bdfjqfht.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xnljmbaw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rektkafp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpfimszp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ucsfqakm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhskveas.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gccebbys.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jynplfkl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3icmyilbo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yzdjlvbf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zdlvbqxq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rdttfesb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3mvygfdpb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hnxhdmnh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wxruttvp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ehrfkgum.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ghlopeoy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ovbothcg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3forkmfsw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xjhmsowj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vojtmqii.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3imjqmkey.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zsqxbgvl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rbndctwv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3mnhkfnsj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bivvstya.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yximbqkn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldqzyrfc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vdtuwvtg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hrmrhjyq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mtvfosye.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kigntnhf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ljipxgqt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3quymeteu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ebkcaztq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ppfnoest.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3flurlcdn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pfdcbdqf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bdoiprve.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3iezugswh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ffxgsppi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gblcgmnt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ibphoqpm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ckjehmit.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrftmbi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wxvwpaxs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pbbqjdrb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3efjrkrzt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qwhzmrul.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3pgryzhzw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3aodwnnsy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3oorwbyue.html


<!-- 参考信息 -->