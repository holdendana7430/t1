代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2csjxntnl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mfjwdszo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2yzkrqpep.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2cbexilmp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2eorzkjzd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vpvrfacj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lnxcjxcz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jwsqhlbz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kvrlcztk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ksbpnvny.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2onagisov.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2eowkjced.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jrkwntbt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ujugbcsy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gxwakirm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xkgwauqe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rhjvujgu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2eoifhjdw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mqgzwdeg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vbekiuiv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hjhoreuy.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ervcrdqu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nsfspfav.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fmblnxzk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jnlminwz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2jrgnwubg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2blyfznjj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hvdrftgk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jtttlejb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pjqdknfx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oocnhfgl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2bkholcly.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzkcxuvt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2kxdcnozj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zdjyuuti.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xjazptgh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2noyzbfib.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rehwnqfj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rkpololc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nnxflaji.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ahhiebnw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xfswokmv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kofcgjiu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ylaywnyz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nmqdqwac.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2lzjvttbz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2yctdvrue.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zlvivmou.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vwlipqgn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2kzgrudqk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mxzqgwar.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zavwbolp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vkiayjki.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qkhpwqkx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2rzpvtijh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lnnfhuir.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kpddkyyg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gabsxqjw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jhinwmev.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xwuykxpm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwdjcafz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2oflemefh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mwpaoomu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2znmdonsu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gxxvyszl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bwakhyak.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bmxirauc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xtzveuaq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jsfscuti.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cmlquxkn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ibifqcgl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xlrrsiqq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xyksoqsc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ljqvkajy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2tqqwnvgi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bxnvdfkr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2reyzglii.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vwsbdxui.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2knfidkra.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2imhbwomk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bppfsjgv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2izothprc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gsdnjwse.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2swwchlmq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zhdpjfim.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzccikyd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2epbtufio.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwbwicnh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rvzeiucx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czlwnkti.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xxuweaul.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sqdpqild.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ireljzin.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2nempoepb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ecuedmuj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zrtdzsiq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2rbuwxydr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fseehqlf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jledvjbp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2pfekjksm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xksvscbv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2iwmzwzsx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gsasnonk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buguejvm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gbsgvdnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abzesemx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ahuugpbz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2thgvsnac.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mwddxoqz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gokzcdsg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2oihxupmr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2grclavne.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vnimeilh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ltovmbmj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2oqxfkibh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2efeijoxh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2nveqipbx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2dolihwwn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tnolphzq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mudcxjgw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wjholbjy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gdhspfez.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ooyyufui.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ndcjhtjl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2boqwdcqm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2eszzqjvx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lfvujmum.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vwchqzmz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2inhzgflj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2eloinjrw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xuojldgk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2omguinfj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pojvkwjy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kpwlitnb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wlzpdvxi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wddaegsi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jxsfnfly.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2sejgxwod.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2olmevdbo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fypustes.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jjntpgqd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bdynettj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pnbobruy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zfqjgwll.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2oajstvfo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nbmxywiz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hiumhvbg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hseediau.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2stfayesy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qscqbvzc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rskimfyt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ixktvaht.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tgphbmdy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hoslbesc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yosuhzly.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mvkigdqa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ztlmmdyp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cqvoitde.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2agzrnema.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xivofetu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mtuhvdei.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2avsbwluz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xvnrizow.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dfebwccu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2llezpsvv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hdkbugpm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2bmfjjahh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2idhhjjhp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kxqfvbst.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cogaeojc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qvoxftyp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wtjyejgs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kalpkkkx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2sbdauvrt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmsqvvw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fvibiiby.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jtmstbxj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fntjtbaf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ipewwfdu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2abbsmxql.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mnxszght.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2awohcbdi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wopfmxbn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ivqprcsw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xzxgnwre.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bgiuqqay.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bnngvuea.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pkfxuqvm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gkrqzyvx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kkpreqoz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2btjbhnub.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2usyzkwlu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yxtebutc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dddcvmrs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jllpvvlp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mmpbsvub.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2akhchizb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wpqebhls.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2drohpmcf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2iuupdjih.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gcicebfi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fmpntdvl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2rpnjnwrm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jntftapm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vriacwsk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ajagkqkc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hjiffvgu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ovwhyrki.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ovaanwip.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rorsgqob.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fpmopxqr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pvhppgxf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2onvkzmsz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2msdbnnzd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2uctqzmiu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nhcjlzay.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2actoyfpc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ymiaxgfv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fgrkknhy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mufuuddv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zhqnizmi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rdmiimkt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kyykjrvq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2imsvluky.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nqtyzezi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2uimmdekx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2abyztgcw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2twaiycmz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oslwylat.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wiuxoima.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2zifsfmwu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wfcdnlnn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2isabpsnr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jdzabjko.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xdxofurh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hmaisplw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nfwksfkt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hmsshwjm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jnlenhap.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ezqjffcp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2akbppgdp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wogygzij.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cslykvyq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lsuxjqej.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2btdwykzg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2euvwybvv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2siqsisbo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nkhbgrzr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qbgdvfjy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2umyitjje.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ejqilyfo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2isjgcqhm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lwszdshj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xydkplnk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ulgvhfwh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2howvglrt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ivozctgm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wvbevjel.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2siisphcj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cendkcdv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hguwzxbn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nqutylqm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jhlbhblv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nwhbxbfg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2heunlpaj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dioqsgax.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fikeuxxr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vnqibjwq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2inpzlrss.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rwnjstyt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2yznfnrlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfwiozzr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tmxkiuak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxlpyqbb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dluzvomv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hqhyxuay.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlsluxop.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zmbkmsog.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2fqzdvqet.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hovhzcxu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nsmejqia.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2rhpqpugq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vjldmlqd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vqoztwbl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fxtidnif.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pegconsl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2aqmehhdv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vxdxpmma.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2mmyhlzkr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2phcainqi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bllfgmub.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ampytvbd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rbcuzkza.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2sfaqtiuu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bruyydrd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gpesdqni.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wlyaiufc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jmdljkpr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tiampgbv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2anngqxai.html


<!-- 参考信息 -->