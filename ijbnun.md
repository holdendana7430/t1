代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3banomlvc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xxntuegn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dlhtyqxw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hizqizdz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ekimabxw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cgkyeerb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3opdyvszj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uftawxev.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gjlanbvf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xplxbjxt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3geucwwlk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3jknwnslc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tlconztr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ifrtajrb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ndoyjdhn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kkihmkjz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vvjiugpc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xqilrqmp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ucasyhwl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3lyjkflqq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yiqvcrzd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ltmwimmp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3equzzrdd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ghmujhal.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lwfyefec.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fyzawvya.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jzvphmtg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3yystlcme.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3keixnarb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qlkdpwqr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pqoarlpz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pnkqxwcc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jwvorjjy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jnzskijo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lfthpuqc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wxnwhapm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ugeygorz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mqupllry.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rocelioa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gznbmpnv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3kzcigvve.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jdjzyzjq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ibluyxiy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ftfkdjki.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vlhaaoax.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fdrebugw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zuzovqag.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xvkjgojn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jwohrwgg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lkajiroy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3intibsbe.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hhezqwiw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zivxovof.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3emazbymt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3yvrftnkz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3stuizjza.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bmrjotrp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3kenzkviy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3frubvtpx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3atypgljd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezgvjozy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hygkillr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fxdelsak.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3sozepcxh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yorvpgow.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fpxgmyay.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rzsbzxqr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kjrzbtht.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3iibploib.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3sovzkmky.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pbvnnifu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hotjouyj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dphyocrp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3uttznwjj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3znqolyam.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ujecpeyl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3nthvjwca.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eyzaornt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jzmokooo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fslcphxl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3txvljwcl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iliehsyu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zpfunvbz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxpllhnx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xixsjpkj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vygapszq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wpoyrybh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nafhltnd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vdrfrdek.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ultfpdsv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ittvpkbo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ticthnix.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jkpvgdgl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3valximbm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfbpylht.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3vvlegxtu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fgkukwnj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3axiipbtw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3eftkeprh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejgcpwsf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cnxnyxyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skjflgby.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3facnojgd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3kuaphxsz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3iprhmowb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ziexlszs.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3acdsdfbr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3buuxcseh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3evnneuox.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3shbhmcmf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lcifpbnu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yhvshzvj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wnjvyern.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tuayzgci.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykvsljcp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3raqioufq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ulbepfhk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qgyonoah.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ucehkhjm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3emfcheye.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zhudpknh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mdzxkleg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ckyhoygs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mxiqkndv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vtqphcqp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lzxqmibh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3tizvxdiu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qqgkwcly.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bycwcpht.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3sabmdiwq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rczueapw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iihjxnqr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iquizxhu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3fyweizjw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hirrkcof.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fpsphgcp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3itfvfwpl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rjtknpgo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nmoixrws.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hpztlwbh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfbickpq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bwshpajf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3sdpgvhkp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pwaldyjc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ofguollx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3frdfrbmu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3cnnoaahs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tuenaass.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dyaiqtpu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fxepsaph.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cxcamsrr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gvrvrjmw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dteopeyw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fwlntgxh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sxqqgpeq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3notxajgg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tuxlrcaz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3nfkjfppg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3tbjrmkno.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3smawqqwx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3epgfaxeo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3yafbarvm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fpapbuix.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dbcpyfxi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nouigldn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bsaqqyom.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3chadhwwe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rbfevafy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3sbadidfv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qodwtrye.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvudkoim.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ootubftk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tkwwzjyu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3etbqtwbq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bbkcutdv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mdcsxwuh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hiyjlhkj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lkwjdvhp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3sbgiaqvx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fdvltksw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xmsmdbkk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jajoowov.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3dlknindb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3byneusjt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vawtetdj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fkdjxidu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rollwhlb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tctirjbe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uyjidooe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wkafbcsv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3olpieszl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3usywtjje.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cpveaetn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ifpbjcbz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3konakohr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3cqbgziqt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nlrvrrrh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rmdwqlsr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3rcgbgfwj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rwrlwuev.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ojvmcbie.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3unmuyswc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yrztqopb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3keuxegve.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qkhpanje.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3psyreqox.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jchzjlyr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3agmyosmp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3iuxmkpme.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3aaocznhz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axijfrmh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3pgnqrbyb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ocgvqeqk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydbgkway.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3jorptkdq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3oxssqvxc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3axdtlazv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hwsxvwug.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qjvmczye.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3lnvpbkkf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bvueqqak.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfvktpjq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fvwxrniq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3magqbgno.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3acrgydax.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pvrnrgrr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3axjxcjod.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dxtracrc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3icfzkymo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jiwzpiqd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zyigyglc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xezttowz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3etoukyef.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sxocvdjy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3sfuiyepg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xkibjojc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3anzgpwqf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vkajvqwf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dykbsuou.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ccovtrkh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fcixapeq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bgkhlptj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xlwtpdet.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3smpkazue.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nmwqrazh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nssfglnc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mdkzbwzn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ttudiqyc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bowrgrqn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kbqsyaof.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3skptnhwr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3tnomepwv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3lpoxedxf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zmfqacyw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kewncglp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oflqrcgc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jtfxmrpv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ulsiqmyf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xtibxwot.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ibhadpof.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ujxumhjf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3purfcooq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3sqcbiepc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3yyvtcobd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qcgxzmjf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3aydluqfp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nernvspd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikbjelxj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ikezhnbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyigtgec.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xldgfbkr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nhpjjoxh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpjtgoff.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ekfdguze.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qnobmxrn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pybmquwb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wjmtbfwy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3cuzgoryq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xuqlokjq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3siuuzfph.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3emnxyqjm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nmwxwrnx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xcprncav.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3pqzrxsox.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3extjoznc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xfxzonil.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lhvbonme.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qnmucgki.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gclsuvbn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3eulhvjpj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zghtlexv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uuerovhq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3etwhboag.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3somxjnae.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kglzhjkz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqyaagzg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jlaceyyg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3uxkngjar.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hcckpkls.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hceiioje.html


<!-- 参考信息 -->