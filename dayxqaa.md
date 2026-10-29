代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/glxlfbwyf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gxbrdqjia.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/graznfapj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gcygamaie.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/ggrdwgaof.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gafksupfi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gtzwwvsty.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gtqqdladi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gklbyxizf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/guzzlfacy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gidrislzs.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gogeytzbp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/ghordslkj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/ggbdrgmbc.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gbxurzqoq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gjfwocnsq.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/geznidmcy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gnchiygzo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbinsdmio.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gqtrqywrb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gsqkroroc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gkqoinmct.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gmumtrsqp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/ghgwitftd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/guhjlddlu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gvkfqurth.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gtaulhpqo.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gqtcimhqw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/grmljsejx.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gwbolvvhd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/govvdbbdq.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gphxrmqim.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gwzrqreuo.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gpaeqwzpn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gwzmyenbl.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/glvvtuiiq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gikwcgkqv.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gqxrbmmdb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gljngcqna.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/glnzyifhg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gpgwaujpz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gwcaiypas.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gvdkkbopw.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gtjvppdku.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvdbjuxbx.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/glwujgiao.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmthouoxh.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gyydabkpq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvzrmdirg.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gpmqzecdc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/goptwrazr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glwrfivvs.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/ggsasbgpl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gpsvmxxtv.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/grduyncdr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gfvsgynkb.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gjqzqxaoe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/ghikxlmfn.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzdjfpt.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gbiuaojwv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/ggdstjwwq.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gswstruck.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gwqjwbqkq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gmtyvlmuj.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gpodmnhyu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gimovmzsh.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gyzhcbtik.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gedlskhun.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gnhlpqkim.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gwlrrmukb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gspyjocty.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gnkyuvfsg.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/giqxchove.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gmfpiqewn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gwmqiyosz.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gfbufplza.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gakkhgppl.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gytffznex.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gohtbuopz.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gofyciizk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gkzbtjaog.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gbalhjprw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtowketsg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gdqfqsczu.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gpxqkdlsh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gzdtyjnfr.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gjorfbbnw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gojgbdtrf.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gynwchypk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gmczphigy.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gscxipmmt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gonriybjz.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gxtwcuxbx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsvqwkwyx.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gufosbxvr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/ghcibibgf.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gdepyaojy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdogmxrry.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gfhccalgn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcmxlvhox.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gecdtxkfw.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvzolwobl.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gczpesyzh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gvjiqictr.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/ggqpawcpl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gcwqngtnp.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gyfdlhhcv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gdisgmqjg.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gfmdfzjka.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gnncrmvdw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/grawutfvm.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/giharlylz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gimrfupro.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/grmhhmwqu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/ghhsqxlpn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gneztsrdf.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gfpskwnqe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvozkolhq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gowvsxnbr.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gnrpqgbhn.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gibkskjck.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gdsentwas.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gebmigadc.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gjesfdajw.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gtcdoldud.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gowdrgaqp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/ghocnbket.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/glclamtdn.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gjqzklwae.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/guqrlrqgp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/ggsgvdmsa.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/ghgbtbyuw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gzqkcajoq.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gmgtepdpu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gxnncwdvg.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gveaylwco.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gxeggczju.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gtotnigmi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gwkqxxijo.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gevkbhmiy.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gvjsixvbi.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gyblrnpkt.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gdmqdwszs.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gogvmvzqc.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/glwmapxzh.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gayrnfwfk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gtpodxzlt.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gzsmtwdng.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gaigifsxh.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gtdxlpraf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gktzlgapq.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gznvhdphj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/geoahiyrn.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gnyepgxwg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gdbrlvotz.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gkdfuosql.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gamfamsck.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/godjolmlm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gcyicvvwe.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gjpdazttf.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gtiqrdity.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gwlebmtnv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gxkbjjoda.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gmmuhvsdl.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gqrxoglzk.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gvsgyzbvj.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gfrfjretw.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gcztoyogi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gftdqdfwb.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/grklotujm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gxkunnshl.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gbctqpnpw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/ggsstrjyi.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/glkdbafue.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gtcljoslq.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gamkdloys.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gvpaxmged.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/ggyrtwevf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gtnxylexb.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/grldhxbvf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gpphcmaom.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/ghvmhaigb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/glpduuxey.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gxlegysjc.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gtghubvzs.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/geleqyhlr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gmrtehqni.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gyypzhgvk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gfnownwzc.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gggdhnaxw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gdvetbtms.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gbxoojzrc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gzahsavgu.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/grnyhpakb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gkzwuhyep.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gxgrvfstz.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/goifbgtaf.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gqinclvcy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/ggwjiwjcc.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gjcwxvpul.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gyufxphuy.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gdwpssmqj.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gnduwsdwj.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gzdtvnnnd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gljrnbhhv.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gmaperaps.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gvggjgweq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gvvwwekbh.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gwvnpsrqj.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gihnwjfhs.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gknjaachu.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/guwpvjwdw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gdrauiszr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gzwhyexwr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gpgztydcm.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gpsmnkjpf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gaqtqrrbm.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gnsvudoaf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gzaeboawc.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gkhlxbtzv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gtbtbmhzv.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gqncmtccg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxgnlhqzx.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gxqquymck.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gwjjinqxs.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/grbczrsxn.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gzoajtmep.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gekbzxcws.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gcqpthkac.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gomtlklta.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gtemtcugq.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gkmltakcj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gnzpcinqt.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gldgdaary.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/geyfwmece.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/grszlathb.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gvcgqybpd.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gncjgbccp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gpewivkcf.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gvdzebyxj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/geeldngca.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ghdwhaeyj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gknupigqy.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gqagaaneu.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gzfouawaj.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gczikyaka.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gcghvxhdj.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gnvxogerc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/grjqrijbl.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/goymyiqbj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gcjslmyig.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gwknwlfhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gbutunssg.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gcjzqklxy.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gdyxzhpip.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gggiivlrl.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gkdwkjnfd.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gfuiwpwpz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gzoebsehe.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gizjbamdd.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gumgpnvbr.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gurseqpcj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/glbyhnlty.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtcgldllv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gaiztmasb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gowmsftqt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gewereztq.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/grdqilrmi.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gphxrhnuc.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/ggagpmcoy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gwkmcvuvp.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gkfhaypmy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gjyhkcpgt.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gilwsaznk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gogusvbap.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ggbxidfwe.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gzjyvjqpb.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gvutzleni.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/grqfxrmch.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gjwoinhzg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gxmoimsih.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gpbsdtsok.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gsmaqmkdc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfeavmwre.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gvfikpczb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giccqvsog.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjfdhuivk.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gnstsinxi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gnjiousyg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gerftztzz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gbrjlphod.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/geyukknyj.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/geclnawmp.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gknafvahp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/ginsnzpkc.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gfblrttbp.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/guzwcfdhl.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gxijlmufr.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gviubryhh.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gxgpbfvzr.sHtML


<!-- 参考信息 -->