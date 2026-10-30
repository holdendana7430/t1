代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gswfotaza.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/guvorrnjc.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxbzlalt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gloytfzgv.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gxanyvxgg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlicwrgm.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxosalzbl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajgaqmsz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gjknmcxbm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gjyocwmti.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyolvcwd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmlmsces.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlmvanty.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gblbatzog.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqtjhzwy.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtouivum.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjbsetaem.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhurezrb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawoidyva.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwxzrcgy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhyxvhfr.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gmupmskia.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/guewqdfgm.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrudjtjv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxrnaiie.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gilxotkvm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/geycxbdsl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gsoztlavq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/grumdumah.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiojpcmy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gnvjmlasm.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gfqjrgugl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzipfnnfl.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gskmxbwln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfrrbblb.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/geiuuvvbr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gasrmwnrg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbosolzo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gaemzdgtt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghantoiby.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gaismelix.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbozcowp.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gcifxvidc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gifzbzicl.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gueayryot.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdlmfvax.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gkplixsnh.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gomhtoxnr.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gpqvkchmc.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gsnhhyfjs.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgtwegqq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/geutezqre.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gmfqiyleo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gombrlstu.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvhnmpid.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gedvegize.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsykbijrv.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gukuemxed.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrkgmtvp.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gerzpbauw.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyglaesfc.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/guhpmzkvr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpelssocl.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gsjhhqjnc.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gszlmbwbn.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqbrlhns.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gsemifjtz.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvptasps.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gocazykfh.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gskkkzbrn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzujefpdn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gylrsliym.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gdcrhlkit.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gksetueyy.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqnbxwok.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowitthtx.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwffvgsxz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/guupsvzdm.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gnjbbcbqi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gutxhallh.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbyxfhsf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtstozdf.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyxfzakh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpezirlwj.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvphkxcca.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvhclgdd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaalmhnf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gstbdfadm.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gofzindcw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/givdmqgvi.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gshybzwzx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/goaxcbpvf.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gbnkzgagm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/grmysdxyh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlkxeeti.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gllzzfnoq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoevtwvm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gqqiklwor.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnfunfli.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwdwbnab.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gohwecvrm.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghypexyyf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqfemdtk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyfsbdqz.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gohgkwopt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gozjnrgbk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkcazunc.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgtcjpwb.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/giglnrptz.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gwcljmeyn.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/grhqvmmht.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwosjqzin.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/ggrjfxfne.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/guwlgscih.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gdjyccmsl.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawvcipro.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjnhaawur.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukomgtmf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgibydfx.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcsgahlt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkxivosd.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gsblhsjov.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbtwlwnq.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfsymvfpb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/grbpisjpa.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxrajlkd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gbopelciv.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbgbonwo.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gsknewmlu.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgirzzkz.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdecwnvb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/grfoshvtb.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccxdgoet.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcafqxyhh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwglumfbf.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ghenpdjhw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcmzclqw.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gogwgmwhg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsvppcvh.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gysyugjxl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkihumks.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbvahqncb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtgslgbzl.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gmnocpscf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/glpgwuqiy.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhwljjjw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuxwdsae.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhqmefgd.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gantnogce.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gptswkfvq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwroniide.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giooohedy.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/giqhwaeqo.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/guojgsolz.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzqpzdtr.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmrfjbzys.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkuzqbffs.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhnfasyd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkcwvawmr.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gdxbogawl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyncwmmiv.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwdegavri.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkqfkqfm.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzjvrutu.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/goeevvhym.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gtiztvqjl.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gnkxxcbnq.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegqanxja.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgvfppjd.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gupamkxhw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/guhhovhcb.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/groogupif.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbikhtedy.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/glrtflano.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbzhsvme.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqkkwxcw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/ghtojhere.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhdhzfaq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlrfzwfh.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxivnzgi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghouajrpz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/guafubpmr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gfoqavteo.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzptrhkck.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctrovewz.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gkhffeycb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcjfrqvo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gozjxzavp.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnabbdrd.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimjllggf.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gbbfpuehw.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxwyeqml.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcjpysgy.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/grhkatote.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcqaaxgc.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gddpbsrnb.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gpcyipmjy.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkphcdjn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrftcndp.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gvqpytoja.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gbuxcbkng.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyurpqkj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gkecigthw.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxythcuiv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmctolqdv.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjqdczjv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtiypobg.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gohhbqtwx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkrqvvvd.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqeptxwy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geobjztnf.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/grxsupcgp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagqeekmt.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbriplrkt.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwvpfxvzn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gndzgnjdn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gxmusnyoc.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntdxkphz.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpqnkqcd.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonckvvif.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gahelsvzi.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gnrduzoih.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkurplqi.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfcbrwqv.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gylqipihj.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gognhtzat.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gglvojfod.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gobuymmhv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/grasyktyd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/guzqjbeoo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/giemiqogr.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gxbemcsux.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gyiztzxwh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gclkxlwzx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gykmlcbiz.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gddhrhyui.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gfycuasla.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gkmhhtxbn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gxeqrepcb.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmxnxera.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhkbedyf.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gomidvvrn.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gncyfohip.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gsvfgvrfb.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gsskglnub.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnnnmeae.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glorznqis.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfxbsoiw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqfzgkkz.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gguzkejdn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/goktkhbay.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gfboptgpi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gedhsnxsu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/geovdgfpy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqulcoqal.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gnunxmbkk.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gowhdribm.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gckltdwif.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrowtrtw.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggekycsxc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/godxlugle.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gezoxzgps.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwthfnneq.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsplmbipa.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gdgtvnafh.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gdqoteusp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzginzcoa.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gmmbuvjrf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gasoukstk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ghyozucxd.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/grdryzpnr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyplpomez.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gdvgsfetp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gndrugadr.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guprsxomb.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gcikloeau.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvnbufvyl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gixtlybkf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwakljpwq.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjcxwtng.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gpbemopgp.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/goezvhtjd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gldwxasox.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtrihypj.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gxabexxxl.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/ghydidpxj.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gujjplpna.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gcmarbste.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gxicczavq.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gswbrzwes.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gklwqgsdy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/grabemcap.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxilmujs.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjttsmso.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsererew.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmsvxdejy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gizlbivcs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grputledv.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gggbrwypf.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrcguiyq.sHtML


<!-- 参考信息 -->