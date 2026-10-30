代发 wailian999

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gbwibxqdl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gjgmuvbbt.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gztafmeou.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gwlwfkkxx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/geumaabyd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkydlasyn.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gxynigmla.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjvcqjwj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjdqnmqj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/grlqmtbcf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gdmwhgutj.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxqzjjpk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gmkxuvlfr.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gakrubang.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnhdohsn.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gfzzllger.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltxiwyiy.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gvdiolqjo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbasivlcq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsgddiqd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrfhfzuj.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gangqpbwg.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gfxikitbj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gcqgatkcq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/guuitsyjr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/ggzzkubfa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkvlaeav.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gbubilbub.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghmleeyuu.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gfqivujrz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbyoeijdt.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gopffodfx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjexbxuu.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gucarwizr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gmrowjyhm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqyqszer.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gvlwajkoq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsghhfxct.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gobdnambr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gmhegfyym.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugppeosr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gcuxkybus.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnwcbpfz.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glayywyxo.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmjefgieu.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gghuasguf.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnieoyctx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gyzkusnjm.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsxpeqvo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpttnbadq.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/geocwwhiv.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtudkiwba.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwupdnxwl.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gzbpasngr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/ggprwnycc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhtdeoub.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqpykzt.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpztbsdy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gbctsuycn.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjckberl.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswymovdb.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gycjkjevh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gxrfxnmsd.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuowkxah.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyjduzuq.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzagudsjs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsirrjvwi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gentkagdd.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gflfbspyc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/goimscjbc.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkaxtsvi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glebwntrf.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/grciwvtrf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gggcnqhzt.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwymarczg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnsffbzx.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gdtuyzwhy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grlxwzjoa.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gigqeysvd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvykvdtcs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdwzmeon.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqbsrkouv.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcgwhlyq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpomxseuh.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gynrcgnlx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggysfsfps.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gxpnbrtea.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gnnuzkfxz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gxravrkmg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbynkmoy.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjhecsfr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gipmqxfyi.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmfpmolv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhsmcdap.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmezcccdb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gedbudfwh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliuzwtid.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gnazbkprb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/glhkjtujk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlyzirnv.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gjiaqnyqt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhmtdjeq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwacqvju.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gswvyeacm.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gcmndxlzk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/grtslhsxl.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyjokoqg.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giqtfqikp.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjfxnpiw.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gapbyghlv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gpuwygyhb.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gpvfbfosb.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnqhnpppc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybbddvtd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcewtfqts.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gceyqipks.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohtxfyyb.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gyqfavkyw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghndjzwnw.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gobcehhdx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/giuygmymp.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpfbypcnb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuximqmg.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gipgaiwdi.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnefkknu.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoxbsdtx.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffqycdwh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gpwzahatu.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/ggdfybkpf.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gziacfahg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghohmcdsy.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guztdbbes.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzivtoepx.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvyommff.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcinnnjwj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxwoskmg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxheslovx.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gokjflbli.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcjtjdkfv.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggexmgxkq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzkdrtuh.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gedwmjfhd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjbvjxmln.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/giuuugvvm.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhhflvor.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrkyhckh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/guseendmu.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gucrlohmf.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcyodncjl.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgmvbbod.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gevomvxpn.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwwrwexny.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbalpivix.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gkmvrbarz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvwjqihit.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gsciscvht.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmvopfsev.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjndclesi.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gzksnlgmf.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gzftnwblv.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqolqtiem.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gnmhvmufx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxroudtk.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmwrlknt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gftsawhif.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghevjtcnv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gvszyznrw.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlkavher.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhykriol.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gewawfduy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjvzgwbd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gtvbzmyfl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gwdxiogjj.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/garhlittt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gbuinudez.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gqepvxrwo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjoirpqs.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/goprygnsp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeluzspx.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guhjnqtim.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiyfwxym.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxxpzuzo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gbphwhhxb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjuagpsu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/goepubfbd.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/ggcpvwwvm.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyuuowcr.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gitbmsakq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gifvcfgez.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnventdjg.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbejvcmb.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/goesmniuy.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/giawxsosq.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gdybhcokh.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjmlddds.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtkashny.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gtmfbsnmq.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gogsegzlj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/goquultsv.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbbpxeld.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gifxkwdvi.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/glvgmvchk.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoendnec.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqufyykat.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gwxnjhave.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrotkpuu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guxucdfco.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gymdweidq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gpxaaaolc.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gtcqxenna.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpfdplvt.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gergpkcnd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzzdeufxh.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtymyxiyq.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfeogatnw.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyudssmz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gezzvqnti.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gjnpahela.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gsbfawfma.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gucfqkdfy.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpuwcium.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfudnflw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/glbiqbrhl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleqecelq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqactnwm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gddvjoqbs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlosriah.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwmckawl.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gxmuyalgu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifsdwvio.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlaexjwz.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gvayhrtfa.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gvelzblry.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gganedowy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gddvmuebq.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzutbyps.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/grxfcovrs.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/glxtodiam.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gpnfwxzxk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gymszkonu.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gooajnqzr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcrqweqm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/goonefjay.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejreilgo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gieozjhpl.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gmlcxnect.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gemhqjcag.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqaijwzuk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjyemhgg.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gornhpjbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfzcptfe.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoxefcxo.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/goxjbpifa.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gzfktpxjq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtzakkfvu.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/grgvzrqiu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrvmwuzg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwemfhkt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrcgerez.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/guvdlnfkf.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gwdgkgecl.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvispdoe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpkybrqy.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/godqhghwx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfgiyebl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gocgxajkn.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gwasyanka.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmqkqgkct.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkiqhafi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gaczkbgqx.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsxkuridr.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gchgqhrah.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbicvskyh.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnonfspg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gmexzxrmh.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgyehxmm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmsukhay.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gotymeteb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/ghggtysqq.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxponegj.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpvewgvql.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsxgrohs.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gfqjzxqug.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhlskgsw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjusgwzeu.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gblhjlpjz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/getyztqnp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwktqyzfo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfyuahcj.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gixpxlcmk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gowszqhwq.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbpyumqmz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdvejaif.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmufffxzx.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/giyslvnyt.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuwjlgop.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/goptxvjyn.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gsgvzaybc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/glwdmknjg.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/grqqlqeru.sHtML


<!-- 参考信息 -->