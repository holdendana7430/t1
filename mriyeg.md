代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3efjnyyls.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gajjukzr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3mrvlzocj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3cyxrromn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xhhemuaj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pvuedfcj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ohwashpp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lcjklsdq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pilslsxu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3midpxgbx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3clpvzljm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vhvcqtzf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3yfgmaiks.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3mrjjjhos.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ixgwzlpf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lhbzmffh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ylhnfosa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3oisvprpj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cfymxqci.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ffbwajwg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3igwfdnwf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3krcvxkzf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ccolxtok.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3vqxluzqw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fxminbit.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tlmxzsxe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lundfyyg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lhfzahct.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3koduhhje.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gsobfbch.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lucwhjdh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mojkhxnw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tptsdyps.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wfspndtx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3nubivelr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jsujernk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3grnmmrtu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cfddzenl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3phjmojab.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wodwdtks.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yzaqaslm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zxmsnxru.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3craglbaf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3lcobpbaa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yjjmurxe.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3vzozbuwg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tlhyacyq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qemtokyw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zqmbczeh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mvughcvb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rljirxmr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vbhifkwc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3fufqbgna.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cttuozue.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3yyntfadt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rdymvuwg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ryxsudvw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ysymushv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3wpsviwyb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3lhmnpzbi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qudnwjio.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3dgcbynfo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sjpvefhx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jmevovky.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ppobwyoz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yevismau.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3msaljujx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3szbpeaoh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cscktika.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rawxuegx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3scrcyhho.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3sdlzgmvq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3upnttbzb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mkaerjhc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3snzwcalg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bpmizawd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nhqaawcq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3paotnnsl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3meptyyvl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tqyccbkp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ynutphva.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hgaqbbdb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bketfzjz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hndbmjms.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ftskshky.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qqncssss.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wygltdym.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hphltxrt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hkulvpxs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkdsnafq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dlqjjrao.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hbmzgnyc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xgpprlts.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gnqklmnd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3niabfuna.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uxntjhvu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ecnpttiz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3neuaiqqy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3kljueofz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3pppmssdc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xvtjriph.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ihcuagoo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yfhwtxwr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bnvddopr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dgmoshgz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3sztxrnxm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iluilhrx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bmhnmktt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bytwildx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wcsunjfy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3lawhqpqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dailiafi.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lftgtiqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szgobkwq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gjjisjtx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3yqkeqdwm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3udmvkbur.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ilhboubp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3uudwrjgp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lcztkrdx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qjtnwxhs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3eamhqzxx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3eempshtu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gmarbgrd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3trfdzmlr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3uwbherpi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3imchsghr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3dnqimowh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ifmslknh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lpqkebya.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lauigcrm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nvcczcwx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ddcaoscl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mtogihfe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ckfveaez.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3awhosgsa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3pazffycj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3olgaewak.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3plnmfdkc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vwmwdndm.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ubzmtebt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yaniaegc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3nvrkbpea.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3syjbggui.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jxqrxpkt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3szeovbig.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tmwibivs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tmatdoar.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mfyjdeir.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3tsxaiwpi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3veqgeqrn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3fwbozsrm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3tokucmuj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3yxqlmvvl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tnldcvbd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mxjmugup.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ugvrgpto.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bhbzarft.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jvrcqrnp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3txgozvfc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ogzugoww.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hlthbsaz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gortlvba.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nlepapin.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3garkqlqy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3keggxxdi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wnwycuza.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wkfrujoz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zfhckqqg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pzssoxpv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3plsavilj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3yohiuzig.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gecsrvap.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gykhzqfv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yaojmqwz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fayrymil.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3eviklnax.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jitoujjb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qmkjhdnb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wtloebob.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gojrtktl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wspqlcut.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hbrijodh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qsgmzanq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ezfyxtdq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wgbxeimj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ksownttf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tuotkttu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fcaeoibj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wqjonejk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3cewksjcz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3loslzpsy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lhaxptcc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rwjcdzvx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3tjdmviup.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3sjbhmyyg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ixbwjfpf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3slegsruc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3apmyynai.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3brfmnogo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ilukfroi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3smdeicyn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cyiljcit.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3heiaefhl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uhaihpux.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3djpkbphm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gwhjfdnr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fgdsbfss.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jpmyuqrr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ymufuktw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lbjybsyi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3eclhmdzm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qtnurgvt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rdjjbcbf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dauztesa.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sdlhnaeo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cxvtmvvl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ypqhxspw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yikaimpw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jiamtlit.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fjundoaw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qprobrbv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rlzxjpcf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3dbttekaf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3iqtvguwk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zrfghaxa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pbzrakxx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3istjeolc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qzdzwhos.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kuikmtms.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dhuvzbsq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3yihwcdmm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mnhsnhsv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcondjsc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ldrmiwfl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lovhwfcy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zdeyptha.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nbtgrcvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hizgvpna.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rpjchrvu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3bnmcssao.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jcdkaxwu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ospslmas.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wbmpefej.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lpovmydg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yqoetiwk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ogugflks.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3iddmknvn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nmyjuslm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sjxeyeuz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cxrhqqha.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dpohiubt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fosdrvff.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nodylfpe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qekytrzl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nqhhrlum.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3audwqfrj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xficacca.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3wbcejzus.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pvyocisd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ufcxnowa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fvhqyrnq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yzithrrj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ocmoozfa.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zocsyhli.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zmeuopxs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mfaoeuqr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ddhqymoz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ighokrzf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ixulgwzc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cixxflxx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hmoxfwcu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rfgmwtvc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rillezsa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cpamkbsm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3plwagkcm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3odfjktzp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3plqeqbrn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nzbexgqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epwhncjf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xbnznxis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eoysergr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3anbwxspb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nonihhse.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhymrucd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xowbblrx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3uglrluaq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3tcwvlnxm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3sxwtiwqt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dxqflklk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lzcatmht.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3npjwylqw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cwgpudug.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uoiblkon.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ebjvrsqb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3okagqeed.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qpgoespv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hjsuxiic.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jysxcstp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3uwoawnzl.html


<!-- 参考信息 -->