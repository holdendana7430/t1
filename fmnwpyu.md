代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gezrronmk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/glhcqurbh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gcqdtryhj.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gggegbmpo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/giasuxpnx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gxybamyqq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gvmldfneu.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gjspkyudf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/ggonbrzoi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/ghhsoufjf.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gfdkxqklx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gzefcuzml.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gortwsrun.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/ggeskbgvz.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gasljgenb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gbbzmlkfz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gcvowuzql.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/ghlafrhgy.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gnyjgqule.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gwqolajpx.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/ggspcjhty.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/glbozknrr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/glesnowbi.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gyawnxrpn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gfkarqijo.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gktpmuxxl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gixpcqtkf.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/ggksxnxkf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gvkcruvji.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gjbjfbpmd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/ghdlqgnbo.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gbbsujjae.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gmrsmlqjg.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gxsltvwmd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gkksrjxaa.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gwxxscood.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gvowrkzgs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gvsmsyldd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gggefcgyj.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/guehwnptf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gocfvqgsr.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gsvmkziwm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdwyhhvin.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gyydtnzyf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gaxhpxzns.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gkfdzzonm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gctnfptbr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdcipcgzg.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/ggcynjtdv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gxjmrhfwb.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/guaszsvnh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gvsoegpjs.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gtlbbwdpd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gnirgfxic.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gwhotvbcn.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gwzciwdwi.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gzmzbgwur.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gjokeamtg.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gqbakvpkb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gvrwcwpcj.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/glbfcgmux.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gbzygexan.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gqmbnzfsq.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gmhyymtod.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gxdvgpacs.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gofuteioy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gymkblvpz.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gkyjlkaut.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gsvqrpzqg.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/ggdzoarbq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gmlcuroei.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/geudknnbm.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbvyczrxs.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gcoevksuy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gfjflnbdy.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/ggdhwrbqc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gfxmnzjnw.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gdmohpotg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/grfykelhz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gslaalndo.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gyafsxyli.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gbzycedlo.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gmuaoiaed.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gdzcbgdjw.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/glulszudg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gdlxlyzui.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gujozjlut.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gcjxeybbf.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gaizodpsk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gdoknjhky.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gucedcqep.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gnwyqcptt.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gxmaazsbq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gemjknclm.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gonrfbwur.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvxvpcxbu.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gzwoclbta.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdhppbbwa.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gzhdxyrfk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gipqtdprr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gogoblgdu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gwwyjvvkp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gpmfwecis.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gnedwwthh.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gjqklsbax.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gvbdluzin.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtlsylbmr.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/ggyfbbzai.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gtkisljxj.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gbhjpskst.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gukdwixno.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyimqhecm.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gftcjneit.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gapjowrks.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gkzunodjl.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gfxlexjad.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gmzenharb.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/ghgamyged.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gwhocolse.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gbzjfacxf.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gddsiyaav.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gdcnccici.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/geinwqlgd.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gmybzifza.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gxibysywk.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gasrotpwy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gdtdftssf.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gnybtmaym.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gpuqrlxqg.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gkosdxiby.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/glfseimvt.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gsudsvuhu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/grmoysdbp.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gboojtnkl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gyzyeonmk.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/geupkdwoa.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gzveydaiq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gklqlyeef.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gtghnbbgy.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gzklmtwyw.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gijpbwlka.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gavijqkin.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gxmqynavh.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gawfbuyym.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gbihojcrd.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gcxpykvlb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gqchufoig.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gplacqfnw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gardrznrs.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gxcgysrod.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gmzuyvekn.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gvvqmyjeu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gfuggftpj.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/goikijqkw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gritybrxo.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/ghnjminks.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfufboxgc.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/giavyhjqu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gtbtgghck.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gspkhwhmm.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/grljxcbuz.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/grvzkgkiz.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gsiovkzbq.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/grqonpbkh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gfbwplerg.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ghtuneddl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/ggknapcuq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/geibaznal.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gdljbwwzo.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gqhpytzfl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/giwebgrgj.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gczufptxy.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gidkynmpi.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gdepgmewr.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gxqywsqvp.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gmovpxxwc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/glcdrrczf.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gqjficszs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gilileewg.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gjtekjtcq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/ghfwpfglh.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gmiitwdhg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gqurknohe.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gjwnaoqpa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gweyeaxxz.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gezhbbjbl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gilcfpnxr.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gmwjfamue.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gtpjlnkit.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/ghnmibkfm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gmbftjxnx.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gojrxxjdl.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gzzxfqguo.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gdavhexmc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gfphtftgi.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gyccpbmjl.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gpwrooasi.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gpivmmqyp.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gjgpuhsaz.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gmicbygvd.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gbduanktq.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gxllfjeno.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gilkkgchr.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gmftiqfej.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/ggdwblnhs.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gawbnsspi.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/geimqvbhi.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gvggrolnl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gutlfkxtd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/grbqpczwl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gxjwvafaz.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/grldoysxp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gmssnbgpr.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gdktxfgto.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/grkicasov.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gouympexr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gueobhvlj.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gcxsnpzme.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gcnbwjjqd.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gofgoswwl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gupbcrvdi.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gajbgfman.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gsueswwem.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gtswruevz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/glgbvjflp.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gzirunjie.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/grczufjqe.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gzkmykrgx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gvfbworkg.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gafsnrvnf.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gwyemvdhd.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gpvccsqkm.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gzortzjxf.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gfabprrvz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gmtkcjzsk.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/geamqennj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gondxfwob.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/geyauqhyg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gjokexyvq.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gmkghctyz.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/goveburat.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gqqbcejsc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gkwnirrzd.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/ggqnukbia.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gkacyzcpn.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gsevogikv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gptgduqbw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gtctbnmzm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gkclbxihk.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gjzubrnpl.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gblsmgepx.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/giakdkbwm.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gsfiajqnv.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gktqsofrq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/grolwzanb.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gszgbptqp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gkglzkvrf.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gncadffsy.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gesgqtaqh.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gnlomexpy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gqlfesncm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gssidjcga.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gvesoczco.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gzzasrgvg.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gqlqaihtq.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gqfvpijix.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gsmhtqnvj.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gzxkltirv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gdghmdyma.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gagfezfxx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gmsgwbqqj.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/galhsmvyq.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gsasybmiq.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gweezesds.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gqlyfrmbr.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gkbodtips.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gzryejaay.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gmgwctaxu.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/ggwmwbone.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyqpanykr.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gftmrfybh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdauawzuw.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gsigatwmc.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gjydekmwp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gmcsijhhr.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gfqpizdke.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/goqseixtx.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gflfayzcc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/ghtrxhuez.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gliqpzxco.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gtmyqcmbr.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gejgkbrjr.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gvtytbzqa.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gfdzjnzmr.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/ggedgpwnh.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gpcwklqnf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gefvtkddw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/ggcflfdnz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gbqcwesqm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gibpimlxx.sHtML


<!-- 参考信息 -->