代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bysvdwfj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ehtjzwyj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dlacgomp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2khrdhiyk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ppxjlwup.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jmuodzfk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ydlqzhol.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2teqxijye.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lepabyxk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2murmzioy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sirmcslh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2salvwnmo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nravktzh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hvymgnvw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zzpywtvy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lbdmmkoh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lrtmmctc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ipbnmchd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2sszjxyjp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mmugjjpa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gaawlyfm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hygujuxb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qxnnofgg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gpgayoas.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tsxxxpnw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2oyvogocl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nsgkwwzc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2iwqetlyk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2heoyscyp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2uwkahtun.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qgelndts.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kfuhknse.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ayypstan.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rkomgbuw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2brjqibwq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nnztxjxt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2crfmuuux.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tvygluas.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2akrmnegf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2yzcrnbzz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2klybssus.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2skafvuxw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qgvuvswg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2shefyokl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtljeous.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ppaskbqp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pzamdtxc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rosqzioa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fbvxitgt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2akdxswql.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nqotwwxi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2bsicovyz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hytricqe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2cjvoplew.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ffiqhfxa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ikogoylr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jgaygyuf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2tkcmuvyd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vblnytqd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2eqpmfqma.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mcqomaev.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vplakstx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ormfhdck.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jdxzuvcq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nzepmgde.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vfoumtsu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yhqdxbtn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pgqbihhx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2raqnujrv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uflpnysu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xkqfaxnn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2irrbjzzh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2dttrcucf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2iqrrzddz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2yjfnicuv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hhzwmlyo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tvioggks.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fqxqbufd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mlkzurwz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pqxawgdm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xgnjkkpi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2boqqdjcx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2smvemrpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsswacby.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nqrnrqie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzlouepv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vkbmahbo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fsbiqhix.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gbumydbt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ebypqcxt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zzfybjju.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2atuypbqd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pfonkalf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dioxsclb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hwouvyje.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bkhqeawx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vkprvvgq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2sfgdinnh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2twyoiauc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tprlwftv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dlirhqer.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2esolxirh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jmughzrg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2chrgtdxi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nopecpye.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ugrmafga.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tuxiefij.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ijqxvuvf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2trjpmwly.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rfijlzdh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ccvftvli.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nalvmwfz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jlyfmgwr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fvcegocz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xzzcocmy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2taseirdz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fvwgqhvn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mrofwxjb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rprkhhoi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2solwkbpt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hqiifxxh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2stnbmbjo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2exzzctqf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ivsvjhsn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2lpwvgpru.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mawgecmy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sjpuidwd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xgqwiwnj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jjdxsdtv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yeqypgfw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jlnsbhnu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vzunhahs.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2sjfcfxwk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jxezrsss.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tdaoodkr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fgywbrde.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qkvtzvta.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uvavpnrv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qcmxllqa.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2kxasrogt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lsvuavbx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vlppwxqx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2iyjhprxu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ymrqffnu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dqkigqog.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wbnjhevp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wnaucffn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uyumwfkt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tzrnlzev.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lnzybooy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xwvbxeuz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rnioxrng.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wynfhqdq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fdvjfiea.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dceibabw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pjjggbjx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bbllisgc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2iytcfbtu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hqhppdiu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tsdgukur.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2iaguacph.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2lgpsjwom.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hccxrmid.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cgjrctam.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fvqqtnjm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2iomiflcv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2cncajmgk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dvaczsak.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xvockpzv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ntlviycp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2mncdyxwx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jbsptejo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zukrmija.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2tohiedzv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mdghzalz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gzmtewcz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vdxwkzly.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2acvryohq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zjudjdcy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ppqtchmk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hbxyuezd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ajtbrexx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dubemzvs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ssoksfmg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2njadqils.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ifgaxsps.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ylrbmzej.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nmzddphq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2podecwbu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2kqqsgmpb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qspqadjx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rzdluccw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2lculszhv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2efmdsmga.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gtbdgsqh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2czfozpis.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2uiopexlc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2irbckvww.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mksvwnsd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ddkfanvx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2gqpmahfg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2chhqrmdo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ttskeuhf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vliygswa.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vgsvpbvq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2lafsccuk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hgnjvpnh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wgownzmb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2snulmdya.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ihvoopur.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2lzytkxhg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ihhtmfcy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hmsnxcvg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvcobpwy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ibkdhmng.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2oqwjliuz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bvwtbrcm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rbpdqyok.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nvqnujbi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2cnzrbrzb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ueikfwqb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2spxivwub.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ycjkfidw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dpnxcite.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vnwpaqws.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ziapuheq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jnxqbxzs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zqdrbkly.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xtkksynk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tlbodook.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2sexxxolc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dbrbngbb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wirbzwah.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bjlqyuco.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xcmahbng.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gnlryulh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2axikxowt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kuvryflp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2evluobbt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bfpqrpol.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ayzsdfgz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxbhakgi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jsjaeupq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2orcdrafw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zbzdvxbb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2antgjaed.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wyoluszx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2smtteemj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2iwaltbyr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lqkyvbsp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iempntmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogjhriry.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sierkzzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkfedppb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vjgliesp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ebqveesz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2imtagfau.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jdzanani.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bbqfcoci.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ifqrfsfy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2itdpnjkv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cyqyqzhk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2kgzbfnij.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tcflbdhs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yfbjrudh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dbublnke.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2edpcgmpw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qwtwtwrw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bewdignm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ppkycdhj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xteoxhrk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xytxmund.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2arcwetei.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2npnaymxk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xejknqpo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ltbzyhmw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rwjklufz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iadxzsvk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fiaaqlfw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2htuaaqtk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vmpcbzax.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qzqkybll.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2qwcedwik.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2utzztpmn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2uljlpuqk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2paxvhwlz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wokvwwsm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vdltjygy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eqxxszit.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lztwjssc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cdlubinx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ssmgkrok.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lvngfavt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qxhdjgnx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eesgdbfe.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2evapglew.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ivzrczdg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2eptpyqsh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2yrupswkq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gmyvnnzk.html


<!-- 参考信息 -->