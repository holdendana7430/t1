代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gwwlxhuqy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gndcxlqbc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gqhraoudx.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/giqzcsgwl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gxnfzuhcm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gjalijhoh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gphegzrur.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gxsafyejq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gugabumgx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gcgneiaks.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/girfvnqdy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gesqfawrv.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gwmorcfld.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gmmuhphhg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/grxikpxmu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gfqajktjn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gbjimymas.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gscapltmy.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/giwdbmons.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/glgfmqiaq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gysbbsrpc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gytlssrzp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gfnyqkylg.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gwuxuadpf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gmkbcomsd.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gyrznvdgf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gxuacowyh.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gkjaiujod.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gfqfvnytg.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gupvkoglg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gtfdtjzev.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gilrefust.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gcqwjbawc.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gjaermlsz.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gvuypdeau.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/glklnrfro.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gyvgzpado.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/ggywxptkx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gloltgnpb.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gvocsvbvi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gxyafkcve.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gvsmrvxiv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/glrrzoilt.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gvowwlbtt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwmrvulge.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gsdrigjly.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gntzjgawf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grthhydke.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/grbqjddik.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gfbgotamn.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gahclbbas.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ghinkcblp.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gduohpiew.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/goyaifqgg.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gnjygcrhs.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/giyuflzhw.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/goalauonu.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gecbydthb.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gbwprambm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gohsbyjqm.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gotjqstau.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gnjfvyvha.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gatpuknqv.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/guymdfxgm.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gwnskwtkg.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gpvosbsfd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gzfnbvszs.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gtbxosuqj.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/ggxbyawca.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gulmbphlk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gqtjbtnng.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gyvovqjuz.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwkqasjgk.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/ggteqwbab.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gjohreoiz.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gtjslgpfx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gbajskzme.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gzzxnhgpk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gnaazualj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gqartqiit.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gcdildrcz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gojqylppa.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/genfzmwsi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gdcyxnnxg.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gulnqwetn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gdmbppqas.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gqsimexhk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gbczjegdn.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gvnddbsme.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmvxstltx.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqazxnepj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/goghblxei.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwpdjleiy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxvququkl.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkhhhlxkp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gyaovghqx.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gniydozmr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsvnpimaf.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gejmeabdr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gpyasdjeb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/guzlloxdh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gpyfkotrx.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gltxxqtop.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gyimktncm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gtgiqtiip.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gcupwdszi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gubbdzvkd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gtwpalucy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/ghlvlgoda.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/ghcrposbf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/glntjidqa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcnjirxrh.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gywxotsxx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmwjptkxq.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gmqqpxavs.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gtfizlhsl.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gpwmxsksj.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gimcjdexx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/githbggkj.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gmbjtuafz.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gkqcuguxr.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/grksqteto.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gbyrqxalb.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gfnhwreoo.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gyhkvqktd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gaattkrlo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gcsaojfhs.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gfbnkbzrl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gqatexgux.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gionfeffw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gosdaxdkq.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gplkiekvd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gdrvskeut.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gpvdicizu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gffphatkp.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gkymkdark.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gxoqccjzk.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gujgokylx.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gjesfvbsb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gsflvaunb.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/ggaolhjti.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/ghlkwttnr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gblkksymt.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/grkjanszo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gqvxxurzj.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gqrosmblh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gjefodzhv.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gppdsulsy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gkqmonzyw.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gkkztefdr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gqwqqwhvm.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gaouyiktu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gydqttmqs.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/grpxijlel.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxifjvnmb.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gwkbxvfrw.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gxazntiza.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gdlygpegm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/guzxewith.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gsolilhrs.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gpoqhmdvu.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gjrnoumzt.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gbankpvja.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/ghvdhuxcu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/grrhrvkfz.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gwfevrmdy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gmmcixnho.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gqsfoznbi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gutnmxdnf.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/glvnosrop.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gutlloocx.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gpjiojwom.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gpaqofjbk.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gkixochgs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/ggemolfkv.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gybypuphn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gxrbapsyl.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gwgfxqxcg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gdixfjlrq.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gljdvfxtg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gvrtxnksb.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gtvizgdyd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gkvllpkyw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gjesgrgal.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gbbvahsgb.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gazmgamcs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/goiepulmo.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gqsnjcggm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gfmihggsg.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gbvzcohwl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gmrplmehh.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/ggpotcjqn.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gvhteiuku.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/goqjqbzjg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gdzwudthx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gaeuforxx.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gmfwxngrs.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gntzutlps.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gihhlxafe.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gvhwiyizw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gqnlbpaij.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gfegukdko.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gplrnbsgf.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gbzwutdjv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gylpxxbee.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gqoffrpeo.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gkfhmskdx.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gghvcnbwn.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gopwwmquk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gxpjzawua.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gbznzlvmj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gueojcmqn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gthofumam.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gasgjdoot.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gunbnddey.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gvqegzysc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gfbjyguzp.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gytqkegaz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvdyqzkjl.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gjfjokmot.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gctsexuut.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gmvwkvpcg.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/ggzzlzetb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gtdagbtci.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gfrpojdnn.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/glteybsbb.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gysfeqxcs.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gjqjptirm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gplsvkxum.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/glzbupmjz.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gasnppesd.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gobfpxaek.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/glpnokmjk.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gqpencrin.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gzuglsdkh.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gyahrlunp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gumqdtgaz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gposwthmr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gdpldmkgy.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gyesddnek.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/grzodatjj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gpxzwhljm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gqcckqojb.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/ggibvyipc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gsvvqgypv.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gtvwawaio.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gjykbhtih.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gtzwysmfr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gskslrdie.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gatdzzutt.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gniulheny.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gzvuvspud.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gyumfbanr.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gowiyfyyj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gxkjowilz.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gufmczhaz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gpouvpeqa.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gqwfoongr.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gnjqushel.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gstimaaek.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gdislumbb.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gmcmgivmk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gtuagcnpg.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gptdlpvoj.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gmdhvhxdn.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gmbymakgb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gidhsaery.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gwhvexpsn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/grtaxfdgp.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gstphcpzx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gemubfcia.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gbcjcubkw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/ghuywhksz.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gkpkmfbsi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gshnbevgs.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/glvxxerrd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gexnkbhuo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/giqbtaqpe.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/golbqwejb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gplfcmadi.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gmxufyuyu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpcmoihvm.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnutrxwvs.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gpnmzkepv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gtszidvoq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gsplomxww.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gnqyvfxxy.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gebjitmyk.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/giyihxhas.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/grrxparut.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/goltoirvg.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gbxogepjb.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gjwittpvu.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gyniygnhj.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gidkwywss.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gdbbchieu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gxdgzthed.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gbjlefser.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gxcgpeysi.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/goxrhqyzb.sHtML


<!-- 参考信息 -->