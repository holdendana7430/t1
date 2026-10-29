代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gecutquod.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gpmqulkfx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gqjnwwphg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gmxejwkno.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/ggotqfgho.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gkyyoipqf.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gzixqapev.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gudqggilp.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmunxkvxt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/geplufpat.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gdcyohgws.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gyovbrhet.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gcdwcuxim.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gwqflaeal.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gugpixomb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gunfjzeny.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gvxhlfqju.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/ghgbvcegt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gkdqnsedf.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gtquuchsc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gzzmqoyhq.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gzboemspe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gcvgubeml.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gnxxgmcxb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gbqdkxjla.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gyjmliqra.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gsldaaugt.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gtiylqepo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gwjfvzxqu.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/grjkzxdxv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gsoagjsyj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gcxezynzs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/ggexydunz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gyuecxqyb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gqoynuxbr.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gqymgffes.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvechkqel.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gicljekkd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcexjrvfa.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gwvahsxpp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbrztejhe.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/grlcfztnr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gyliwvxyy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxguouxwu.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gwfnmsscz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gluklfqft.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gtokmfpls.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gqfowszkw.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gsuorsrnv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gfdhmwscw.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gmjwncvmn.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gsglvotyy.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gzdvhwlnv.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/ghcmpjted.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gttrmkoyd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gqxlkdffi.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/guoucatfs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gibjeepqk.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gjzppsznv.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gcuctltru.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gkjfxxhlo.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gsxfudaip.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gmthekson.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gcwbpozxb.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gxuwccwnp.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gxngxawro.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gqgnperyc.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gvwwkxbnp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwyvjmioi.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gfrgzjjmo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/ghnrzhsiy.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gbffrwkig.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gejtmrcuv.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gieawandb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/galwdwsjc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/guvijhvax.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gkxefqrtt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gjnrqtnfg.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/govvyfegr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gblenyecx.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/glrkxozwt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/geokpffbl.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gynsfpeeu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gdaxciugu.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gjqhwdebt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwglowkpv.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gqultfdgf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gldlflcgm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gyxkokcss.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/guabgcypa.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/grlijoybh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqjzneszk.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gjynlvzdi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqleuimol.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gxlovyham.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbqgkejh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gfsmyrrho.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/guffouauk.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gbgmsmdrv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gxmmepgca.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gmqjegxts.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/grdbvljck.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvqpsboxj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gyvbsdjnw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gqbiphzoe.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gsgviuiwc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gycvxsqwz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxweghfwz.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gzdlciaxm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfutfhynd.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gtrrsurtg.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gdisogcwq.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/ggiaebsbv.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gytijekeg.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gpsttpatt.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/ggerovbfs.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gxzpdoryl.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gkoktwrrd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gnobgjvyd.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gtkpmskqc.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/grvnrnmon.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gzugxvddc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gphwghtzc.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/grjtuvxuc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/ghybyqzyz.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gbcgposas.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gnawxcaou.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjcxkvckw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gkvekvyhc.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gzkwdgzfi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gmfpnaikf.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gjvwiwvvo.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gypqrsawg.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/grcictbra.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gobhrjogy.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/glphsvylg.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gxwrstpjn.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/grztkqush.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gyhzubjca.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/glfsidgxn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gstoqdtji.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gdpqtjmvj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gduywzyvr.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gulnmbwgt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gjpqbiiiv.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gnyqqriqi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gegghacjf.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gkkmwkhov.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/grlsbsggj.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/grdzosrdp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gshfcgmie.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/grggnmzeo.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/guwktuuni.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/goeihzgve.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gpgcyicvm.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gxvuwumfb.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gzazqtkzp.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/guhbuthvz.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gppjsmwic.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gshymwhaj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gabwrvrqr.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gahbsdhnx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gefchzrcu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gajpnobjt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/guovlajgw.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gzjkjubbm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gzlggrfjy.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gluxilabf.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/giwifjsvp.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gjrovvgia.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gcgwbuwzq.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gkpdajbfc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gdgkfddvx.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gycakmdrp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gjundttpw.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gbinhhpnf.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gdpxblkmj.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gabtyucjw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfayoeseu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gewgcriwj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gdhmgepgk.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gwpwswdgq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gmbdvmouz.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gpozystdv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gbggfclbj.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gujibgtdz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gxzmcgcxy.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gcniokeco.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtasvnsm.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gvjwirfvb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gkmgsknmb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gieeypyog.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gmkkvestd.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gokvqowra.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gmlzjrpvg.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gerkbhjdx.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gbqhetjzh.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gegrjvwsx.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gxloitguh.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gfbmocmux.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gdrbowkcu.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/geskohose.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gircltoxn.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gupxcbgun.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/ghjimmrpz.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gdclcnnhu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/geojiqfxs.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/glaqsnazl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/ghzpwidah.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/guqdlegxf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnqzsdkog.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gvmgsjllv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gnbzbhmbc.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gydovvvux.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gibnosdup.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gihuccxkq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gxkbgcvhm.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gffmfwoxs.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gqnvrsxfy.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gircauxil.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gftenxcke.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gigujeauv.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gqibhpkes.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/guxlvqfsx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gvoegjhaz.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gjblqncri.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gihcbwsqs.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gnebylghc.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/ghdsnklsa.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gqurjjftx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gxzqqzonj.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/grypzqxjs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gnbxmicpf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/grwcqnqcv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/glnuhxbkt.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gjrhgykzx.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gzsgqnnpt.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gmcezvaim.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gnmmjzgjv.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gfdalaxgn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gtyooxyid.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gxgxmzfxs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gypblpfps.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gwlphzghi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gsvapoyfm.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/ghtwemoez.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gtmzciues.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gxcfacris.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gpubylnju.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gicolbjzi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gbjkigexa.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gbbtjpklj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gvzdexsjy.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gepybymgl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gcviybauu.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gxqudbjtj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/glvpgxrna.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gauyssgxf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gppzenitr.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gmwtvmwkk.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/geylenryo.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gyrjvqtep.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gghrhyrmd.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gvarvumku.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gkzcrqulf.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gbruojvcj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gwdcqktoi.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gqrklagnq.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/ggiitdrrr.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gayzfzzzq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gsjoxcmyo.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gnenaebnj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/giqyewmwo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gcqeuxace.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/ggwxbxnzp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjrdhbdlp.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gypgbdsqq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjooxeoyl.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gqsvtgelt.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gqmvhtqua.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gnkjkqmnb.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gihmtizpk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gggiakmbk.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gngprqtne.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gdtwcltjo.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gyylpadjv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gwybhabfe.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gmptmqjkj.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gymboutpl.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/guqnwdlqx.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gjpiewrcf.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gdqodfhko.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gyzmbtaaw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gjucmpbga.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gbhqkucuc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gwmgnmdfa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gusoyruyf.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/glkrlvuwi.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/ggqipidsa.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/guenycoyw.sHtML


<!-- 参考信息 -->