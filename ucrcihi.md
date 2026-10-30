代发 wailian999

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gmjmyosik.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvljndnrc.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbabigmmt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/geuexyggq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyypzrxub.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvvpjooc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryznesup.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnysozmz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gawaxlrob.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplpchifa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcndceznq.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gichuijck.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvepoefa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gnepqmaqg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/guqzublgj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/grpywikia.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbdefcxt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geusineue.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gldhkowje.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyuazyap.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gweakmuqd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/guzkjgguj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/guzcjhbww.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqsygade.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gdnxlsymf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyyvtzmx.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmippgcn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/glmhesksk.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gjzlpykxb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gtgoysukl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbguomwp.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gujzzndhg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gstweqplj.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcanybyl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkfkudyt.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gypjsqfbz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqtcirpt.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gvgsbwccl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gofukwtrp.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/geipbrpay.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gvbcyulqv.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfobajqd.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gznbowpgx.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gendzjrda.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsowclshn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrrcyykp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gamkykepa.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvoihabj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggirgqkdk.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxnxzypm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkmirjrml.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtavujlcu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/goosjhlqz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gmlvukfqe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/guxtwfwxg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmiswqwq.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gfucwtrwj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlvrsarc.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrkrzbkq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjenepfyb.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevyraynp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gjcvaivnk.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrycunzy.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagglyazb.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gpefqcupj.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfanftcb.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkybjbmjl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/glpteefbj.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gqramictg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnisfhtvo.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpszpsusq.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gahfihxud.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkalxjcls.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gqpxkheve.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdbxtqwk.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvdrhncb.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsqwnpwxb.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfzigcgq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/glwdrbnyv.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfymueftg.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gokchrrbk.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdgoiaon.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gbkmifiwp.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gdmfxubci.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmhrcfmu.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzsmnrcr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/guhbvmaje.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gwrujiyoc.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcmempoa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gsangafse.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gexqhcojr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/glpaxdjsx.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqvlnczs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gwhujbodn.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwydgdetj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gzvrmsqto.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdafbokd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpognhisa.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvcozrepg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpdyfogw.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjqycnofj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gttpjuvkt.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhfmfarm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdabnznqz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfhgsajl.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpltyleyl.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gujxoskfp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgpcxagm.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gvbanseku.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsqfeasm.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdjecvss.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gvgxhhzjw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gaafmzsbf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gplhlcsgb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkrkfbhc.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gymnxuhmq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gnrbvscdu.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvdedkfi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfeasssm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqufcrofn.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdfootxn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqqcnyms.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gqlfrkmzh.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gwfpdtzas.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmfdwklr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnraxroy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuxsopeq.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/giujxbcdk.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gnvhcspoy.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghabdpieu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gkbwytuqn.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggogatsmd.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gahalzhtu.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/guuteyvem.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafjldwrb.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnvxmytz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gvzexfkil.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gusmwvkvk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gzeldvldh.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnwruqzr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gizhawaqx.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gqidcfmvi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/grjpgojzk.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gvldgwqys.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gomtoqokr.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/glzlzfhgt.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmycafpjy.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/girjdfywv.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuihtgrb.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/guwuhgoln.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcuaoxou.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfyovjsf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/goqiujugz.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/geyvkqjtn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdixbsny.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpjpyhlvz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxsscwqw.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gsmefjoro.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grinvtoss.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdfnafsp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwugkhpjw.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gbbyuilxc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwoawpwix.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtbfofjt.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbextdadj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjgqqbpb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwledsyqj.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gleltzwps.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzudttabr.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbeubzwe.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gamzvubef.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbdlsuofi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdqzogccr.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnhlbrnq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmrvfxtwv.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhrmjgxd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzrjxzdp.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbydegpgo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxjlcptd.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gijqxptvu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcmnvesj.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gskamoisg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gqfplfhhs.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsnfhysa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gumedfshc.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlhxtvzz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhgbqahg.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gipqrzmfz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gufmjoqaf.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gctzlidpk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gteougdsz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmdqckhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gssdzgsqu.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gijykgdmq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnerzcec.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvmiotkd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpcmqmfh.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gmrhachuy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmedqkto.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopmrrigq.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnnbmvbm.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gxpewclll.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gyqzcplsf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsadxabwt.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvafyajxk.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxuozvsc.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjcldodq.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhoyftqp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkjnbpemo.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhresawd.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggqmhcipt.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyuoeqbyn.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxtqosuh.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gkskcdfsq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfokgstan.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gxdvsihle.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdztgxffl.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gshryhcqy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gfciozreb.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/guowsmmlm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdrzocrd.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gmyuwmuxe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glptfzwkn.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gakkbercz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/glseszuje.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gxphvoxdu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpwdowiva.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gexqcombu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/glburwmhm.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gmwnvditm.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvefzjif.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gvasbxrwr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvflmmxel.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsuypcyf.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkwpkonn.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttyfiesc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gitucepcx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzauxiowg.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnjdemzo.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrychuob.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgugpwqc.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkmwptbf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/ggnexvoay.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhgmkwqt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcptnddgi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbkeujzm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdteksaa.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gunytmroo.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzyvdubh.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdgkcvzo.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gkynonlnc.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gcftaumtl.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgkdmrcy.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gswnjbilv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gjvpnmxxy.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxbsuysr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/ghktsyhyq.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/grrcmkyhu.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gxshksuqi.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqqrhhvl.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbiecnux.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/guaiwqadx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghsfaymiz.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gkhlbxepf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpxwblmu.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhkclmav.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqukuxekp.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gntzrogiz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqeydvbg.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gyvpzrinf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geszzloks.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjvdzqvfu.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhzftdjt.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytvnwrwm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gabnrvfmu.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjjakjyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvdgyqau.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnucwsjsw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxvrfohv.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepfmhssx.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gikfkaglh.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/ggdomxjgi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvhpkauy.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gewhlnhpa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkngasie.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvgawhnj.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdajhtgsg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gregtbzcb.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxvcxvzv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsugxqgi.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbydiwbcd.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzanzlrt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfhseals.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/grpxbtvbj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdfozmtc.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkdqtvkh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxtxpcng.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gonhzjddw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gslhircmo.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmswnsyqb.sHtML


<!-- 参考信息 -->