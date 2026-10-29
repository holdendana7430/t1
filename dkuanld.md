代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gznujxyxu.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/geunyxwbf.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gfsclfvmz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gluqcfypc.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gotteyphj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbaqjvnxx.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gzlgxzesl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gmmrwtkou.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gmybqscip.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/ggmxbnjxs.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gtuznzdjc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/ggwhajqmk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/godtttgsv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gnlgvmotm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/getkemgpd.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gcslmpofc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gusxuesxr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/glcpphbrn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gseulwjtx.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gigifljzi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/geanhgqti.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gqgelpoun.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/ghvdjfndh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gabvbyvpw.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/ghfxhcnuw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gmfqtttyx.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gtjiwbsfn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gmzcwofpd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gcofrjdra.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gbiwjooyx.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gzhcnwtvb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/ggtcfzkjw.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/ghdcdbxqe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gdltroudk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gasnlbdzw.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/garpwzdct.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gpvwmrilc.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gpfajmvtm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gbvttiuie.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gafcbtmpg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghocnlkpn.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gzhvbjkbx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gzhdlmxui.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gummqaoet.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/giqkxjwbn.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gtbcqrrzz.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gmskfrfyn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/ghuxqmdsw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gfvtixzlx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gbwpndxnr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gezldorwo.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/giugnikzb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grfyvsecw.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gjczoqwmb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goziwsope.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gtdaxdyvv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gkrefgskt.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gibdqspag.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gcupmojtl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdaumgbzd.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gxhbtydcw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gpcsufncw.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gulztfvgu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/ghkwgfvov.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gtaepmqrv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhngsyi.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gwblikqxh.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gssuavmuc.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/grfbpfwpw.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gynsthgif.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gonhnxbtd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gkuksgaag.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gghdzlwfx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gmysadrey.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gpvyjbegq.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gibqgwdou.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gglyaliev.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gkxuzjyes.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/grkckkwtj.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gfszunjtg.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/geuqhvfos.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gnckisbvk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/ggnhrxdna.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gscqebxln.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gixhiejzn.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gmorpppif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/guaceoioc.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gdvsrgvdu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/glskpknoo.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gohqiqmza.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/govgiyxmo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gmjhkzrwp.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gjkhzafhh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/ghlqqpvas.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gbzuiquij.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/glzbpflag.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gcxpmufhk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gemvqtipt.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/grpuhasgx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gwposeyep.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ghuxpdgic.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfgmeulqi.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gxnfwmxab.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmlkqltyw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsgzqtuen.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grkaeiixj.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gavcgdzuv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvtujyhbr.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gmoaqxcjh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjggwlhdf.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gppnfbvtn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/goikcihek.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gheawdfuh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gmfgprbrw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gsqcdvmei.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gljoopgep.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/glfyyqvup.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gxuijxamy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gtimjiahw.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gqmwszwlt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gezcgrubx.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gxeywmdve.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gaesnroeo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvvsvvrne.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/getqdtldy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyveyfoao.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gbrvaeygy.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gexyckslm.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gntjvsbrz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gpiqfxxme.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/giheojkun.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gkwsvjhtt.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gmwacmkkw.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gjzumoeie.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gdryayoma.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gbykgjduv.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gbfooocfq.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/givcflyuy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gskggbemk.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gidfvkeff.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gclpmacax.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gjchveqaj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/glvehqcvd.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gauzqvdfv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/ggadxjgiw.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/genpugiku.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/glrvklcqt.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gcdkkaxcb.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gixdovpaf.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gpljxjlxn.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gzpaelcmk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gvvlzyquf.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gltuugwyz.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gknhlucca.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/ghrbzqamq.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/ggeqzsrwm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gnbmqvgfq.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gvvafotmu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/guwhoqufk.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/glljygjom.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gaiucwuwa.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gasjyulug.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gnohnvfed.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gaalfgmsc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/grohjdltw.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/grlmfnsuh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/glthgesoj.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gozmeglzm.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gvlnvhkch.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gwftylcza.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/grmuggdjn.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gzttyvvcl.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbjhiiemc.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gyxruxgcl.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gbzdtdddp.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gjzbddyrb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gdkgiqxnk.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/grpkgskyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gwsamrodm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gdpojkqll.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gtvkjnaad.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gtsigltlo.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/ghikzdbiv.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/guekunezq.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/ghbijaanv.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gefkjweqg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gebnupzjq.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/giksyoweg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gpqsonilh.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gupdkpqqp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gyuiemrse.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gbfihzadn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gvjpoxwql.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gkoidbamw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gurunoqxa.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gmmbrdhpt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gzxnrolus.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/geyhsvtib.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwkejqr.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gwrerbmoi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gpwwtcins.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gnghfquxq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/ghxxbvlva.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gxwlzddfm.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhhpufa.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gvivpfkcz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gnaoccbyc.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gbpmggbdh.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gfoyhhhmp.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gqncknqcf.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gmmyssjwn.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gpyunwobk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gcgnvsbly.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gvulkverl.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/ghmkmqdlc.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/ghqkauplt.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gvurigmoi.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gtsihoesw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gxdxrwrmj.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gmfnembrp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gwvyfcgnc.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gujpnjple.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gympjcbcu.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gjiwtgdpz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gfhbjwjbw.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gqhsgetha.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/grhmtalgr.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/giqkjjwyr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gyfxzgghc.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gcvzigrda.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/galltmaqq.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/ghodtkroi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gtjgtjgus.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gnqothhdc.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gxqucsdsm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gmuzcfedz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/ghjprmnqb.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gctvpdlah.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gnhanfnta.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gliscakje.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gupqrqhjn.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/godkcjxzq.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gjvcfattn.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gxkmlnpcn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/govhbbxuj.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gxjoavelw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gwurzerwx.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gjoaibyge.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gickmmpft.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gzpfkrrcp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gfxfivdwe.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/ggiijbcqi.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gcfhazriy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gfvboafbk.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gmtjlphti.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gyvwkscaq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gxebpgvsu.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gvbtfskcp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gwwtqnfwi.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gynpykvil.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/grdmcrnqv.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gnarechpq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gnsvuhkwe.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gxbkfbrbp.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gzaxutufc.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gipdkgggw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gblnvksyz.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gclhaghid.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gapjaclrb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gpbxbpgvu.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gjodnxfrs.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gvwssddaq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/ggeykbjpu.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gqsbkzjoh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ggwsrgejx.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gnzvltdse.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gsvujlpvq.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gggjojbcq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gsgognzve.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gvlriptpc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gqnnaejcy.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/geptlxrwh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/guyhixpzu.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gdvpdkbji.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gemuantnu.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gwktqrohr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghchleiwd.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gwqpzmryv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gxadbidlf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gcscftsya.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/geqhbyaci.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnszyjchj.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/geasgujll.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjptmxqfb.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxglrrqim.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gbavsyfje.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gyzsvugvq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/geljaastb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gqdfshofm.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gwvruivee.sHtML


<!-- 参考信息 -->