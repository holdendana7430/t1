代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/glgzbunju.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gmqmqrmcs.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gfrnkwfoc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gvoldhnlr.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcrshkni.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/grszinagl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflxxefir.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gehaqffku.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapfefclc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjwmlizh.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqlcsbnw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gmwwuhmuh.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyciaopf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxulfcnk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gtufcsixy.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gntmiibkh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpmvuubv.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/ghieqmymj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrfruzig.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsywbqlg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gazdzrfgg.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gedvcfmir.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldlhypss.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gchsgydke.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrlnmqdp.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrjbttwi.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gnxegpxlb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvixpkot.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gjhixxqek.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdynthvlc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvikdabpz.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gscbmasvs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwbsdtavx.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gsogcqiqr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjedzttw.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/geljpvpnt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbfqywbez.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgsqprmt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gyvqaitsh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gekvaawtp.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gfkmpfslz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvgaofqh.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevdcwdja.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gsijnpmor.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gcljvimch.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjeklats.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjquazskn.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedtuyepm.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gwwmijqfs.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbdrwxgu.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrnnwdkl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyeggqkp.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gjthqxnzb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gitxzqnvd.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gkiznsnvv.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gihvequhl.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrmglevb.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gkqhaweyk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gxxecufli.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdkzltkn.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwwmlvsu.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gycnmhmcs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gszlttzok.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gwarsmbfo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbxxaxge.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqroaqnzr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfadmbje.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gclitrthj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpepvrebo.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfbaggfx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvusslru.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxaagful.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkazpkhyd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggamwcvmz.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsjbgbmt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/giklevzlc.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gigkfnevp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gawehvnzo.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gervjwfee.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gtryfjdld.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gdapapueu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhjxebnr.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvuggixb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcffcyyoe.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzjfbynom.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggealwarc.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmesopqhk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfrncvcl.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoliilwj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gusxwclev.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gxqxyqzdr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gswwklrhw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyrvwupf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbrfpqmq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwncsncpx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlsslycr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnxcmtsk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gzljznvkc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqrbgowcw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnyimutt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gyjwdekrb.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gljlqjodt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gdhblimoi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmaelcdqq.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaownmwfl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiczhtkf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdkfhlgx.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grruuuwnv.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfmtxbtb.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjatenxnk.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvbvqwbw.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmnrwjel.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/glkcedybb.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidxpthky.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkmnyxpr.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiqeehjo.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeuijunq.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsozluaq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgficjnk.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxswsacwi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsilkkido.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmwfnmoh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuebxafx.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtkcnmzis.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gikbiqaws.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfcyxijl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gcyhmyfoe.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmtvafrx.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/glwbqluqq.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqehecutx.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbiovkqru.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gutspbxtx.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gmkfwwwap.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdpancot.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzrbklah.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gcczanlvu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjihyjhbd.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/ggrehxutr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjlwdadxz.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbczlguvp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoviaysg.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpopkovrs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghzdczbtk.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxyjtxdi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfwrabbi.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/grdrkdcyj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgpatpyg.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgnekstc.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxlupxrb.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggleopyyd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggctirxmb.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzutzmbm.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gychtzpkw.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmismbnkf.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswzcyrui.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfjvinfy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmymxyzhz.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfghbhol.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gthitegeo.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gzadjhsyg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsanwpqdz.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkdjscib.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsuvanzk.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/glyzgadws.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnlaonni.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqftsirc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givcecqen.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtpztfqx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gwtfqbxdx.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gvbhswylj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/geapystic.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdijdleit.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gizpaynks.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gehrwteyv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/giakzfyoy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjorprccv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gjxfecmkh.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gyihqwrgv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhuxctqd.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzzbexpx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gprxmckva.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/giwennxhc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gvfgewnbw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrkvwtsp.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjilgqmku.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/guevdvcjq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gvyifxfdb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyfpuxsv.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/giyektvhn.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gladhgtez.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gglwnlvid.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgaihvpm.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ggdqpyvsp.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/glaubkadf.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygypivsr.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfhvhzbio.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gyunjoceb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzgmcitp.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gckgksvjv.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gwzpeaeia.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuygcirf.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/ggosrehpi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gnazrdwnc.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfahdhnq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsjpxusz.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqahzbcqz.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfhikqkv.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gemixkuqp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbbggpnm.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gkckylljh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gthhwgntr.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gdstpshal.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gcakdzqvo.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhuhiglm.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gicfgiode.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gadyflwkt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzymhweb.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/glctftvec.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbguufhs.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkulqnzt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhrxsuhn.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfkgapcl.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gcatcblme.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsuvchth.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqupecfr.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwwyunhp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gggarpmax.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqhmyfnd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/grofbygnm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gpgxmergr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbmlbomnr.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdtaaxps.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gezoprlii.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdrbbtpef.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gcocdavmm.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/guidlnzbg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/geghfspxb.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzhucoaz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gzrbvdmjz.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gltvaoelt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyleroyo.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/ghoquphow.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsludshbi.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpkbcret.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gknwvucxe.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqpnzoei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxhkczale.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gufymdlnb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gictibjye.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyvkyvmq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gypbxuhaz.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtkeqdor.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqxbhtcl.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guflayrvq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwmzbqsy.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgprqxiy.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gjiwcvfqm.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gbsaeseqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/geskmgjyy.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gogxkbawl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gfurofckv.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhdxosxn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngtblttb.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsnadepg.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gevoeajpp.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gyuddvwrr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glgcnzuvo.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gyfkvwwed.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtpvjnzv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtpkhyue.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/ghsjmekvt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzboqnyhl.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvjmwkfm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfezvwrti.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsjgnyij.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkzjhtrw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdpgzzlht.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gmazoeowa.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxeicccw.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gbbtjzerd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqlioksu.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gbxmdpzuh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyzdqzxu.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbnywxjvi.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfeylpnhx.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjolbjxe.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gktlsievq.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkzzrmamk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhycehac.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gtwscdjbo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gizlxldar.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginljjsuv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/geqhpzeqd.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gyrcqifbz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmveiyzry.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltyfagix.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gnhhnukos.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gslaygmpb.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnenobizc.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvszfshve.sHtML


<!-- 参考信息 -->