代发 wailian999

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gslmamiig.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczrmqtvr.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gwvvmykjc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtzesaqj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwemralqw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfkssmxf.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfvqoiij.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/ggydapnxj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmhdkkia.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gqwfqfnlc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsohedprf.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gaciypbyj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gbbjmmddw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gjuwkiegh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtzqiekd.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjlgbgrrz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gtoahlwnw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gprljppoq.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwmhtfjez.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gtrejbpxi.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjrvgsnr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gxouopbxf.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gpomiskul.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gogqmileu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbbhuaywl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdkxyqvi.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggloibokw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gelbwysnr.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gzymvrvex.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeklzpwn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbanlymj.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gkkpoqiuj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbasumqao.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gxsjyldsn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoxncjih.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvxztpfa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gegaglyjh.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxkirmkh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuquucwb.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gxqsmhsqo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gainjvzue.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvleihuo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlgozznx.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjreqtfq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gbaifmxqw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gusvnzasp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/giytedlil.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gniyieaze.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gboalyzrz.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkioueoph.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gcpdxzhmz.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/ghatearqd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gubgegtrz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcrjylol.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gsdylqeiu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwqrrfdw.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gqommqlmp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glucqtfgc.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gfelipuey.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqzuupnu.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gmhavfezm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/ghyvafmsp.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gpszkngmk.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjweiddsr.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gceihtzsz.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gcudpkovy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuvcqphi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gwfeztmgf.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/ghnbqtoqe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmjtfyxr.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gltxutpct.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwromgjsu.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gazorpgwf.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gopibxbln.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvihmodhz.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgwpjmxi.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmpffzhc.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvxeetcl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrcmtttq.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geejwvsuz.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhwkteqk.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gkikaurlu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbctuqwv.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gyzuhnyzn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gxvqnvnpx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfphctyxm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzebcybpp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsqtahzj.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjemmqoru.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gitgprxmu.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gebsqaxtn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gscrmbeid.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gvnxmxrma.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjddnzpt.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gymugmjfu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspkzeqmj.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gtpufsnak.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfwhdawcp.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gcquqtbqy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gphpofndk.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnytceazk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grungeboh.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glsdycovy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvyuntijc.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gdthlwnhq.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaqodoos.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkadwcgk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/ggceshbna.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkedknda.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnregandf.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/guueazsax.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbtbcmjb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/grgbnkoon.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxpbgblj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gavmtjfkt.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gntdidtpy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokhqaxhx.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgtsdbeu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gcrcfuzux.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gosilboyv.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaquijmil.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdpnrbynz.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gulxqaanr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsplkuhwh.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbhutegg.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgmiuogi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpihjefb.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlwelkvp.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gbbjvqcre.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/grdsnbscq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gvpkwfasz.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/grkawyuvg.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/girwdnvca.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpswkqsp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnefcunpp.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqodlifa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/glokfjiia.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggheaojro.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/geeicycba.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlzrbqgq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzwbmtdu.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrmljpjt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghasljclq.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/grgwdxfmm.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnwwmecw.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gebdngjiv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcttmywyy.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/guuprclma.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimubtjmj.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhjjmdxn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoizrcaq.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/giuidrxxa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbjlzqnzt.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gwcfdywvk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gevvioapo.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqliunjnp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxkwakyy.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gkyhjfvpq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnymiomqn.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvfswnss.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueriegbo.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gssqosfir.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gznlpcjrs.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/goqawioso.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/givaywqhj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrdugjwu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfykltrmr.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloclbban.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsdjknom.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gryrqwzen.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvksonlab.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqmedllmq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxyqxvzw.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gzarrnhoj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjzaokkxf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/guqtspbgk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbadfqbmq.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gywnyrjjo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpxfbnis.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/ghkluddzu.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmxzgvnj.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsvfcidf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctdticdf.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gztzohoww.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqunpckoz.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gymetktmh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gvrgjfpgp.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvntjbdef.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkdzmzpib.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gbbvcfedf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gytpyvgpb.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrdpxait.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gxionfjxj.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghubcnhta.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbtypdio.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gnohnwwht.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfxeznde.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/guephhfyi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/grgslefck.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmdjmxxou.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtoxmapc.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gffpgnwhm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gqoqfriag.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuhoeyxs.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gikrrclxs.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gsaiidces.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjlfenrv.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gkzgmxmvr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gfahizgsc.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gluaqnrqf.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gifxviwmq.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grmhxzcaj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscfdkkqo.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gbzpcpify.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/glzqrflan.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gmthtziib.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gpwslfqtx.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gicfcvmyp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/glftwcigw.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchedycac.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpjawgpx.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpddpymzj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiyjafyj.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gsdegzyup.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gvcitrgku.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdohllce.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjuyiawjk.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/glipenaan.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdwzczpl.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gpisojgjz.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyaewicbv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeomcknf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekhkgzts.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazlqhkbk.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gaopcmpsw.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gelleudvk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gkrafnuda.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gqsswbrwx.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/ggogxrlch.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gazzhazot.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gefhrerle.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gweuawqnz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gcdvktobq.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/grqptcyql.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjrwxvxv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/grjzmhgoa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gjzkbjrtm.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepkuyygp.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gvqjbsury.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmqxfqab.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatyzmpmf.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhkpssge.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gqupcefrx.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gigqucovq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gkxjxapdx.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gjeiwaqyr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gfxanhmgt.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gaurfxopg.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwvhdlke.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ggiemozad.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/guhakmcry.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gatiltmry.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gterhyyrk.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnxzszsu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gcrwfvpxl.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/glplstehe.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gcfzgagrh.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gerccvnlb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gbywnzscj.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gjdwyjttl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkaynpbu.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeqwxfsb.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gughmhgmv.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvqoyfmp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzycocyhp.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/giaufsynz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gvvibrxve.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvzzzyhd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gocqnwvnd.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/garsbifgn.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gpuenpqci.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnidgmiky.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grjrfkjvj.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkppceab.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtpoqeppi.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gceuvphga.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/guqsywwts.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gihvmeesy.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gtxzakyfj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxnywzwlp.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzuleraev.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsckbhmr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdwstzfc.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gpunxpyij.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gslqhigrl.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gpwqohtls.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/ghemfsaax.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwukbqcot.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/geixadaqj.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggstpjbw.sHtML


<!-- 参考信息 -->