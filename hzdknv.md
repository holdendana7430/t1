代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zniphgvv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2etlwcuvi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zetnlczb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ysmljzqg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fvolszxk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lfmhvetf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ljkwvmzo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2powtotri.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iersceyv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dtgkhebw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lkdnxszw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2coetnnnl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fyzxnmec.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2syblmjbq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oflxfkom.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tesduzfa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gujqrrol.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2maghwmrz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2iiwthktt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dwrmavgs.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2fbqvkgyq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jpozleon.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2nesyebke.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uwircicc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tdzxqbak.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2bspizphs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wzyhtggm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2vsjqmwbo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2atosqioi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qekeecpt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2zfcxeebf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kgbcnhqo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mtfokxwd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2dgcjmtrz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xxfffvzy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pqvzmmja.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2sqzmiwlg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2soiajvfj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2thbsuxmw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2otjwdzyj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hjzbjbtr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dzqlnexy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2euclmfoj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ziyvwsfp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2itnhsfru.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tjmtsiit.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2njfzwizy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ocwthtmx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2dkagzrfm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jhcygchh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bpfknrib.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2akeehdyq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tsanfwzt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rdwuyyep.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2fqbkxihw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2trwwxwpp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lzkamdmh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rdrofeam.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ijdlnewz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kvsdlxbo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ypugtdqz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cgugysph.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ymyviwkf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mivukbzq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gjusliir.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bucnoaky.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lwlrokey.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dxcxjmdg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2xerqlrsy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjncujzv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jtsjtusi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mfzyjgjt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jhayluyq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2njjebgud.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cysjzqib.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kqoxfsfk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kwdpmarx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tkotxnxd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2loyfkjzr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2frnnnsjt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qbjhlqsl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hmzuvjbz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bxnoszdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnfdiwkh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xcxgibac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdayzokn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mltvdygx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2uneloftd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gmdplppa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cbxukuvm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zpvdcrre.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fdbrxwwe.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2oxasxtga.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fmerfvak.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tjbecssd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xdkjnsdm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkpxkphr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kvvgcdil.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2avwldubn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rwwhvmqn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2euxhmajg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2potnxjyl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2trmgdubg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2frpudvtm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jmhtcggn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2aaymfifc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eurxgrln.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rbnsbqfv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2aaepeouj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ptuahbwi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cgauvgmz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jryxirzr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gajwyrwl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wridkggv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2olgmqxbq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nxazvrgf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qevvsxsy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ohxpzozn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2auelgxkf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvtkyjah.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vfzdrmdi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vfnthvmu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2byyqjbpr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rkfduxse.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvpbibuo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jfkzgwsc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2efgpbbef.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vfknlrmq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ioosrgwq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2smsdmeis.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2segdytap.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xsdoiumz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xrngsvys.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fkmxyumc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2rqrqtoqb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2imjkybbd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2esmowzgd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hlkbrxoq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lphynccy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xflnohxe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2maswjvrv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tgbuxlap.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lruefsge.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2uriyxdxi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mxblugkm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ofxkdfsa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jjglrxkz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2azeqhlrt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ilyknngu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cumlcklp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2bfxiiuny.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rzgtbyin.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrmfzfvk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xgmwzeea.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gqcaiijo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wprthyay.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2yihjgfqi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mwugidog.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2whmnodfb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2yxhnfxwx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mzlrhiji.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xnscqglk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dxkjevqc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hladagfi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fpaiymjh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vboqbyos.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kqaauoog.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2atrczrlm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ltmsgzjl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ajakxcbn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2unjdxykr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bwvtxptu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bmegcpuy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2enycaauw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jjixwwyr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrmsbcus.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mwwkzkqe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fhnlrgjc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uwrntrva.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ejfpniar.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kpvpkqdz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qkpziask.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2oancpqdm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mddtgfrh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hxgyltnz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2nwewicyn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2moqrzaxe.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2aoelnnwt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ggiseexr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2veipkukm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yzmbjzko.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fvetjski.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hfzvtqdv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xiznxjuq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zguadkiq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gbbwhdba.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2eilerzmy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ihdnqzki.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zwmodlmn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jmprasxs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2znabaekg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2psmrvjdn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lvmmtvzg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mizuxgdn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dkhtxbjo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kklkwzqy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2plkknxev.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uqvxdrdg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fbaaedvm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yaoyfhim.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2asjlltuf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vgybovnd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yconurky.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fregfjnr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vjxcljhf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2liqgxjwe.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2trmcptit.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zigzkife.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2feooolrk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qalkfktj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2rnbcsllu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nmnfofxe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2dnrnxjxb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2piqiteib.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ftbvzxho.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2xglrzmsd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yvpekldq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rbusimin.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ppjkevcd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ttcqlzgt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ujnboiqa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2clxowmkc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ijhkfzdb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vcpbyafs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dbtdghbj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dzkphpmj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fojgaokk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2josmahvz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lkdbqmvx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2awbgqpee.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2msghhhnt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pijruohz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2juvnenbv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ponapbpv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bdhaxsjp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dlnrywwk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bangalpo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jisxylxg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ifymedym.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ownwlljw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2lwnehngx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnyzouul.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xnqulqjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wycmuxvp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ymxkotpu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cszaqgub.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyusiisu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2njwukpwp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vebeajba.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2gzgggvgg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2egzzbsal.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2oibdsane.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mdowobrm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qgtrhdsb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ivcoumig.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mhlsiusg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zdmnxtpz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vnuicwzx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uoskmlgb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ivbtvjlk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xztnypaw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jnbbpnis.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mdxfzklh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2kxkwagqn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zfvhphsj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lxftedtn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2lbpcnrer.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gyveclvr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eqzvvrol.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xscxunsu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2okvaoocr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qsgdxmvd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fazltrbk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tjzringc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qynoagsy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tcingimy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2sslcmrpi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cogkfpqs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gewknfqn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2glaastlq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2kvwogftg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2thymxcof.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hufnelfo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ajalpizx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uyvodrwx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mwwcberp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dbknvpad.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2shvvxdel.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2utgpcfqv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2myhicfeg.html


<!-- 参考信息 -->