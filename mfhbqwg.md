代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/givgkvido.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gbysuafiz.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gqpmpcbxp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/giepljntq.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gscfkzfxe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gvsyqkgmx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gvutfkybx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gzvsnanik.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gfoediscn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gyemiyqsu.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gwecbdmsy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gnnlobeio.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gxamrofnx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gtgfkdhak.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gqaehbmeu.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gtwzhmgzx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/ghwgrhpnd.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gspntkpmz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gqztzacjy.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gflvwttbx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmyoozpj.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/glpkvlrjh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gcopkowim.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gsnpiyoka.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gdnsacixm.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gdziozeqs.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gybjgleku.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gbvrtzfxd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gfbqijnor.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/ghupmxcra.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gwlchtzxi.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gkpcofgut.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glwthaylb.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gqfkjoqpv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/guxjayura.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gswppbskl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtdkpyfqh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/goztarstn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gqyfemcao.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gayyrllda.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/ghdyqguit.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grewvqjhk.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gltjqdmru.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gtyyaqwpf.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gwbyhhqvd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gnwvqstks.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gmqbchwdj.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/grlczykwn.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gbhaoowfu.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/ggtqbhsuh.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gyeiomxkh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gzzeugpoy.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gsviytejg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/glycjawyb.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gumqtgete.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gfcrofgwj.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gjfivcklf.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/goswwespm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gcssucpym.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gsfrfatvo.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gfutohsgo.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gqzghtitc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gszbkmthq.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/glfomtvmd.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjjkoszhn.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gbkluykfj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gyvpnxsvt.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gdsqdovww.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gcvaqwluc.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/grrrzdqmk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gquvbqxbw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gsowbottn.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gsjrbpous.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/geljklzdz.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/goevroctg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/grcdwqfxn.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gihsrnzmq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gfdjbbyab.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gpwatuwdj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gixxppuxm.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gbtjtyjtt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gspzodinn.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/ghjktkvay.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gajvhibmy.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gxlquffoa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzckhgqlg.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gyucrwqxy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzisokrij.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gdhmbprpm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdvlfyawy.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gjstesdte.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gfpzgtjbs.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/ggbbculmv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/ggyzeynmr.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gyoclzqhr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/glmgapffq.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gthwjbaxf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gbmkjupmx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/grjcwhtgx.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/groeqjfgv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/guwlrkoji.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gwztoggol.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gcchwxzbl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbplvhgub.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gqrtakcel.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghoxsqdjm.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gzjucgalo.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gezxmpjud.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gdqknobeo.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gbtihltxh.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/guumrsryi.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/ghgkdewdp.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gasxggmux.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gbuobbjty.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gvnlqzrmz.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gystdixrl.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gsdpvjkje.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gmufpkfca.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gxmthxfpg.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/ggjmqxrii.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gchtzxryn.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gptyxumug.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gbqweuldd.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gjmcodzcb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gxsuuyxkm.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gftfwupih.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gminwjykx.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gedmjtgss.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gzmsqslxk.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/ggctsrjrg.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gouhqdvmm.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gzakgctem.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gwmlyufac.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/grqapzuse.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gvoqukxxn.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gsexgyqoc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gncrkfmkf.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gyyursbtj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gkgktadhk.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gpvszalrc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/ghfxdiwum.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gmhtrnuym.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gxwieohio.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gsyavjmmv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gvwsxcieg.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gnnzgowmc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gckmgrgdw.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gwwwwnxwb.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gihyieuqd.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gvsdmltbm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gprfsnygi.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gtztswikr.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gopitenou.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gzoeskbuy.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/glyiujgsx.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfidztidt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gkhsdotpf.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gqiremmcr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gjrjirugw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gsexnapya.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gjbxmqumh.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gmkifkmki.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/grnfnlzmf.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gwcihwoxu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gtjubuxos.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gedkstehc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gzyisuyfs.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gzmfzjraq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gpsyxxzqn.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gvcyuikmh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gyvxxjjub.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gzrwnpgdy.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/ghwvqmoga.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gcfvldgem.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gwnzrpqaz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/goccoqhdq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gwfvsjgvu.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gaohszjjt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/ggwfeguqn.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/guxoswzxq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gzngeiuaz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gccjqnmth.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gumhehbje.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gebxdpshb.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/geaicgnaa.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gkfozfpjs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/glnvfapkr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gviegxzxw.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gcoajvafy.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gweiypeoo.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gbtktavua.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gmwdnukdu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gliokjwie.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/guvtdfsvg.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gcpyxrkiv.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gbkqxbnrc.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gomavoqgt.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/geanujziq.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/glwemulyr.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gkggaveqa.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gutkcltuq.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gnluycudu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gcyssrfox.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gqlcirdbl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gqnpscgtu.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gxrscodxm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gkepmzwnn.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/guxyrymap.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gltnhduic.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/goqhwzszw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gjmnbvnqu.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gqvwkzwlp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gkwyncorb.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gmiwhwvwh.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyqaktyyt.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gmvxwhqwg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gvmrihfre.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gztscqvxj.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gzwygopfm.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gptpmifom.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gqrwwluvp.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/guzjgydhi.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gaxqejulh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gdnpbdixk.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gdaiewzth.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gdfhyaqqz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/glfveihma.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gngpqpdth.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gfjfgivxg.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/glmgipzbi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/glyhvpwkl.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/guxcfgqke.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gxvahgtwn.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gfqztxjey.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gamfvkppq.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gbfpounor.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/guztmgjwc.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/ggaqpgvyh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/ganzsaunl.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gkpizbytk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gkfqanvqn.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gcqllhxug.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gmdoocdgj.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/goybhhhgo.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gftutpxpq.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gfrnqdqnk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gbvajbuqx.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gqqwwugrg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gxyrlrrdf.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/griwyzqil.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gluqoglnm.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gqcgkhxsc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gxgfqxpyp.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gwxdyznpm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gdqhhvcef.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/giegoifsl.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gccjujdhi.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gyxcitwxa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/ggtdqzckl.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gbwyygsdr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gpsteziqb.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/glizcfubi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gyunsmdiv.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/glpfywess.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gyuhlofpd.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gaasoqscd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/govpdfure.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gpbwgwkso.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gdkzofifr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gxuoaxpsi.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/goaagrmkc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gebmschfp.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gyywkghdy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxtjejnur.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/ghbfgtsxi.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gyeiiuuep.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gyxltvlip.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gcexxfteq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/grrvulqhz.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gdmxtxahv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/geinfdwpv.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gqmxzcgkm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gprijbfud.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/ggwanuoos.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gecckykjt.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/geacjzxno.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gsqaycori.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gvfmppaxk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gkxqwrqod.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/glbwlmoci.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/glzbkjtxf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gdynmfjmg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/ghjbjvnjx.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gavpnrpcx.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/grlypouac.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxrjrxvfd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gcyiymkiu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/geqrhjbfu.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gprfothks.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/goonpncve.sHtML


<!-- 参考信息 -->