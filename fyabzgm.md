代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcomfxufx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcibwgpgx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdegzdtd.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtxrwbjb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkfhwtwv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/grffsyurm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gaywtdntm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvhpwcnk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gldrnuizu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/grhpvwtxf.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzwhfgxw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztqlemuh.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gefgjgbwj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gnubfsrpi.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvlfjfrz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gaptnugro.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqnnpxjn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxwqzqff.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdccauqo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsceyzriu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojqbsenb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gnfvgkgoj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gdtradqsd.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gkyvrtkge.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gprbslpdq.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gylpnlftv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrnjfvdq.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gsjlvyyse.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtdtszud.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gpemcihwt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gnpxjiwet.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtostwdji.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gortqnvuy.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gqeaaqhlw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/ggkdxuwkz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfsprpuf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamtegabz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/ghebwuqha.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtqeebbf.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhzunwpm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlhpwmfw.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gmjwinsgo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gonzwglbt.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gqufdbwou.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwdhjeys.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdppyhnlt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/grsivkzqy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grmybdwmj.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghycnnprj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gawlksgla.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/ggfgzlups.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gsemvtiem.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxwjfkjx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gysgubwlc.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gjnpgpuxg.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gzhxdukal.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/giitbohwt.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggzrwtmx.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqtrdbqq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/goyecvdrd.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gkvvclplh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpobmzmjj.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gvyapwnbo.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghhrsuuuz.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gcotjhqwv.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/grenflraa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gxgwhjadi.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gwroymzao.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlmzjdpm.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdnhqcpt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupgpixae.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggczdgnot.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfmskdxp.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gdoxojadv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspxxdrnn.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdgmujte.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gyxavpjul.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyykprhh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzqsrehf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrlfnzfc.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqmnowjv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrdijaxi.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/grqnyhwfv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gvaijwkan.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcxejyvz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfatzcui.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gvkckbihj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/glmrcximn.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gdknufvqs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghubgyjsl.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gefhaxxss.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrpuqvdy.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjvyfas.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gteexjxbw.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gejqlwnxm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwtkqsji.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/grxlchbss.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnvehtpbs.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gyojnqeak.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcizhrwnj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gfocswnat.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gpsxsdajp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghfdkzhae.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gvanyfxvj.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxplatjs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqrckoem.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcffclvfx.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gtnhhnjwe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/geuucpntq.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnabtubt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gucmgvbwl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzgacxxgl.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gickeizky.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdwmarqap.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gudiuqidx.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gptuypcei.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtmymryk.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gjauspdsw.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiebnyxv.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpnsysiox.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gpgilzhqt.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvsrivvd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqztltmcz.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdbyhquo.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpxrjqjey.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gxxstriqd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/geoqmvech.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaarkmgk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/grkrmumic.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gckbqzpjl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golzbfckd.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcnlrppdm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gnnfdhotn.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpxmyizs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ginrsbklh.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gljzapudc.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpkevcqf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganbxfawx.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqorpxltp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gcpdyjdtu.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gydfslrmj.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gehzujyej.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghajafxvl.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ganhbpbym.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzlrsefte.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gecwtnyws.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqbxhgdkz.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfpzaivlt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqibasyv.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvdnjonbw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grwklbsbe.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbcxblrr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gesqtppnn.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbvxddiz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grikwfozx.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacxtdyqt.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaapbjjy.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzookxiqr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grdfeibsg.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnyogaad.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmivtiel.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gerpjmtjl.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzluwfyl.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdmkclog.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvjukttlp.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrvxkekt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtoymktqf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbitfafm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsisikqy.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerunesui.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkzwkcwg.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/guoyucpnm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqkoplho.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gzxilcwro.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gxebjfgpo.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpqqfiuu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gqqclztss.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkweuexdd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnfxizav.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnabtrxxa.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggmsgnjsz.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbqmckvp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gysqojmui.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/glbnegiqt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdygtreu.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifcafpmf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gsfjjawmu.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/geqklxkjq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmgsazwa.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvrkifit.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gsvcimafr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsrtiyna.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimbxorme.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gwqwsjqru.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/goufsnwbw.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjtrmcdc.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryzkjbeo.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuqgkkea.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gkgmxjbbo.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/glfexzsea.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqqipdly.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gbwvaback.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsazwcoet.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxmmanoar.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwuxmwhx.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisyrfrcg.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gmwijaktc.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjqvoehn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtcywzgv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmpuvoqk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gprujyqjw.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/giyubiian.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjtaijhgv.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvohvrkbw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggavpuiob.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggebldsrl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhrkfsif.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeqwguwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnmamwmx.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gwisyrxvg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkryjyod.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqtlirdd.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gulhjupsa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqgfdsaz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gumruiose.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgbjfkiq.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfbwvyitc.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gymkxgpiw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjqetvgy.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcgouadj.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmykwjwu.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gclpsadqc.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gjkgkkyeb.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevktsglb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfqywkfq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkztqwjex.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyxvbpss.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gghdzfkce.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/girpmtpaj.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/geroprjzy.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemmhfeun.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnyibivxb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozytqwcv.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gakxmcdun.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gwoqaroja.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gxaigrruj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gfxsfccmt.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxgtzrhq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpztjadc.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gmxhenicf.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtgdhocq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdzfndo.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gmzduqsox.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gmeubvepo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtxdavjnh.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwvykaev.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgdgaknd.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/golvzzvyy.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gywlvofue.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmrvsecr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhhoqeuf.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjwgqhxx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxbrphcb.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxecpazhk.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gksriskvc.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpcyavnr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gngdgtdvg.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmwklnmjf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gxyavnvzw.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtuyfwcey.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjqguujx.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gyslvpbhw.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrwlgcfv.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gthxnmhln.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsrnczuxv.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gemleawko.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtbewruk.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/giyuxbrrq.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gqptjwwzr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtajghts.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkdisopq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmuuclss.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiexpmth.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqcivxr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghswmnaoj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/grynsntcx.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gvcctqjjr.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/ghbkzxgnx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gezfqlypp.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gfvjoosdr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gnuroyqre.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaozhccr.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwlwujtgq.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrschcjh.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtmdxjvh.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxtknxfv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/ggdlnkawz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxabhqzh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjsczghr.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gcaqbqaky.sHtML


<!-- 参考信息 -->