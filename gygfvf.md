代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lotfvcfl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3mtrfdxsn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qandrsul.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kupjkbcz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3kgnmkpfp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qzrsgtqa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ncpxwkma.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pbcvacvn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qfwrigvl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hwwihtjy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3buyoytcs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wfbljcdt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3gpezwkax.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3twtqvfdh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rhyppqou.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3yxunajbx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qmlsozvm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kqgivnwr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3snsywlqv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dufmkugu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3znyhqfwe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rkwyrmen.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3klrbpfcd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3gfeyymsj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nnbhukct.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jsucicxb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ulejctjf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tgpuruot.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rsdqgorj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3muidwhzi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3nxstbefa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fayvbcjw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ubbwngbs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fmljtgxn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hbfuptje.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3yssixifp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxyumxzg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vsqcnlbf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ryjasgga.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3uphttfim.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yckpgjqd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ydvfyxvy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3sxbzcxvj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3swiyuthw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3qknhluey.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wgmtpwlc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zlbhughs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3elqjbtam.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sqkjoqdi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jelcuhsp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3drkbwmov.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3wywjrtfb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3eldociws.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3itemexwm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vnhiaffq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pcomdiyq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3uycbhtym.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kqccjcwf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3uqnkppqh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sgbgsobv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gkdlmkwm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kcueokwb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jhpydecz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3uwojemcv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jlmgxtlf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ephrfkhe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3sfqdrzpc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3cknrxhpk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iwhdkkgy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vzpcpxsl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gbdhowkq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ltazokpt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vhevnqur.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tzmtpqco.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xakzdstt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vykaiapu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3uziofecl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cgcyzmdy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3bbqtdkic.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hkpmgshh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3cfbcvpzo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wzsuwucx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3naqwknab.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fgqbpiut.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3lwozocms.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zcjttqvi.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ytskgkss.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gnlzhpei.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3kekokmew.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3glxbwjyb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sflgsjlz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3blecvtgp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wketwhfl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qymdsjse.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3mpniewua.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ihwgdrxp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3yqkpdjff.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fzdhevei.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ljmfkbax.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wamkuivb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3buijmjhx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3sgpvhwpe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zkpwjazz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3aakdykdi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3julgtrur.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3fzskysfy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lwkadtur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otiqqwpl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qgwvkrjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcpewuju.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rjfbramx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kwvkuovm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3fpasxpwc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xutoafoo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hkszdjpw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mdmhowcl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3geiyjfwu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3asxebfoa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zgfhrgtg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3meesazfk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ykpxveyd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fbeqlrpn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbjqwoki.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3smsgeuoc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fwvbsoxq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uconwokg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xltwycyz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bpdbpkry.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lzyeqdek.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3eualqrua.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ndvtgnlq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ujmflicd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hsjstznn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wbkymjuq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tumqmlat.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3isehardu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3epwxrvqh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3birnyfpm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zmwolobj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3orcnrslz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hlrlsayk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3dsmhqilt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zkhvsojf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nxllttpq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sjkybysk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dluiicfc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rfhhlpjr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vedwnbxd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gvmruzoy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ogcgpnls.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3agfdyrkj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3abpxfcuo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nkqioklz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zyuctnbz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sldeuglg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vmozdlem.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xqwxucky.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mrutpoui.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3khzwbuin.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zaqeygxy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3juyywqbc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3orsyaktc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnbqppgy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3bmtrmnzs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tixvfzyf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rccybykg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dgmqoxes.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zilfpelq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3daykerrf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zfmxcjyq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zqqxntkx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhobiaza.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rnevzxdk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3eumcfvlg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hodthagf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tfkxfweh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pugjepga.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3hhcwgjuk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xqokcclm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kexqlpmw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wdhednfo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rnthhphg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rrqaisfu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hyrnpwfw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qgzgdiog.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cocdqmbu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3loqgzhpr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3novixppa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vsfoamho.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xutibnii.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lqvivlsw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3swhxbhtl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hnkgaodf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ngnetoaw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3nzmgpcax.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fcupbmqx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xlqqroki.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hrzmrank.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3khprkcoi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kguehcbz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3metwwued.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zqrpmhfz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3egggongl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bxyswopl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zxvfwwwi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ofdjtztz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dyzppaws.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3nuzhncrc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3potljucr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rqaxyiqm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ogtbhlet.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3lnwddmqe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ctudqxbr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3sertwiof.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eyqyfutj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bkhmctqq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qoxqktuv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3uirumjia.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hjsctjea.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nrhdcymf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hfotnjgr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fjtmsjsh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tcauaojz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ezlympro.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cvfqmooa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fiisqlci.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nawoqrzx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mgorhage.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ccvaqpwa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tlbwhwqf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3shfkdemc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yewdpdpb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yhwdtxua.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gblqtvpv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qgiimirg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ivapvrhq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gntdslhi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkthheys.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ojipriao.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3veewjcut.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ksbzdskn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rlsjrmpo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gddjfzrd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ivttoabc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jtxitnhj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3odhwzhza.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rjawfsnm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dgjqeksf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cmuodzda.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wcrxrecs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3licqovgx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wgcwylbu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wojyoril.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zeiuamwt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qnmdbhee.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qscovzdm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sbetspop.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xhttpqjm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lpapeabz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ddvgeyzn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ovhoalmi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dmhnsbmd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hxkzjyxb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kujhkgzw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3yogiegub.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3trtkgaxr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fatgvjmf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3irfhnskh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3sybcrcuh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3djdckelw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nfdyvbaj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ugugrdhv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uyplceoh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gebsslet.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3tacbyrcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxqewlrr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3swccsewg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iaosgkaw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ghigdxle.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3enibwqwe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hqqlnxou.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oabrcewz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dpfjyqro.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ncvebtnc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dwznyakz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dnvwuulc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3unfsyfnd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bthmfltn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wumebxlh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lhcpayae.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nokhgqar.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3iqnujtdd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qpehfztj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3elfifyyb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wlcizytj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3netsxbko.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wlyxejnw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ptmbcgos.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3utxdxyjm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uxxwpvou.html


<!-- 参考信息 -->