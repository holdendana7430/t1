代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/grjpgvwnp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gtxvzymju.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/giemycplq.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gbnjkstuz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gxexzhgmw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gnyjsxonp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gmkrpufgd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gbturjgpm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/ggfgcpqoc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/ggbwyanun.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gpleinxsl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gkjaonypo.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gccgsinzs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/ggruhnily.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gloscvwfd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gpsuwwesr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gczorhxoa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/glbvmznlf.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/grxztvsww.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gmdqsxkxz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gfsnumqcz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/ggviquubh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gorygphyj.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gcolyczbo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/giiavdrxa.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gpusyohdn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/govmhpvnb.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/ggxxtdaqj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gsnafevzg.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gdgtwsdbj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gnrqmvtjq.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gibncbyop.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gukhtsczf.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/ggmzmnnkm.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/glylrppoi.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gjjddxeqc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gkhhjdpfx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gpykkzhce.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gqnayhozs.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gqvtjftmo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/glhydtphr.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gjtyhkmrl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gcviegffh.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gffdwwfst.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ggmrrcxho.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gdowsnhjj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gkptmbpyc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gancztjig.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/ghoybwsum.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdrtgbgrg.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/ghoeuupka.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gzqynwezb.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/ghevwtnqz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gkmjotanz.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gpgxaultm.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gzbtndyco.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/grmbsxhqi.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/getfgzklh.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gbxxnkhzr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gccohlgng.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gnfypxkzt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gfwnjrxvb.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gscjfjihs.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gndfbvqnm.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gcfgesdmp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gdbixwogw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gqtasljwt.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/grjbkjtbo.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/grgmkdoar.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gurboffds.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gupekbxpg.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gviwehocp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjmqoeweb.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gshmsvnzi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gecymkrep.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gkyjjtrhe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/ghvezpclo.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gpwgpzgmb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gaewraciz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gjlomdhqo.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/glcilzgpe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gseuqkigl.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gskwryhrp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/goebycmqp.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gommtlqnk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gdicgcxqw.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gebddikyk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gfoqacluy.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gjkjnwrcv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gipoqzojt.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gklvoxscw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwpnmtame.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gmfdsmzkl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/glknujznr.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/geqidapmr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gevroiysm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gpoknykid.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbrfipudh.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gebrixsak.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gfvrswqkq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/ggaghffog.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/grlgxwrxw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gbjvkvtmc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gwkgxybpk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gdsmvldnr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/guvuymrat.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnphnoimu.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/ghufwajoa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gxsuxnjge.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gytphoauo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gxyarqedw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gidudfyuu.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gdjszjhvg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghupausok.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gynewbvdj.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gacrbpqjk.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gctjdqyok.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gxzlviaeh.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gtqrgyhdw.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gknarwzru.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/ghlcceywp.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gkvrlgolv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gdtteurjp.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/grpluisha.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/ggfkbtcfn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gaywsayoi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gewilcfur.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/glqxccnmb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gaeyidxcg.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/glqolxapg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gyckymfwb.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gpgissjas.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmwvihcxc.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/grbushrct.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ghersbiai.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gqtytqqzi.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gurbpewzn.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gkfdxbldd.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gadahlbfe.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gyxqwkslv.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gxdauikhu.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gdjinyewc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghcggtxog.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gyqywwqip.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gfhlyzxno.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gfoqtahng.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gmrbfdeon.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzbkmmrur.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggybpjeso.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gzcokthli.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ghemhvxko.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gshxwnslv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gbqmojwwl.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gqpriuleu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/ghxtbgeoy.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/geaspdcmd.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/grtgnkiek.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gxjtmklwy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gbroibbwm.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gxtoruwou.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gfhgimunc.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/goeqwfjxj.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/ggyhygeac.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gkpgqwhlx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gckqipyye.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gqhiujzdu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/ggmgfzrrj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gbqivqcke.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gdlupgatt.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gzbbwrhxy.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gkiggrqwj.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/geojgjzhi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gkjumicgg.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/ggfslcfma.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gmowmzzuz.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gsqmexmuw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gbklaxzgy.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/giiiatoqk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gvtvsxkjh.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gajhphfnf.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gmwvdiyyi.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/giaimmwyf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gqciecppn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gcjtsvumx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gwyvlldyh.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gslryfmxc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gvmqihdgc.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gqrlznkcg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gdihsszvw.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gwaeawxur.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gfuizyaen.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gbswoiihf.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/geoelffsn.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/glaercoon.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/guzatiuvt.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gctechejs.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gssbqbgjq.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gxsyallvp.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/grwlschqh.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gtzjetvdh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gjxulnhhm.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gfonoqjml.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gnblibnog.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gsesibvgv.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gqfvcaxum.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gnpnacego.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gxookyhdw.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gwwdxlcxp.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/glzufieyn.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gahaffvvc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gjhnpvcvj.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/ghlzppxkq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gutmgklmk.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gmgclnchm.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gwolqjvro.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gkyqhqtfr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gbdhhrxvn.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gjhqwrcqx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/glhobuqlx.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gywhszmov.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gvuarzaka.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gmxoeuyug.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gxxgfkzzd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/ggjaaxfpj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/glksovwna.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gbvmbsvqw.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gbypbqgpo.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gekzkshwu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gsmyxrezm.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gjlchuhfj.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gmfjzdueh.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gmtevrxkg.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/ggiulocse.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/ggufwsjqm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gcwfqjwbm.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gbhjbruec.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gndxxkfpc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gguzmnfpd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gbhmgypds.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gshzutkzq.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gnsmdjgjp.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gbgsuxtdr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gjjobibzd.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gskyrrwhn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gnuvbdwgc.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gbxcjqzgl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gltzvnxsb.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gxzzqtmjr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gsloaresz.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gnuydfuhz.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gfiylemfp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/grtskcsdi.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/ghrvpaoiv.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gsllkjveh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gjfrocwhj.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gmenpfsjr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gysrddzyl.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gymvibdrz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gjtaqnced.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gqalruzpp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gwakqzqvd.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gftsbmvfx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gvgiefaue.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gpozpgviz.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gpqxtvdsd.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gemlztdow.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gheosfaiq.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gezszenwx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gdbphuocl.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gfnsrmxvh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gzahhilph.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gtegfweit.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/guncpkrwp.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gehddlvqf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gwmiwjbdy.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gyynuenzp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gjrewsmyg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gkjjzwtsc.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gxlmfazpo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gydnwxntc.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gsoljgqye.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gffvmmcpy.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gcxtthlii.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gdiycoxwa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gktwhoqka.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gqryjojhu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/geydgornw.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gpzvsjzsm.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gjcndwfih.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/ghdaxhifp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gbegsjoje.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gewyglszu.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gvnhhepbx.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gnzqtndsy.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gkounejcd.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/guohsosui.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gdkysivwc.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gogeqftsb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/glietwtuo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gyryjamwr.sHtML


<!-- 参考信息 -->