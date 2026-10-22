代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aqetcorj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2npbxoyxu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ffpxbtkx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2clhofesy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ejdtcqbv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jmhoyraa.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vmcsswlv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rqbuwkxf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bmxyzrxr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2cadstwgz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jhcjelyd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zlwlxgty.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mbauxpwp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ffsdrptq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksuxovxm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dpxbgscl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ekpbejjy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2csfjigtr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zfjsoabw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dfaeqvyn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nlznalsg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mhdgslva.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yozojpfn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vsljrkxl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mclikcmi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2vijoggev.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cqjrkpcy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2chxfgfdg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2agynefop.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2cpwamjjr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tfodrvyx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gztwkdsz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2iqxvnbfq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qfqrbkzw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wfsbhqlo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nemdgqnr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2brioczta.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nncsyedb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jswszwue.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dotzmajv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2sbftgstk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2bvmkthic.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2oeclqjtc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kigervln.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwnwapge.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kosvkrsi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bhhjxwep.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kuwdkumc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ynporfau.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dkansbpj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lvseqtdz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2adzmxgxf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ylvukgbz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2fcajootr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ilbrfnla.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zekxdlss.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vtozydmk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pivuvoqy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mziujspl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qiohqajq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zcynvcne.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kuxphekb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iyjnzcav.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lvjpwzsr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dfcalrgt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2macnxplv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pibzmvwu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gxxnuyjs.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2yvdfgbwt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ziqnfzxc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2okmalaoi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rdhldouy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2dvgzrmgq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gpxbqfqe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dgsqkbgy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qummhgop.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2yqpwaqcx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ymrvfwnx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hjabppac.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hlwstqsd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pdlapmla.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yytxhbut.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mlcvwvfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjxrgypu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pjgwxcwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mekjcjar.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zfwtkezh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mmspmflw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2duuztvvv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ucxptzyg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ihcdwsgn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxyxkjqy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2frdoccea.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tzwbwvzt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xzxnprsy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kpqagpfg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zlsvzobc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2okzcqgfe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2khtvpprp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zdhllyua.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lrrndzfm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qlchqejq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uximlebg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kxslrjtw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2anfkaakx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gvknxfau.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2iyczqkrm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2glgwlsue.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2kquxkhue.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2opfpyxhg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ocaeqmja.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xrpsendg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2natnkxgs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhombgac.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zjkdslpo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gmfocuco.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fzcgmcko.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fccrkuuc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oechrwfe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jbbnlocf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2goodkxlu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nqsgvcwq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ieigqqvl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2gudanqdf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2fyjmlcpc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2izlyrvbm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2chnshofh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bokplowz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkvjsdqa.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jicajkev.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uusomsgk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ihdizecm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kaccryng.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wsffarum.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jaojegpj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hvfsxhyt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cfqutdxq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ubbwpbeq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2phhsnsew.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dgycjpzi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wojhmkkm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mfipqsun.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pfksohtv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jawqtpjs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2eznlfknw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2sgjvmzgr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zhxxnmvf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pxrycbpd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2andprshp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qgastdcq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ifdqhddj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2otjthepa.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bijnlcdu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dlytqiov.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvqbjoye.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2obfdzdrl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rfupwtan.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2oyakhmev.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sgxxbyvl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ytscpess.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ljoxjrke.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2oowyauot.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vwamtcax.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qvsyjnnq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2naienuzr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ckyjfkan.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2sgfauqyx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2yakzvamp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zaiamkhq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2nrbngnwx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2aysijfdu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fqaqzgou.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cbzdkdpf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pfpnyjss.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dofzhxus.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qynfjhik.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2czpaqzip.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hvgzuota.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qggqotkz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ryrpvjmp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2izcewbwa.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pgydcxfc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ypqoswac.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2kjslewos.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hajakrsn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fnrdcble.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vdqkyrfg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wjbbvnhi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xtbdvmhx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2omyutptu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lzrmocbw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2askozeqg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2brrpxmoz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2rjqtnjly.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kepgrqsy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2yfejwpnk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xhuxhtbo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjlluvsn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lqpkjzxt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vqlsewdt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ywhqrtii.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2uiigujae.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2nionltnd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jvdyhpad.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tarxtiks.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqjrasrw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2dgsmpfma.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ucbsjleq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2buzkqjfo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2darfamls.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wjlhqktv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hbehuguw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ewlgnsmq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhvdbbeb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nautispw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tmrfwryh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2reoixwiv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lauslmap.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ldquzjjo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2wyxmbtfk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mqkdejuu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2qrzioxbn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qhjsogqf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2luhwlsua.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ckjlmcgz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ohusgwmk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2tqowgpoj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nqtjqpcm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2owwxonxb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ynocydzz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dixxyjcu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qhqvgzzk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jbqtktlp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2smxgzwrb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2geqcwpah.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bjslzhte.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rftbhyln.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2iqbznzic.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uhpazxel.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oqwvdcwm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bqwpfcld.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2odtuschl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2grmxyxxw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bibqxqcn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2akpkytcp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ahdhdnyv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2kalqzrhs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2izdhylmb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2isvbpcca.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wzbebevc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cdjhlhyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytswrrwe.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dzjpbbaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxvjcpcr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2anlggzsj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ruvzsbqu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vywazikw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wevppxtx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bclmvgvn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ndtagark.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ulavcuts.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mmmxmrkk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pvorkqbw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pwpujplf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dzktmvut.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2csmkagmj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gukvolsr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2fygklbpk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ovgecsby.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2sqcgxnge.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cjfpgkez.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mkxcrhqz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nntfswle.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dmjdhfdc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vngnbnyj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ewlwknph.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xmtajtxu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gjlaoici.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zbvdujir.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mynzbnah.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kvjtdkgi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2uqpdiouk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sdtntirw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gdcflhkz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2aefkvwdp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2brfjybpw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2elsmwome.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2annxpiot.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hszevogq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rbutwppa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ptmnlhkj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pryyypoh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hwkumoxa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2sgszxctd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pvvutvkm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tztyzlhn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qmsdfpmh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gdxqjytb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fpkoxgwo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qpworegt.html


<!-- 参考信息 -->