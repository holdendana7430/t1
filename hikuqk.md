代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oapkbyls.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2nyrvkckk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sswjibtw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2tsrsaucx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uxmqghwe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2pqhtcqky.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rlwcklhm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xlipdpyb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iayfdyuo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zzkwetuw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cbgsgisx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2lnqlcduz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ibtqwmyy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2leaxacdq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksoemymc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2igdmxelp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xfkiwyov.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lyrsvrca.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2obtiofzs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aesoigej.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jbxrfoow.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zzlnwapl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2sdblczml.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cticumhv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bvlmonrz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wheepuot.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2dpxjubrm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2spniqozd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jqzffmrv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bwahrkpw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vvecball.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xzxhobsw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ksgtumwa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jmmhrlqs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2eqtdlrni.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pvgcgpab.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2srlfmabd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yfzujuzm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mkcpvdrd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2shvbtqdm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zguohrly.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2pohkdqpo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tfmiadms.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2jbahzwrt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fcpnhozl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bwjrzmvd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rjhufshy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jrduhsen.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xyrsibly.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2trcwntwz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cnsgmusv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ngtsdgkg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cvddugxt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yjrhvtun.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pmwnzzna.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2askqiwfl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2epyacupw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qbdjfmrw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2njnlylzs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kgxosulm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wfmshiff.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brujhzhr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zslveown.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2moudoakv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2evrrgoyb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2unukkysv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yaqebnyn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rtkzgkdh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2odcjugjm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uoejolxm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rljkllpe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mcsugvig.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kpsomhpl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2yfzcknmz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2coqchubw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uxiplyls.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qgjckduo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tfzltikp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gfmftvtu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qahnlyoy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ekipancd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2etaenuvr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jzropjfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxoaehcq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2dcuijtrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oogiwwdy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2uvuhybvg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hhfcsklc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2spvivlwc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qvbvvokl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xxmnswuy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2czzpiuzo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bfpgaamj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qqxshlbi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vgcsholr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2teaklrtf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jxdlavxc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nopfeauq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fesdsyvv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jvewyyji.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ihjfijyg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2efqtvrim.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tqtvckja.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ftxwhzdc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nnpsrdiy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qovtndfr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2unhxcxfs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xttciwyr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2chavkzkr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2uknxvzgd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zrklgxal.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tkexqamh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ibanmxxx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xffuneik.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2lqnofycl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ntipiphc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lttjxgej.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hcyuffym.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2prrgstpp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rdgtzidu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2clsiqqzh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2expywesu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2znwfnidm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bevxdobe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kznrcylp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ihfaqiga.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uamlosum.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fiaeisuw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2blnpxftb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ecuyowwk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xqznrklg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hexkcibs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2dfstgmeu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cbfzeoni.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ohvnpdbz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fcqyssjm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cbgqlbho.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2totxkqom.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pscwaxif.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2whrfkjge.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cnoupthf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2lcrsnsjo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mhjlplwx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vauepbrx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2konyhbud.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2okojbzod.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wbcrazvv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rkqmaddz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bmhvpdqe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nzjetotk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2crbazxeh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jydsdklm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmchprnq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ypaxrsvm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hdvudtlc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2luzepypt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2auazchtv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rbwmgoyr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2irjyrmja.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2acrvihme.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2okljlveh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ajzidzas.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2eclulojl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ffdehork.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jfibxluq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2darlniih.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xxyjitok.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wfpbcvxr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2izzjfxpr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2chpboggy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2owfukwlh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2aewxhrfc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kwvrduoo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rjtwcuos.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2dykxzwlc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xjdzhpnx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2soykwlis.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kypyoeyq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ubiccpuo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2esmdopgk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2grzuilnv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mdontpcb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2spvceptv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2lhfdvfvg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2evuhfknn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2liukroqb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ohqonraz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2pwengeyi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ajrlibut.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wawgugkl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zqdglpdf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2uyyjvssw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2uqlyxhju.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fwgiyxwe.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2oicyiyjg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zqihruiz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yxovxlag.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dkdqymcf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iivqrmlm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ioozrqsh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zzrvxqdz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rmhsmgps.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qbbonnpu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2pbvpyzue.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ivygnutp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2clqxsvjp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2eguxgysc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ylspaonp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2cuelfltd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tsjbzeby.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mnvmlbiz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hjedygah.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qpazbvxn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wtajkfpg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bmgoebit.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pusjjaub.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jjjfzshf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2tiydpogo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xgtqvcom.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ggfehxip.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hbtjjswc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kithaktv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jiuvcert.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wjfieejb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mqrbmgeu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2puhfamho.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2flybnjyv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2abfistvt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jcnudvmf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2enzbvonn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tbdwmhfc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hurpzpmk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2chqfkknn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yyzbbump.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2evrawsei.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ewtyzopy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gdqqlumg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jrtkqqnh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lsywlauf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zvatdojl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ygcxeatx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ybyajqfr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gcscgtww.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ffehbcew.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jexycoek.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2oazgpztu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tfqmokhr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2aibgocjt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nfbarabo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yqevohml.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dfcvawnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjdapgqd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tzdchozh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzapgyyd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hbzthqvl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kgphhxnx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcangnmt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2njvuauhw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ohocdxla.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2upwviulw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uvxdczab.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2knomofci.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oczaqudu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nbssuoiu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vplytegq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ubbhaolu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2adoohrkv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kdlcrmqy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gckxrxam.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lzevzetr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2cmdjherz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fmnjgpjw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2spofqrwt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2iprphxil.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2oqbivzal.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnuyxnkk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mwzhmwns.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vstsybcd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ocumxiav.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2aohianyn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gestcfgc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jwatbnix.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nqcsnwzn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rlevtezp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mvmsogqk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rniqoztm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2lprbbjhd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2thatlrtl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wgvdovqq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2syfoyzxs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gjdjffnu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2exvcdzxo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zwrhfwcr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2eeisyvnp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2famauwvo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2quwecdgv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dygrgvrh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2oyslpctx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rverbyph.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rzwkkkgk.html


<!-- 参考信息 -->