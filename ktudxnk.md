代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnsayqqg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqyedzke.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gidsrdfyf.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gbbrqycud.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwrglhbf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvuemtwh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gibjhofsx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gzspkpdsw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gdhzthnbs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gxymkxavs.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxtpfhcx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemxtvfgz.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gakqzwkjl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkwmwfgb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtacbkmk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/ggyqbwaef.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gghosgycl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gpghipoij.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwjckngm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlwwkkpd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyvjgaok.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gxjdtnqpq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gogotzush.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/ggshlrpfm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsbcdnup.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gfbaqsgrm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gevoyxsvf.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gtmsdoztc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkgaidmc.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gdbqmwsuu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhpqzfrn.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmzvqkpa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnztkdmgs.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gyovtrakp.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/goryzsxma.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnbicmoo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gdcoxvdwh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmatucmwg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gjvjplzbr.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gatmgabzd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmggqycr.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmeiuxry.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gwpwqyeqs.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gslvznpkq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdlpgvbt.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvjvjmrt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/guplnnqlj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ganwthchv.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkudppomz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gyemflgqb.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gfldunfqu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gcwdcfysi.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gssobltzj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gapjmtzii.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gtzaeypjs.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbtcuffv.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gcmetbntm.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gmavmmwhc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvavqhxei.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxvvvdyt.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gwusntpoh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/guxcdfblt.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxadedzpw.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/govclrsws.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gafubaoiv.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gojqxjskc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gliznslbm.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gxlaotbug.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/galeilbca.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvalkljl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gvskijtgm.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/goiksnmpb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldlbhkxu.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfurpzbq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/ghljicwqm.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gforpqvgv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gihraouqi.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrwjtdpb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gdxbnuquo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gnprtewvx.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisidgnoh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhrfcdbb.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gntfogcfu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqugmwwor.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gbdguoshl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/grmsqstkc.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdqvybdx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gczkmjzkv.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/grzwfwfjo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghpmcomio.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcewawqx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxayrxlgn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxarkxrkf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxeabvqj.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gsatinbld.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjwdvgyr.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gnawbeipw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsozdfku.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqueearvo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizklmrlf.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gnutmiitb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdebvqoc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkexfsopg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrnwpqgy.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/giwdyamnl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyefnbzy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gejspgjny.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzutuxeq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gimdjgoni.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrbbmocu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpoaxhdj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtznnbsbj.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozednwiv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guzjddjws.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gftwywzhp.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gtdzskopd.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gtizcciqd.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjbbxoxy.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbetjkxc.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxguzjrr.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gsnjincqk.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwarsfgo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gufhmxikr.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gimjsaqyr.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqgaqdsni.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpxokegj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwcgezycc.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gloymloab.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjvuxjck.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmkjdfqs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmqrehqx.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gakxddsuf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqadfqgnp.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gltnqnnnd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/giyiqtxfc.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwepowrd.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gzhystciv.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcmwvgij.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyfddcsh.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzyyiarfs.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqxmmuog.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/godggjltv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtxzpogo.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gkkmmxerw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrdppdqt.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwivfpgxv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gupmqnysc.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmyprdnxu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gaclyczgd.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grelodiqy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcnempao.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gllkfviys.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvudsmtb.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gqztbnkqw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjcuaypxq.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gyrmmrfbm.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuotfsbc.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/ghhmbqghk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmksgqgkd.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhypxoxk.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqalyuud.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqhhrivt.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmicxbmbx.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaynlzht.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcdxdlbu.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gygkdipum.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrwpneyo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gqixfgluj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guymyreoo.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/geibqefgs.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gniaxypzp.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gqhfeexql.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaimszbmn.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfaipvuz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrfzjdmj.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfxntcp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyenmxvyj.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gatadwsox.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxnvhtwl.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glqkfynzc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtenajvnh.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/govpxkfpz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjpzbtmlc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gpknutaoe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/geuabjvvg.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/ghcospanh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/ghybqlpeb.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gbliwqrkq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gecdncgia.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjtrfqps.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gvklxhscz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlvkjytq.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvluuhoa.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gjmajkdvt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gxzyoczsi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gerjrsswz.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gjqfddxiq.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwrwuuqd.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/guqziezur.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gyokyulcb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/geiqhfwfy.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gacucerpy.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giozhnddv.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghyrouwdt.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gjinlijis.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gzlodrvei.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gncoittpn.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/grunscoye.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiktbybe.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpapslvdk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwqauvkj.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtuxczui.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnubufkgj.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gcfqirspw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkafgtju.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/giieyqian.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gryzomflg.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gcyxmmvdf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwurtfue.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/ggwrlbigj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjtyhhqu.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfaerpaz.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geklqdjhv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/glppkkien.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gagftzusd.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/goiqikibj.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhxvystu.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gdjmaryin.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmmeiucj.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpikxzch.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gzmocgydr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnlyftnt.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxtapgjj.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllnnnfdx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuhkobxh.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gdzmatfnz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gsijnnypv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ginpsgrfi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gufpxejmw.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gnigenrar.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gyvfxjpku.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglfnztwm.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmlfaoxe.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gsghpigeb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjbcgkbd.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gqmwnlxcz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gfelvitye.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gforvusgf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdilkkkef.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gkgurlktp.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gcorzypms.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/girgtxyni.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbwueblc.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaicplby.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiodciti.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/goirtnruu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gppvnifuh.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmdssyez.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gueywlfgk.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjibpgsxa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpgyqqcx.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxclgwuv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpnnutcdb.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcuamnkl.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgqxsjiv.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjvsojkq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxujuythz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevfygxzn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gsrminaqj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgxpypgl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/grgibgyta.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/geamapgpo.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnyrjbhk.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gpwyhfram.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyutzfyex.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/ghzaeckdc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwegyclwp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjutxgtrf.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkulukux.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdskvuaq.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gsadklixp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmxhaagpj.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzywyqxxc.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/grxszbocj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiknmzrp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvqfkkhy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gztmfmokw.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysihsvxn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjhgrxml.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltawwoud.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/geyamqxhw.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvygrzdt.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzfvjovo.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gujkhrpvr.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gwyovhpmm.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/geookpcvy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypxhivka.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gkahvugfp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gzfyuuibp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyklazgm.sHtML


<!-- 参考信息 -->