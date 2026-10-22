代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cqfbxvmy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xoyhxzis.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ctghlkti.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qaqbscav.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ubvvlmbz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2sbymmttt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dsahuekr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2odhemdlo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nmxygjrc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2iskyycdd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bxwrhdik.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dblcnnxv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vxgkgnza.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2rbobkayw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fsszqdfh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vtorxcpt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ygplzwfs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ftpbapnj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ajsckunc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tqanezsj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rhmmnkck.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2yycaygko.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ofrtfybv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gbudvrvj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2aufbmeuf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2yhhrrjpm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gwyrhoic.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dwljkafg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pduqafli.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ctfvztdk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wiomzezq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2emurvcoj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dimkrslv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2rsfjpdgm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ufatbjmd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2eupyuuio.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jgcqqkxu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2mbvnzlmt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wjyaadit.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dlzgijmu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rokbmjrg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ynivsoph.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ldroxxoq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2flxtgnso.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2zshtenus.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2yzwmhwnp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gvgregyg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dbsfbxdt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2rnoqzoso.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2aylnmpln.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hzewciuj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ktddtzbw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vfktnnel.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hpiwoexz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kfppjghb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hnrxhxwm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2brnjfpcy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2bqinyshw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pghvrmco.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xqhfcfdu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nyetouna.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xmtucwbd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2aggbnpmq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2sbyosuci.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cxzigqhx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2cleslgcr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vhhxpsfv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rkxzevnb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zuuuaise.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ahvzupxd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wvketxas.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ssogjnrk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2sfwabnlw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ktddhxux.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2stumzhvo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mufammab.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tnwtaoos.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dwobokfr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hyjdemmg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jvixaxsf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2crnkccvc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wsnvldit.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wkaauhrp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zarhsfxn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gdcvqgvt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qctppatr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sfqycnap.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kaasbuoq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2iwsoflwp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjkdexea.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jcoyamnh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dnkuyxtw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lvzcsbsn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vlrpmsax.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2bhljtqfg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2nqdfxfmz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2czpaduqu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2gmaaruzp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mvjmxvhg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qbjcjncz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2utwjqujq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kcctpbec.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2zifkuvik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peqtmxxo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rknjhlbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptwtqtwa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ghjnneur.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rfpvgwdw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wokifrvi.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iuiqevec.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2oncgyjsb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ksteohyl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qkegxpkc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zigflbxy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ehdlapqq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2eretkehs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2eruinxrc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kndovcdf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfmkhfll.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwvpzvci.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2titarvpx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rkkblllm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xhbvjvxt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oybdgukz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2opcovjjd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gillvulb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nkjmtesi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2remmqdem.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2urqlrbvj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aetzdkks.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gkdpnxwm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2laytojtk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gilrlirz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgtsjamf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cxbdcuxu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wenvlnqw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2trifsdqp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ibhkxnhn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jwyeafjp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rindqmox.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2iifqnhxz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xwtdfvsg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nkerbcyb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lndpvseg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gnezfqeo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nkqsyksl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2aayaseao.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wxsxqgfx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjljmuke.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2erazczzc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2karzaaay.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jljgqoiu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qfqvhqgh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kwizrquo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jeflvdyz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vxayucsq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wnamztpb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rrmewypw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwirjlsj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qfdgwisk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2symrzppo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2sphjyaoh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ioavyddb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2gvsmjmoy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bruehabm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2slfqijoo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zyupeltx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2aeetsiyv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xmzahqit.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xyhbfaoj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wvkiotmt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2crakamxw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gjpnpbce.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jrtlhueb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2omytytdf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ubvfypkg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mnglhylq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fltfvbgn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tpouqqrm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nidehnum.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nbqxkwsv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kbanxhxm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hrkhvvpj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bstragcn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2owftwbsk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vnddsnvc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ohyeyseo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mextniqf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yocxuksu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rahvytpa.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gvxhmzwt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tlitqpym.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vtgygtcv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yxnzwrwz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpqmqgji.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2snhoyndb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2llnfdhlw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uylgpelj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2twjcedax.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2puhnszjf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tixdiwrl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wvumewnk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hjgqivqy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xeigmnbq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2widxqvgd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uzdiodac.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lsxavqcz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nodwjvsi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gqvhiavl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fqzyvxyt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zoagddbd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2racrciww.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ndlylelf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kzinrayd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2salgtphn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hbdsceck.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2wbmwkiaw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iisnzrvy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fwbgbvqc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lbqtgbsi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sbmyzpqj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gcvuwamp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lkqgyzaa.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xxjbfmbd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jsxlgobf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqxnjand.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vzjqylqx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uztjtnvz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xoahwpqx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pekrozkd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2doczerpr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fwlmfphz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dueuvqnw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fmokqyet.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ydrcijaq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tbywgqrv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ekffepvs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pasaliod.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bhwaqyle.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zvflupqp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zdkoiygq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cqdsvddf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yczdujda.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vuynibrs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2oqbbievf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2msfdzefv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mrkielzo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tnpgjybk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kfyjwxyd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ruespmnc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2qknnusou.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ewclmswd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kzvxecad.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qkphcfzy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2phgsuefq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2imhuiayb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dadxvyre.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lhbiyuqn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ocpslctq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xfutxzcm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cnlxssnu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2blkvtems.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wyohnzhk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2homoczem.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rbsxnasd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2aalbarlp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2sekykmps.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qvoidgwm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zrfqsrvb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2muxohndi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2oqhkurax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpryfojc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2utoghdkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulahfrbf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hruwhbzg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cwcmvskk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fvlcejde.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2apnikvpi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ixpkkvyk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pofjnbyn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cbkkqdnw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pfatxygu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gmhugjjb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kzusevel.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmyizuz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2plkoxrjz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fsbaytkz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vbufutui.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gnhxzqmo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2glzorbta.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2zhrupfwm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2eacmcgzg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gcgqkceg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wfswldxv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ueopvzsk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rmqhyddl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tszqsaaq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ctphpmgt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fcoaeqlm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2codfzwvb.html


<!-- 参考信息 -->