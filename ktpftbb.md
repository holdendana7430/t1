代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gzcbuiots.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gusvlurza.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gjotbbdij.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gmwgdbnyt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gncmfvgnx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gdujwjcjl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gkhdzyged.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gmgwmezcz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/ggmfjfuzy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gnnshqxff.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gwbdbwsjd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/guwteqxsu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gorzwyjna.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gdemehbnb.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gubycpsym.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gvxucktwz.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gouqxuvbj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gvdaphikl.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gwermrmld.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gvwhbnkei.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gzcjvdzhn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/ggnrfckis.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gewyjfqkj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/geystgbha.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gbpsaopey.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/giwabxoid.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/goznmramg.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/geaganxul.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gwektyhhw.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gurbvfgpb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gbsqhjhma.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/ghjdgvsmd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gtpqtvtql.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/ghaagfnpa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gwbxwtgxw.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gqhhzdkff.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/givgrtvtz.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gylolxkpg.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gsqvjqfne.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/ghruglbbs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gkuseppvi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gotgtmzie.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gcryhwgge.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gdpczddeg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcqibbbnq.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gwdzsglio.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gkwnizqht.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gwkqttnex.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfrljekqh.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gytwnadpx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gwmrabkzd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ghdqfepde.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/glhdowgww.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gcfbyolyi.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gxlgspahn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gxtzmbzbs.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gyictqfgn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/glkbhvlpv.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gqtdtjgtn.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/ghdhzhrto.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/glnnyfguw.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvqguwcw.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gtxecitxb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gyhcdqyek.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/grzmpvinu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gecfzhjsh.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gtubzvcfn.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/ghuwovpqy.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gkxlpxcpr.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gquhcyesy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gmpbtjicl.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gzipwlfry.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gzpxwxwvw.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/geovdboxu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gbisenxqs.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gaigecbmq.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjxsttvtu.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gbkotwmuk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gztlarepl.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gyuzvheba.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gyskfqsjc.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/genkwwfip.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gaxgtypfk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gvniyevgc.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/geajvvcnd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gncutsikq.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gkmiwqtwa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gmaimmocj.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gelyfsden.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/giinavepz.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gajvuebbv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/grttuwxly.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gjpdrxlpf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gtlvmkdml.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gmsafvpmw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/geouxwtlj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gheclahpw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyqukmtse.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gnbzejjet.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzonmlmma.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/ggggwwagk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gduotzgom.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gmfkwhnqu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/ggtxdlvco.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gtvjttmqm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gpttyjnir.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gjjcnulev.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gvpdtjywq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gumthdyvy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gemdkfxrq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gimdlhvnl.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/glznhhggv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gfcodayqe.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gohmkgijx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gfnljrkqj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyjydxtmo.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gvvmqbnru.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtqmofhqs.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/glmpbfyck.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gnridkkgm.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gtrpgbkkn.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gdtccjkfu.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gaottodla.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gztsdvgai.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/geopashtw.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gliqfxwja.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/grzdkuaui.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gwelsnjqa.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjsghnt.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gbipwzckt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gsewiyalv.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdlqjvsfd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gfusjxvwg.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gsfxwwlpa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/girrqyupg.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ghednuatb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gzqejkrja.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/grnriduox.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gnctmaaqj.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gnhguvhkb.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/grskrfdkg.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gfldhgtbm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gwtgzkrkv.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gtnsinfqk.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gjvvqvqdk.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gzgreirpi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gjjlqhvrj.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/ggzfklwrh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gjfabvlld.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gkrumproh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmcvsqbql.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/grddhecek.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gqvlxmwnj.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gpxrewqca.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gtssyhkpd.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/galmdkedi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gcxvdwnrc.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gredppsvh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gxywrspfs.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gnywzgfvz.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gnluleizr.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gspvtynqw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gfogpvmwt.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gedvfucif.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/ggugwutvm.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gnzffjczw.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gprhtcuid.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gxefqoijz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gxqjkstbc.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gfotaqreu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gfcrflyti.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gssxvnusc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gaskkpxkr.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gymudimxp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gyyfdmqgb.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gfqdzervm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gwyibysgr.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gyqbfhvms.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gamcmdzga.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gxrcwenye.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gtqdwuims.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gvnwnykvd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gzkjeyjcf.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/glhaysuqq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gmcdzwoqz.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gtclehrhk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gbixgekxd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gaewydrtc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/glvmyvzcb.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gdvtznktj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gzfzyjmyj.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gcnwryjrj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gjjicsatc.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/ghhenaxxx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/giipyhrfp.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/grzxotudc.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/geyxeqgiy.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gmixxyczo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/grpaoxnmy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gqoxqqhgr.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gexlqhinp.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gmdvcnois.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gtriskhit.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gcaqmjgzr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gjwtjtary.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/ggmyrkbcz.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gkdqnavqj.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gpreylshf.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gdmdkvxvx.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gaquercsa.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gwqphaaws.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gdqpfpjri.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/ghdvibbim.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gnkbthgsx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gsswjvzak.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/grpupvrxg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gepmyldxy.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gvjqywtkq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gflrxilqu.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gssbycjpt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gkwbepjyx.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gldplhchm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gstuiropf.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gdlgawbxq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gkoikddgv.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gqywawvat.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gzxhcjbpl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gzkzspqyi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gimlhodul.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gabgjpkeo.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gshqgdrfe.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gowysqtnk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/geeeanpcb.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/geocggsoi.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/ghjehtxjy.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gfrgcfrqs.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gteykpdhk.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gphyfutaz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gnbnhbtoh.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/getktyrcq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gqnemhmld.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/giicpekrm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/grceiikok.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gaijelfpc.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gjffpsqsh.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gwaklnekp.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gahmpcctv.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gjpjznpus.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/goxiimtvh.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/grnamfooy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gguywvqmy.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gjzcqhmyv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gcxulogte.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gbzkousjh.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gavilfniq.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gcfvkblft.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gvqpfrqtg.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/geqqxadyr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/giqpgchty.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gkkjlucrd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/geberyywp.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gbzqlasyn.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gpcqoiaxu.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gjpbgmqhg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/grcinnpre.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/ghknbpmfe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gisfbakgi.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gmrxxjqcl.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gpykhrmmt.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/glxoemcmg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gbthouksr.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gbzbmkxhq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gpqtmhpgo.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gwjrycqxp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/grxlvcuec.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gzpeegngi.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gtaxnnpxi.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gbpdteyqd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbluepmuw.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gjyeigwmu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/givrfonwi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gbkjnhdae.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gtlzuhawl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbxpwzpik.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/ggdjgjgam.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkdjmzpbz.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsuxzetse.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/golswltgk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gazrqrthe.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gpqvjgcza.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gxvvdvjpy.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gxvgruiqh.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gsynyumkd.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/ghiuibwke.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gmuankula.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ggycjwtwy.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/ghzjxbuxr.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gwgcvgvis.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gebbbtmaf.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gbtsxnoff.sHtML


<!-- 参考信息 -->