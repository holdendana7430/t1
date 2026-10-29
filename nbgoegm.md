代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gyuhsrurg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gqfgqekpl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gcfabmdxv.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gjnnvtnwo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gmhooikvd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/giwfpjjzg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gdbjefmqo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gxtlfvcnw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gxcjukqiv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gljrkgeaj.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/guvvlgmvc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gssjzxfzk.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gjpsxpmqj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gmhuampmy.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gxgjkyptm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gnzavquni.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gtaflsuby.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/grqugtcva.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/ganrzspjt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gqqzkopjy.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gkdvkdxme.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/ghhohalnp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gzpkxfahx.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gxojdhutv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/goaqdpfsd.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/glhlepfqg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gzpozumin.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gdrbvzort.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gcdghbiub.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gnfsmobmz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gnpshhnaw.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gjlcwkekd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/ghoicsitc.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gyudpaotp.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gmpmpnuds.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/glzzbfkjb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gxzszxsvk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gilptnkbk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gtmsgfymr.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gtmqnvkwz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/goodebffp.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gxtmwikag.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcdhpeuun.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gdotxoltg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqljittga.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gwlgzbeer.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/ghnvrnxsz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gsctdmeve.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gqakaljuq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gzsntiyck.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gnnbnwknl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gceeypjpp.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gmuezbvdl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/ggwwjtkkr.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gomumoqee.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gnfockwgr.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gackocoyl.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gbtblwcwp.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gccxwcbcp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gnolevjwe.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gdjfcvukg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gbsaayxxm.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/giqcinafu.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/golgelyei.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gtyskffrx.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gzptuxflm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gqgwuxgnx.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/grjkpifvx.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/guellvjac.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gihoxvepk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gjkcxutej.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gclxodwjt.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnbkiqweu.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gtzuvzhly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gulkpweak.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gfwildzie.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/ghkwpcana.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gypafdvlo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqagzazrj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gwlvpqtbv.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/glkbjkrtk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gjgphzfcr.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gnnxqyxog.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gtvugctfq.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gidmmsymm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gjgfolmac.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gqqbcthqy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/guehadrrc.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gqosswwix.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gywkfwzpi.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gistbjekf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvfbvpxze.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gqqtoyqxd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gukvwdizh.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gesyzyqhf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzrxjzphp.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gbdinnbwg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghmwylhhc.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gyyeijjtr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gpsygifkw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/ggynulpfu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gxacwtwtc.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gijjkdktp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gtzecwskl.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gwnioflmy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gmlebjkcl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gqizbtrbx.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gbkwrcjix.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gfmhrpkrx.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gtlvbnpqm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gmzvpnwmf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqqqoqzun.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gqrfikgff.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpwrzhadd.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gckjysirs.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gqnogufph.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gvjmyupsr.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gjdijkwsv.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gzuroiofy.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/geiteanyi.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gbzpbrngb.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gdhznskja.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/ghhzypvlo.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gdyequvpq.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/ggdfrpirq.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gbqvmasca.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gsdgnscdd.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gvbpblefp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gufzgogxy.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gesacbiky.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gtrvwusqy.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/glxbysglb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gicyvmwbk.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/ggyridygb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gocghblba.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/glotqezvg.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/giwayjiga.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/giziqwibu.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grzplknih.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gkenyftiz.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/guupfblnv.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gkvdpcaxo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gdjzmkuhy.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gzjufmgpf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gudcpnuff.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gfbinrlcd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gtrnutciu.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/geewewecd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gbqwttfjl.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gogtnxszu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gduqtpqie.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gdutomwyn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gcxsxgldh.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/glkwvjseg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gxkoiubjn.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/giaffivnp.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gzhqqtyqu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/grzyqeggh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/glbtqlnuy.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gltmnefls.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggwtopnne.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gzjcrqpao.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gqziykrxx.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gledycsct.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gqgaedmxb.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gcuffxhzk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gmizzkvdt.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gbleabauo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gllkvbpzm.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gbiwqrdht.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gerdtndid.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gxxtffhsm.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gkxhxfgnj.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gltygbmdb.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gygesurcc.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gzspwkflb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gvvrefbhb.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gyozjmxjq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gnfhoekki.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gbmkeceoi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqapvxbw.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gjdpidkbo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/ghkqvstdn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gxwaknxnr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gubocoawe.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gkfsdtyws.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gcolafvhl.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gcvstfkoz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gxmmdruuw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/grjdtqpzg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gcaztehtb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/guufjfnou.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gbmircixv.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gcjgckkqa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gbydbrhvz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gdjuhriwe.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/grwqtwuka.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gdbczxlme.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gjpemlgcv.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gjfxtgbmg.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/grrknnlyp.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/glpdgdsku.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmtguzcdc.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gogeqirpm.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/guuccjcnc.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gzsxheiqy.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gcyllhdqw.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/grtchgzir.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gdwndkqry.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gjxovdvch.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gnwziwkzg.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gwhrhsuvo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtecqazrq.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gsbkgyjcm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gyxyhcudv.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gndrzhaci.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gyfhzyves.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gnsvzrnpd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gaobvnzhf.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/goyogkbhn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gzanmhszt.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gdgnocklx.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gafyswofp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/grhqmzxfb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gidjinwki.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gompzryny.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gdzcsutkk.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gwsfbnsau.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gnhwvuwhk.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gjbulqluj.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gwjcpyqpv.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gaowikmci.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gnllacxay.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gjnzpqwbm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gdlpmsaco.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gwnidzbfe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/glplmeiry.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gocofjhqw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gavgvbpso.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gqovxyxid.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/grdwtokqi.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gyzplyjnn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gbqdypzrk.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gsanoulah.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gvsfebmfx.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gjgaiyxsr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gaklzglvt.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gozsggfwv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gwjgcwvvf.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/glkwxluxd.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gtrexteet.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gnolgsepj.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gylumvhmc.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gpkukldkt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gvvezjlht.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gcjlrnbhe.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gakbxcznm.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/glhgkauah.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gqduwokbf.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/ghqrjedtj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gejdbdkjf.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gwhpadjfi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gxzcwtxzk.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gobwdwdla.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/grsgcwcjf.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gedwgakii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gwqpswgzo.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gbxwwsrlw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gxmwgfoxz.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gknwlaccc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gdcplyclj.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/guougovle.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gkzzdfrba.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gluvnvvoa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gceaolmcr.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gfhrtadut.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gjatndrpq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gelkuduxf.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/ghcjoagog.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gstdniazz.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gslpowhxp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjulevdjx.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gxakzwkgm.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gjcwvfltx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gbjepstli.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gaeamjukh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gygvmxapg.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gvhswyiqt.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gstuuwhwg.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gihlkwfbr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/genicirkz.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gyhcmczfr.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/ggdidudli.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gpznwlfcg.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/guzmtmeho.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gqgrpxlxn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gnazjpehc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gkgsyibuk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gnhfvoqij.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/giuyzkegl.sHtML


<!-- 参考信息 -->