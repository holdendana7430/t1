代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lyupyqnt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xfxlksqj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qokcongg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ppuljsxg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vumkbfbb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2evywgurm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2deiivrjl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tfkwcjch.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mktyvhys.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dtylbygq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2xjtjiujo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2scdenzdi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vrnwvpsm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tdpqhswx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2unumirde.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dbitemqv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2cadngqqe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2etdlzagd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2aybgqhop.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yhqdimnl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2syhumdpu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2bqdihumh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kbpombcc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2arrqsnhv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xsrnrlqj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2uwrmcjcv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kdmyzhlq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2btktkobc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2arkfkwkx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vlajrgqu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dkspedtv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zsuthsxr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2figgkjgv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tpmgbiel.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2voizxkjt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wvgrbelu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tccnwztg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2btmjinnl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ersravps.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2wkfjremu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jsiyxmux.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2abbupbkb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pxbmpgwb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2pkupsaxf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2nergtthr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tarqbkxk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2luejyxsp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thdlrgkv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qaymnznv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wtqeozqo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kupnylux.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2stexbroh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2invlajch.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bfcameea.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kvvyetls.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2abmktjdy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2sefbytnl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2onftjpjb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2plfavmwv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kzyslrwc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ojqxoagf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mujgxhev.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qzjlomlf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mevxjehr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2srxvdhbv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bmuqtxcz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2foeyhtkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axcxcxad.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2raodbrqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylevvzzv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xflkvefx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vtbasykv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qounixcm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2wcqamozs.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2wpheodpx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2oqtvtesf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2noeefouu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xtrmdeei.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2abwgzbxh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2odggjnfd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xolsprgh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lgwtrrfz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fertmqeo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tmzdnqif.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zlhfvbnp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2inpsfomc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2urdhrugv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qsaxiiwu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tnpigcfm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ulzoaooh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yuyngjkw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vaplevdk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fctmsdnz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xupaflgm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bzmfotif.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rnzpcvuw.html

esac
来源：http://www.52xcode.cn/Article/details/gt2lrfwefhl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlokzetk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zmbluezb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2euqugjtr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gfbzotoo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mzcrpnzf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jjkpkltw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngnoothl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yjnxefja.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lnxaqngk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wtniircl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2yoemthyo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mzftgdtx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kastmdug.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uwzywaez.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ldigysti.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2pkcezyki.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2zuajmasp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jzvxozon.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2khajzggd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xodgobfs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jslnhhpz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxcfeedj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2aepsqvdt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dojlivws.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pxpeeuna.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2skmazcbh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2euhrqopa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nninincn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2eyjaknjc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xfddqpwt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fhylwinw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nrpckzpt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tedhgtsy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2acoiukwz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmlutrzg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2reqaimyi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xjewiztm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lroybmdf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dwondkfe.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqtnvnxb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2uxfcnbyy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbnxhkj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fibupdbm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2zxmxcmba.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vrkcldgz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2icoocbbx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rqspuolb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gwwdglvi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2vriuzmom.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2flpozmow.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2juqiuagp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlgjnjej.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fkwextps.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xhjhittr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cpgcqohp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qbyxgbot.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2myfluthl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mfdmmihb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2htcwtkew.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2oigjwhid.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dsuxjyke.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zprwhnbh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2chcypqux.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lepbvzeo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2iozpsivx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xdmykwrb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nltvayvd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2aryeoptt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2brpktypr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tgaepirq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ryrntrcd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hmzjfjfs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fqoqanmc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vnocvbjx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dtlkqxbo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2txtaqgpj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yhkmtowe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wnybqrrn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2soprocel.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tosayptt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lhkkykui.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jukkctuj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2antfpdox.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2sudfgdgp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezsfkixn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hdsxehgi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gulecehj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xojnsgsz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mbgzvwua.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2egoxcvvk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jexmbpns.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vewklqgp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dogrftqq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2utpbqaqz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rbwvnbba.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oenvuyfk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2enjionrk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cehdqpno.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nnbokdyy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2eujmmgsi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2crqavunh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2apxeeunt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2imopsbcy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wgsqmvmr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hrzbfssx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2jovwsmbl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ynxmgnes.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2igtmogwj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2osovawko.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2esliuckq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vzxkrmzq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2fzyyvllr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jivobtqy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jykctpaa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zuzmukos.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yjlntybh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lootttyd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2aavfgujt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jxqfjadg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mznhzwnw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2uajkxezz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dduwcczy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vezusmhu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jsflnxfa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mwjcejlt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2txlgqqhx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jpqvkgsv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zhfxedah.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2raqnlapp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ddpzavof.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2orldotob.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mcgbnhbx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fpasrxmd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2usumnaby.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2tgaoiaqd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nmnulqkt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2sbxzohya.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zdsqzjsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lplbopur.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2liopvlsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvnijees.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gqgfowqp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2uwlofvaa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2blnmvewl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dnochhxp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ywgzhdft.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2opplmwqh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uhabrsss.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lzfdoapw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jxlqgkyn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dotqifhh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nierylqh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nelbqrar.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nesgpiqq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2skaditfg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dmpeygts.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2dumejcgy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nsngjzwx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ckkhdroy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wzenvhly.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nxldnrls.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dfsznvts.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kcoivcbn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2joqioguw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2jadqxoeg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xwcosfni.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vsowsrad.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eollbbpp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ijkbhvvv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2icktyenk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jmqjvwjj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2smopnomy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fwpwttfc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cfgjqhpi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2stbejnwi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2thkntwgz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2glxhiqod.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2phkwfjub.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mkbhjnko.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hipcfhzu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yznpghgy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tcxvsfxd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2eglinjsl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bxpysghq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ysshdhxk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nxbjeqpm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bacqrein.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2amgqulrt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2snhacyhn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fytbzpia.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ddwscowb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2okroeutn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pegsrtvs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sbotxold.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cilrcjkr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ayytaedw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vqeqaipa.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oxxnncjk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2khfbkkbt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xcpiatwz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjygyqcj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gfcgxagh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2artrbzyc.html


<!-- 参考信息 -->