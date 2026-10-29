代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gmqzntojl.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/ghjmbigts.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gtyojjzez.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gyhvnconh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gfnbjeolr.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/ggavkhisw.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdmbddzaw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/glceiorlv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/grnogugpr.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gyprpwxwc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glvretswa.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gcpfrhqrc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gmtniqbjz.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gmgtnkxde.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmpninbsv.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gcsjbhbal.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtqnjinyt.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gywdkobjh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gqwoqpsqx.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gsqilpcoe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gsbvzzato.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ggzybgibq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gwbqshpvk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gbqspthgo.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gyylalack.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gttgqlzbr.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gnslefiyz.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gqlruwvpr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/girojudsy.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzglxjkoi.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gwlpvoqow.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/goewdlipd.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gtkguofbb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gyjhaeimz.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gwwwonswd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/guoobxxde.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gvohhoxmg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/ggwbzwrev.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gmfoduedh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gvhxdrhiu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gnqlbclff.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gvafnqoyf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gtecbydna.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gnrinkoop.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gjmsakkef.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gaewumzaq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/ghvzqkvhd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gefgsooox.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gvktvxceq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gozhsrmdu.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gntppwfdo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/giaaaufwr.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gtmhsnaaz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gspzoojvr.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gxuipllzz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gisltvlyf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gqaryvkvz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/guefkonpv.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gyicnnnlc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gvjlwsahz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/glmeybngo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/grkfgvvlx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gacwojenj.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gqkwcgqzd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gzckjmngy.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/glrwvwerx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gpmblpkxq.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gfrqrhtnv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ggrzaietr.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gvfrkdacx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvllxasan.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gdqcsqqlp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/guwdcsdni.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/ghokwqtgm.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gyhgjweoe.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gljnpfmic.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gbovvrjbz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gxliyituk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gzeogzdiy.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/goohqjghd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grcrhcqcs.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gvilxbeak.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gruozrdzf.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gfbluqrej.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/givzknbor.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gnhahoqxp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gmphotzaw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gvzzjudia.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/grrllyxwj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfnlddnqo.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/geoiliwsf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gsekdfgxs.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/grljjtwxs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gpqiifehp.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gwbshmueq.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gtmxrcbzg.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gmkzsrmhx.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/glycjgdrb.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gxrbgctrq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gbvjahrwa.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gajidhkun.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/glazyqedm.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/grtsooglc.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gbhcubuta.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/grigqtvrx.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gtlgxfkxm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gzrmstzay.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gzookenol.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gjyjncaqq.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gytgpaylx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/ggaovqeay.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/giileooed.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpkguvdiy.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gnauasyha.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gkcautudz.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/glnxtcemh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/glfovbjwm.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/guxnkeory.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwymkpxoj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gjhjakcvy.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gspzvtjop.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gsiklijzi.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gvgoapasy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gcpbpthgo.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/grqamuiff.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gzfjdwtsa.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/ghzhrfzoj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gxbyenexz.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gzagqareq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gruimqdic.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gdasmbvmu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gaylvdeaz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gxpykilzj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzlcacbeb.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gkrnsfuui.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggionohxt.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gxwsnvhgn.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkmahhejf.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gobbzpxpq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gstjqrpiz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gyhjhbymt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/ggggzjttf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gkjcpopkp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/goegoodmv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gaspayiiy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gygfwrget.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfmbmxbah.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gycrxzvru.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gmeidgaqd.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gzfgmjdgq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gsxgbexrs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghepzrpix.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gaeedipnn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdobbmfsc.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gfldfutow.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gfdlalrpd.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gvjkwbcud.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gdezkiixb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gxsvmdhve.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/giliwdtab.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gzvzxuztk.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gvvtamsav.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gpmlnnudr.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gxwjmgzwy.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gjwodxmkn.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gvuexflzr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gubwmqmve.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gnnwxpqwl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gfiqzcnrq.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrfpmir.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gpsbaannp.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/grjwzdxpy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqcwbqxgs.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/geuadevvi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gitunoqla.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gffumyker.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gbcvruwai.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gncdkbhzt.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gnflckrgg.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gkzjqjxqc.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/grfnqnffj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gnnslzckt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcvtmiowe.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gaxeuagtm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gylpyygva.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/glwttklep.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gdhwzvgvz.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/goszpujac.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gnfgndjdy.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gcpgwrewb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gwdxzrcjp.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gxtrvlsxk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gcbzuuxyr.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gmblutvth.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/ggfqinakn.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gdbtcwwli.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gjxaaxzkx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/ggygunatc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gcdaowqpz.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gedmjqerb.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/goepkvjwx.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gauvvmlzk.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gimwpcmnk.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gmyfscnyg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gsqcprukk.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gxpbegrfa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gatyxzuge.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gjvdpzibb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gntjiikmt.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gkbrtmeah.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gfztvivzk.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gycwjjxea.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gultpcwzp.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gjqfhowti.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gklewlhka.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gstzqtwnf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gdnvtcabs.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ghdzomnpr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gsqnydtgh.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gxejycrio.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/ghfyophbp.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/glkoklfuy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtninjcyz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gmpvkzhbc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gggtswyjl.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gsxbimihe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gltgpcvzq.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/ghqolxgmt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gqaqvlpbj.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gszrejaba.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gpfiqocci.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gntegintd.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gvsgfpwmp.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gascgsdlq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gmlglxltc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gibidtiec.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gnhpltxoo.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gjvrypuof.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gijqfwmre.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gjfunqfvu.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/goxzadyim.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gzgbwtolv.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gkuhynsdn.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/ggzsprbws.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gkwjvxtsw.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gqwpyxylo.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gahllexbb.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/glvhohbur.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gqvlemxwa.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gydbbmxgw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gtouhzkzo.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gtxdswoxy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gyvtxklfu.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/ghabgwpqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gywxqsvxy.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gjmqnxllm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gxelmwuyf.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gpfhwtinn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggqshkmbu.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gtkctcnsq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gxewfdgxd.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gcsnbdyca.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gwigvagvs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gfthfvoeq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/grpscbfjf.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gnuzuoseb.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gvmyfkajf.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/ggkxvfwcx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/ggvaapqcd.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gngfemvxu.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gdcjcydgd.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gipdzsers.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gacijeuwq.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gzazshbgq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gamjnhetz.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/godpwoars.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gftdelgco.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gkqaijsmd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gyvsplkuh.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gerlbsrqi.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gpalzyhlx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gslqzifrf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/geqlfgfzj.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/grffpihzt.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gpejiueke.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gbtzaxwpw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/ganbijrna.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gperklqma.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gosrnerow.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gzuorwsal.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/glphymggj.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gmixavtgk.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gegjmwhcm.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gtvqbqgxn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gaamxuvkw.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/grutjabgf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gpybrvqxh.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gmkymgmxa.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gkpqqszms.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gsalycloq.sHtML


<!-- 参考信息 -->