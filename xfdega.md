代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yqrfdmaj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2jfbvyzix.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ozzmichu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lfjalhrf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nbfjiirx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vmgrtarh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2urttlrye.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ojhduoxw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nrhtogki.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tdhaotsb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qjezhctt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wppmamyk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dptgfoyy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bbhubvby.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mekactct.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jmwukstg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zcnosffq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2olivdwmd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kutjjgin.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pfcfbtqx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2eftvjsbt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rpozckli.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ujdevrgd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ihlpoblz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kqiowazb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vpsdpqzj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ejqtbkev.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2iadfosqw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2amoluifa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ajxrqklf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cqjlqfjp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2gttwnbzf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2bgfrjmnl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xdzbvnxb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nskaqwxd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2veevjbvu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ktqtuqwy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2yzenygpe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2baivuoyb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zocgijwx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qnwqawti.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bekvvcpg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2odmspwok.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hjkthnwc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cirhacvp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hsmrszxt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2llskvffg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2yhlpphqm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zlndvmcm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oqdntopv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hbwitsre.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2asneqgci.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jsgylzeu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2flzvtlvq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xbkoqsov.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ejpuyehh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hfyqdcka.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hooqwbgs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wisiykjq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sxosebdw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xzkxocpu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eueqomql.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2teqqcdwl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bdzsiqao.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2llafxots.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bibjbkpo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kjyrzmaw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2udkgpspq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2whgwrjbt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2blszwwmi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2trtatbhv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zkfnuwjk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2cevcvpnv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vqgqihmt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qykxqynd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lqajtqlw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qjrlwwlh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2awrxzrst.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dictkxss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uexgqzjb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2forcsalk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2manqcyar.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2yvikyslp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2delnyeur.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2nlskoiif.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ldnqokts.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ursnlcqh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jvhrlunf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2otwobdru.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hsqnguvm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xzsqzqcy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gtkgedut.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qlglqkac.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nwkyxdxk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2secxexum.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pxwgbrwk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jbgzavft.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2aqlujfbw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xbxawdpz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2frgwyfom.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fjrfcekt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yuktbhkc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bwpfjhwl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2oqohmujs.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ezzqrenm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rkbqazkm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ltqyqvbf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tfyrosyl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ippdotlx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhmzqkta.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ceitewmd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2znkvlaxs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2srukrrvi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dbsdxdbm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mdowkvji.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxedpvzj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cotahjgo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cnsidvxy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vpgugagi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rhqlhbfb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dubatruf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vtxletrv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2sezcosls.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ddpgkrpd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yftzkywy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2pfcktmfh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjicrmbz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cyvxyory.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kzsgpdnb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cprwtwuj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vkwbqhyl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nlgcwemr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yrgpxzlc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mqyhrave.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jzmkkhez.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2nvrdtojg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nicebbnm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vlowprly.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2suazqohr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2anufbelv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ecvksuok.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vdsknhai.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2shxdbzii.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xytvscez.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2yaljbyij.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2emcuofxc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2idcthrgl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mvwlzsrk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqdwqnre.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2kqccquza.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wawyskrq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ssmgearf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jgguctvs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mxiijsve.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xiqyxdhv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2iiqupdqw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ijfbkhym.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2prrbnbkw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2grajikjz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2puxcoxrd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vuyctouz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2gljmdrlj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vyifcuvy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qptzqggl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2oyxmasbj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ihtyvdnh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2krktvduu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kqprolpz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tiimvgor.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dyvbtntp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mcfimfsj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2jgchujtl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xxskszcf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bxbnmfre.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2oktxarpr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2gqqnebyh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rlkxyuav.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ibsxmxyn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mrewylby.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2yotbiifo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aqbjuiqe.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2yavdggok.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ittilbmm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dkackfxh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gugxblal.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2blqfdthf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrcqoqpw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cqylsjbv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ophlujfk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uncubcej.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tyndtlbd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2drpdfouo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2sxrtugli.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntgatrda.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wigakngm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2iibcmdho.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kgucxpbm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ouflwmzj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kqkgwkuq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mubihjtc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cklensnt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfnmxqbr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nfygjiui.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ymduncrt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hvtqqheg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ahxdmlfb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2beucngab.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nwwtwfek.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2sqhcooam.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2aycfignd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gnfjcpvu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2npfenorf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2azmiunsx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fajzdtbb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kqywtzsx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wcrbqnus.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2eeyditzv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nwmklnph.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mqxcpizy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2izqfsved.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yhrugxth.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ylpfnzgm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2aihhdjbz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ijtumnmc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mguqqkkl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mainrvme.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lwicyeje.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jlkcuqsk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2beqdktvc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2chfierqc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xhnxewww.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2clbvoqml.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ranlhioi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ayhannmh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uywtvutb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2syhbbksh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cuzkdukb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dnaasyox.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yyuaoddi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ybeehkwg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ymjpsneh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jfkkzqzz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2nphnydbu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rsooedtv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qobsplot.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2uusdksgs.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2qogmjrhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bocpjewg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qsjaqdqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swzeagpf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fufrcrzc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rsqblseq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zironybl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hfnnurym.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2evdhupgf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hnqmvupm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hjsnmlne.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lbumrqcl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2sywqcewz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kmsouvzb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxnnjkby.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qwrdnxdz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dkkqtvvi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2cmndffrq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dujohinx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bdlulqkn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mwxpdhbz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2nxoefkul.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xaanfrab.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2zvktuqfd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pwnyehil.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vnqlnjxc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hdedyaos.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hrakvcst.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ckgqdqmb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2labpocqs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fgkffpfw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wyeaqubh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2iwoykdza.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tpvebirm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mxgxaotg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2piiottmu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2myiqbjom.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ncufdonm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2wlyhynib.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zmlffvsn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xpdafawd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bmiztrcw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hudacgqm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cshqtmxe.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vqlelshb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tabvcgap.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ihguzmmf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vlzumcyh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gheptklw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xtaeznsc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hxpvdcxs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vgfcjsmg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tnbetbfz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tkoehdyd.html


<!-- 参考信息 -->