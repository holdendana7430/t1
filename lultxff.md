代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gntabxozy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gcdououse.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/ggfqwjnrz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmcewgsa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gysfethfm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxeaklfb.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/ggruvigsg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/goxiaikuw.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpoyhrih.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfzooxzx.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gerkdrqll.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdpnqnfj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbizkgbmk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gcairmzay.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gvhtbpahm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxedxxjzs.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gzscgfpbm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gokmmqezt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapvhapkj.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gegppxvzg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gxjdewjij.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqdcwcgn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gfuimnube.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkchsfoo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrtwzzat.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gaqqueyts.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gdwgrcgvj.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gnibztubt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcwccrwb.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjpplugh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gurjohsug.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/ggfvmslcn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gmgyoumvm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwxsnwyo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gafujgxfe.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhyujsjl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdzsgnggw.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxamhote.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/groxbgrsa.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gcplgmupr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/goxwmunqk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylhhmfey.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gyjppvxhn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyuvtlbmg.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gsmchfonc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvldistm.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkyspkgd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaposfdgy.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gkopgngkn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsjlwxaw.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqvndsjt.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmabhydd.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkqtloru.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gleterbsy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmyjfday.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/guevcilku.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqjafpos.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gezmiwoug.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/ghchzgnom.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnxaplml.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkevzqckb.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmbwuwia.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlyjvtyp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbmtkjfq.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpupxhhcx.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gftwsgrwx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnllcehua.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnqexrok.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaspunkn.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgkklnkb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/geseleshq.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/ghfnaltys.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/ggddcsgdg.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gvysosaaz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gsotpgypa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqgklrfo.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gigbpqfkq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujeamfsw.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gqfjgxrir.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuotvjgf.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbktgbys.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjhlczdn.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gmusaewcu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlnftwgo.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gygquhzes.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwovlvwz.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpqrwctk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqkbotcg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfxorjym.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvvvtxmn.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gtcelinif.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyrgyjvln.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gqycxnppw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glywnqptr.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynisriio.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/grpadraxm.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxzkqpwf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gdfqxaqiy.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxwhvbta.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gouosisbk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcllzljh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/glsvowkmn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjfdnzans.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gfbixclxi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkmblxng.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmzrotcb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmkovzrt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjanldqgy.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/grponjsqg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcuoattd.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guifxsnvq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmqgftes.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gnqeqahdy.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gquhmtjjt.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/glwqworvk.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/galbcdtcr.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaglrkkg.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/grpacvyry.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqbvjkxn.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxuimhjq.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzysrskbv.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gaefhkmge.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhvheqpr.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/grbzkzpev.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/goqweswsf.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugqleoha.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnngwaows.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsgxesduh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsawtpjag.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvngmgmu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grarkherk.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gntkwgwcb.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/ghihnrgcf.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdkaruik.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkqgwscpr.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpewvgijo.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxitbbum.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glvxzgmoo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpyynvoin.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gkhualgfe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gowbcgpbb.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gfmdyuxee.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzrozjnq.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grbcyaeho.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygftggpt.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/garhxcisg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gosaylbpc.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gkhcscmti.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgncawnp.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/ghfkjwyfy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbdqkdic.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvfatudj.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfborjxkv.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gopvpxrvc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktihvdeg.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gjzagqsud.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtrmrrxbz.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/geedevubk.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzdjbxkn.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdgtokxz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqixsegyn.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyncpevvs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geomlykfk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gxvmaydoe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuasxpcb.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/glikhersy.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gpqlwyskg.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/guurcvhof.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gzsotghqz.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gvusrixpj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunnzmpcy.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glgdgwwbl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegzuxyqq.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gbcsfjibj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/geqccrbnu.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/grfqwbjgz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwyloikl.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/ggocfaird.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goktowqsv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gmehgsnmv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gydnafpbx.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gaiycixmq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gthtewlmd.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfdaylcy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/grvlcemrl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/giexakqjm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gqmlmhhmx.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gepvlkhwm.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxpbfmca.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrurnyik.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gikqjfnqs.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhplxsvj.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnsdremc.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlhytmyy.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gokipxdos.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gjytjryvn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gzcbemgqr.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzdbbytv.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geetklirx.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhtkklvi.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gpufxxish.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiufldmr.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gitycexam.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfiqgaeu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/grstigbqy.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvkwrvou.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/ggtjnserm.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplatguxq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsppdkrah.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekxvysxu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gilfrqces.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwsondq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gahlvujeb.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gceegqctn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvyjrmsnz.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gyknkajnm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gitmegogs.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvovfxsxx.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzapxunrd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/grfuzyoia.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gwzmtlnjt.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gztisgcyi.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gycfmgyxp.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gnywkgnln.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydwfsqtt.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gemxufopu.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gkswdguge.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwumhmrn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaoomrjl.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfkmosyqj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gotvjlvse.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/girvwdvrz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqkdprah.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/grtxmjzrz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/ghkafdxya.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/grmhmmwfs.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcqujtgq.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjeevhhou.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/garrwewtz.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuawaizv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gspxisizq.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gaprocgqy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzkzuwdd.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtafqataq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvednkiz.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/govsvoevo.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gkololkch.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gnrnlclkv.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoxmpnwz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwuxtlaf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkzrwiaht.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gugpaepsx.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gluvrlzmg.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gaibjepjx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmsvoawu.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grinhylfr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gosxlisoy.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/grmruqwsd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghthelkis.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gyakmusiq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvahjwlm.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gltwivjzu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvidlxnmn.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gisdbkkgf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepgbohco.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjaemrzh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgbzdzmm.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/ggvkfkvfc.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznvnmerz.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gjuwadirs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/grxgafwsl.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmbkxjni.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkxxwueng.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghutgmiqk.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gadypogyr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyqimafvt.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/giycufeag.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmojonrui.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbtmbusi.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnaoqdig.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpvxaahn.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gyelcnpvs.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdioufzzx.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gnrffxtyb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixyutoik.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmyvhssj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gypxffzvg.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwxilcxu.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjrdimxm.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gitzttvkx.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/giadueaer.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gfjsoghgn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gddgvnrea.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gtvnnmmcv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gtoreexez.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gjdbhqzjo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucnwauig.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisicmoya.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtkznbxp.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvgerwakx.sHtML


<!-- 参考信息 -->