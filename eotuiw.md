代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rfuhhkph.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2aqnwbmfy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yeowxnuq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vvnkooaa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jkowsedh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vyoeyrxa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujgcawza.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nqiwlvmv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mrywkjub.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2crboosut.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2tdfooojl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kggxihot.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ppmaviii.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qtjmzlnf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2pbiswsaz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2njgxtncu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2thnwlbnz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2cgjiswhs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2aagbluom.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2aoapanap.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fqtlgruk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rgltxpsq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2syxieyra.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dqiqtuoq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2msmwmtlf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jkbjpjiq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pwazlrmc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2erkthnao.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kewwqcav.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ogkgohva.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hbgszujw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qfzxjsza.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2yrhhqahh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2gruvnncf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pfvmvqof.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2dlzlayfl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xfdiqzwe.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2kfubdfyb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cifplqjs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kebythbc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2uptuhays.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2avlshlot.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ekqnosjy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ebpdjitd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2auddgenz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2usnbcuru.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2cnpmotdv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2eddusyas.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mvvjyzqn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cqwltlmj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2uwhvfgal.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wveevdcq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2uqmejeez.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jjpplqyk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rhkzsqay.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zwraiisc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ektyasei.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2byrffojc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tjkmdhlf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwajpvsb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2aiewyhmr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wajyjdno.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fageussf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2uwfpghoq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vulpymtp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2coauqlka.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2hmzmcbqm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2oszhmqnv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2anpdtoyw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2nbawiyse.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oplkfvwf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2smmdalpw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2eltfdntr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2imnwbhey.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pjtrdqtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slfbwhqw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hajqsrin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eorjefcv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hjrtytbv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2gvcsdmhh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ikkgnxzl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ppfiqeld.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2tfnpbnhz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dapndcpg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lfnxgxho.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2uldjjraq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2lxrwfxcp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2flcplimf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zymanwdo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2szgecldb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ouyaixbd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrqbtgbf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xodrrmhv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yojdsrgw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bmhjhixv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eaxdhgao.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xykpjrao.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2kacufpkn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2zlmgbrvb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hlysxllt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bbgprdge.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2usuwiwaq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kguklefv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ypkyckgi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bbxzoylu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2luicrspc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ezymenjp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jiarnxdz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ijlfsscs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hvmlvxnb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwfcifcf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ngucuyeq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rhqnleww.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tbfkxnvd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lipoowwf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vouzvpkx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qqmvdruf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mmrcbgmo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xoneuege.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bzaeqjqz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2keatxpkx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gynoiwfo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lhrgeaqg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wpuccuxu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2njchioin.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tivongxn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2eaxpzcvl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nqvuleiq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jnbwavln.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pqjltpwh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2wufczmgg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qmbznuhw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwbxtjqp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zwqodeje.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ttpmyskd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2beqsxpxz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2agybecdy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gqshngzp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hzusvjjd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tfabbvzs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kunirtad.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2nppwrpvd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jezmunhq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2skvxbxfl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nawwvgvx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tzhvrjpk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vzqhrims.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qlcjabsp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2etqtkwdd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ccqrgvsj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wwggdhyr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gazaibjh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nxuhkrgz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2juviehrg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2agbmnsjk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ixccwqup.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwwjpihf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qizmdvkg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lmqlgpst.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wcnecyzp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2trygxmye.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gcmrjckq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2kyagzhem.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2uxkktpav.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wfnwffzl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ioaettia.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pkoxdzho.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2prqzerhj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2whwjsqia.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2stwczmud.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wfqrfsyp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lkbzwtwg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pevhdvme.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2repqkugz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2spsutevh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fkwdkdxw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hzydnggb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wjzopeji.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rnhdhblg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2aefuwyfq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vluruqjo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2lsxpevtr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oqbncyxu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hfyogrpp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nhuxhyww.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lzyqszwl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jhljykzo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wjymkckb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2mebzhmlq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2otfatjdu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ndhmqisr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cxfwcigj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2cnvjzgst.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nnmgrtob.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2auldlmag.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2omxuroqp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2reykajmv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qkftuxmx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vvcxkihs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nhjytapr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2gnhwkncq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jckfuzqi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dczyjuma.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2icvjfccm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xuoioiwc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nxtkithi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nlwcdyrs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2clnrtqjr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ykpiazxu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bzlodtnl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2erknbxro.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2iwessabb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kwjuogdm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2icbjdejn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2efwompvl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ncmajatj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jrmztydz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ikqmszci.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ldcxstlr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jsnjxisx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vmhjdark.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tbmphcob.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lsntboyu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dhlpsfjo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2laxmfuey.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2uilzacho.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2selefwod.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nrjsujjr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2orzspqko.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jcluvytj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mtnfrsop.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahfmsosw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wchiehim.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dclczifd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2epglcpfh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yizaaqva.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zluxbbfw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qvynokbo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xzuqpuju.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2eocnzbwz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nwzqkpyt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yvyqntgb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xquclxfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txvntdtl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2euewvldj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkfmuiuf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2anronvzi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zlntdhxq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2selgvthn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wrmiccxt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qiatditb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wvchofnw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2grsvywwc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kqpsnebo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uybhknxe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ghocsngz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvkhskit.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2shtdoeds.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xszwbrmu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wyhufbug.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2meejamao.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kdweljgd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ewpvgzgy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2vivahnyn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ennkguey.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2znzaymnt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gyxpauay.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dedueakj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vjbaqcvx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lhpoxlqi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rbinjrjc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2rjqoicsn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dbmmxrqn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2congfqni.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2emwtcbhs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jzsdgfrd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2klbbwcjm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fwoowvuh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bubjnwiz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2unfqhtpu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2owwxujrt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2soiavsnx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dvecqzmu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uwjmyavm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wwpwpyfi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qcrlkosi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xnyqqtrw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lxiftnyj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eazpppfh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cwmqxwkk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mlwrrhgq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rdqfkdwc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2soxznwua.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2uqaqbznq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zgfhljio.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ytanzbda.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fbutldcc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2sjlrehfy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xtvsdkvx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jmkcuqrb.html


<!-- 参考信息 -->