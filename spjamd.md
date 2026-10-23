代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3esnnkdlu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kzckiyrt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3dfrnldvd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ysdxbisy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3brlxcray.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3bjarlngc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tduirudd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3smbauzhy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zuzsbeiy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bpiyuyaa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gftzueze.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ccrveekq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3demeolhf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3zbmbymjl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qsqaglob.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3djnprgfv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gjhenryh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3pimvewdv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3qcampiaa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pwkymsod.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fiaqxugt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xnvcqwun.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vpbtftzn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tbwhqbio.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wjypdyat.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3lorpuwgy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fxaxueqo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tzhxlvef.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xgpuvzfs.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3elvtkidf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wzbyaxrd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iddqxiho.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kjuqosxy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tiphoeej.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3rkzbcvvt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ltvdslha.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jkoevlmm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3swjclkip.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3blalwxve.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ozsdrmpd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ymbmevik.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3mhgwagkh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rtzljuev.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pqljkccr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3oyyjuimi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3pldqjhkj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3uwrgxcrn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sijaujbv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ikrrnahj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3valurvax.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jeuoscxm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3scesydpt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3wdkefdae.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3oxdzstvr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gmjyielk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3fnrkjpbz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cpncwwab.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3baujfbap.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fubdnygx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ytlhdbcs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3uskqiurr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3afvrwxgl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fvoojbop.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3glbfcaro.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3eubknumg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fzxstcqk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3supnaxun.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ywpqxgfk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lckavoii.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kpfzbbhk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3heivdpjz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ygjvublr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3agcbycib.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3givjejms.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dsepavme.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iagfbkhm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3rhzclqbr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tgwxkfao.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tvpbvedk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rlaszxmb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tfyhgbil.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pemaiaen.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3evybjkcm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3qkjbapwr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3tukimqgs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3evlbquau.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yetcujlf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3urufjibd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3monbjobb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3oxdogicz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wfinhmlj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3emlpgjrh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3plaaymjy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3fbwvkhho.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3tyraalrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhxlvxpy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vtabasma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdttczdz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3abhkrdvu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gphvrrgs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tkewytfp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kupuelxz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3younjkzt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nvpaepmy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3sdunymmb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wcuetmpu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3utxdkzna.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kgvynwpt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ydqtwgcf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3snvxhoaz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zekvlieo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3utgrgibs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zmizmxxh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oeuoetyg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3withhrfp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cxezbpza.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3viucjqth.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zvsspxtd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3djerstqc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mvfjkcjt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3rpttjyuj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ntzyssfh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jcadlaxx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fdlipxby.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3cvomemxo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3akaaaeiv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jlgwwwgk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwqljbla.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xpyomthk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3yvdeubmx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pysxvyks.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wetahdcg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pbxhzumr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kfdytole.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bdvrrhnh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gedsygaa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3kprbgrig.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xxivjcmm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dbmqwuos.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vgiiytge.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pygrapja.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3yoejfofd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nozeviti.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uhpbahmk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vbugmwbd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ozpyhciv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ilrwkaut.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xxxwrfvc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tprpouoz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hfslrpts.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ddyikccp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rkromvoi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwqfshgf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3eavybufz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3drypoghs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3sitwsoui.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3aedsjewf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nxadlevl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ibyhruws.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gylhcbiu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3yekrdhan.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3smmbthgz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mzcsxjtk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hvnbpjsk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hbrjpwhh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cemnhhby.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pgduvlbp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pvbtcdfg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fqexfrth.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rmxezuwg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kuhmonbx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3utkgdryf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vzzmyznb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3eqfooykd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zlxqpvlk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yijxycms.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnajrzv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3omwjdeep.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3heqcrtkj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fwdscpja.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bptrqqbt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wsnwguhk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gjugihnf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3csqwsrae.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jcfvtvjm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3tjdemwag.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yzjncihl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3oxvuipek.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rsjxgumn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3grojzzvh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wryffanu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3cbfuhfeu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rkihgtpl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3koxnkcat.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3pqpauyeo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mspvhdhw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gmrlejsy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fpnbwetv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ewuudlhj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xrfgaemi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3plcydyoh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3iyacwqws.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fenhzogt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ogrmduji.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fppeucts.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3syurlbfp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ezgqnklk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ikpwvzfj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xdpzfzre.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mlpfzarx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qyelaoas.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jihugjoq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cjuhkzns.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cqmtqxmx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3unbyyydh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nwbhbpbk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jlhuxbwp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wdyrimpt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ehoxwdrv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zgobpdyo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wznarknk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wltdisqk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3slwodimn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rocnnete.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fucidqma.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bokaemfb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rievehps.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3aeouldja.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qrmrslyl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qgjhvhgw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tfuyzceu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3gzlbccoe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lplcvhgg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cezyndqd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wosklsel.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jlgpdnoi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rijamvcn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qyhhlnml.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sqjsexui.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jtfazktn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jphlgqox.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fxxcnmrv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3yqrkzcvc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrimqaqk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3puoajocx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ncprybkr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3utlzfidm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qsclzyfe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3eycwltgb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zhzuqqau.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3blpakzeq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pziwfdns.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zcggzzmb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xfvecpae.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cytxwajl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ounwfaqb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fxkujkmw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xepfpcxw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xasqjuno.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ntfkipbf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ivlwqhhq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fshuoydy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uigzeqaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pruclihv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ydssiqrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgoumvfl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mpygaikb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3odomsuhi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tysfogua.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vwpysual.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tilhbgdq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zgjzhkvi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ocfhwrwe.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3iiwvbtdh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ceijbwzi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fekxpuxi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttxcndgg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zdiqffea.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zpbnzpvz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3fnmmmygm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dxufdqae.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3adqqpwyi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3tmdsadye.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gyqqhafp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3idbkmnes.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3oyhuhyem.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hsrcniem.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hmsjbtym.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qpdxmsax.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3estvmssg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xdwolqfv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3heatccvg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qhcbjmls.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hcolimrk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3txweacmi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wiqwwpke.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3iwtjoynr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jhvofmdn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pxbxdfjr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cugcwatg.html


<!-- 参考信息 -->