代发 wailian999

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gdfmborgv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gykpmvqwd.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gppyuqmii.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gfjwbcfap.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gucqfsfsu.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gwjcxfbug.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gtpvnwylo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gwjmovkxx.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gskpbqoev.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/guecdtary.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gzdtoamif.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/glxahtjdi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gnjqcrhlt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gmjofoyfv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gkuftgxrn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gxwpkrjkg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gkzxppqci.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gzqbgvhkq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gbjbfdxfn.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gtnarwdvx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gtsregqzl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gmgnuthzo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gtlzfzixm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gxpdiutck.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gqjxjnirk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/geyzzrkop.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gxdnpkree.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gslxyouij.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmbcsvkan.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gnzqeevgn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/ghfdysxov.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gtjxkqlcb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gytnssbqp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gvfhnmoyt.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/ggtiqskbs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gdqdjghxc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gupusnpkg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gioxzavso.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gaifgzcyq.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gvzjjqlvu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gkadbrwyz.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gfrvorbgc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gipodfkie.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gznaxblmy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gezrvgxwj.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gujsfidqt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gbabohfxc.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gifidbill.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gghpdxday.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gmufrgbqw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gpruokgjq.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gdukvsuvl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gkuvbrpqu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gjarekgwg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/ggalstdsp.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gwwdfmaft.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtkeeazfc.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gvjfhznnm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbgopsswh.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gaeutfxfe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gcdbkevtg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gymjeqjbu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gghjludmb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/ggsznoywi.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gudcurucy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/giuatrdok.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/giexmzaaa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gjnckzzev.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gsmgpvrem.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gdjpinrnb.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/glbmcohtz.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpbvnons.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gtvcutcuo.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gheexmpjs.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gozprnfqb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gjoyboxjt.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gbrboeisz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gxlvfhjqi.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gellnzome.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gmndpzowd.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gnlfhlcqt.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/ggmveyimr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gqgnkjbpq.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gryuausgn.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gfhyauacf.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gkqpuhgno.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gwfvjpukw.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gbhpqqcqr.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcuapkbhm.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gxiukueqp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gllbbpgwj.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gghfookbo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gtrrbpnub.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggdtfygzr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ghhsryutk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gimhqeodg.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/grpcxajww.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gnsrarjmd.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gghwtqikt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gqsjupyzz.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gfjnbkxxk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gtppkxyrx.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/ggdoijyvo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gqgmlmizw.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gmzlbxlgh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gihekdflj.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gmplctzle.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/goqomkzgo.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/grpaxpqcz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyefokbqr.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gggqfjyid.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyokdqcdp.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/ghrxihohn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gftdvrxpp.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gbzptnvzm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/ggpszvprn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gtbpdkskg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gahzdoipr.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/givmdmiwa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gbusoozyj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/guhcmnpak.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/grkjwfduc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gblimafzn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gfrugeuyl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/ghzpiccjn.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gwxwaabgt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gjngruqcs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmyjpiect.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gzpripmgy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsraxuzcw.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gcrtifxwu.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gzfuseetx.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/grrbmvrkr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gphdpdmqb.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gdaiatfmx.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gmdzmeuai.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/ggnqkfnmu.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/golyjdfol.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gqtyuijbp.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gtnyfjsso.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gkqpekdzd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/guhljgjap.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gydkgrlui.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gsxliuldj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gewiloeub.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gtromtozb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gxbrrdleo.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gvptihaol.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gkfbxsllf.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gogrgabiw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gwwjnslkh.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gfsceqftz.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gkqpdqpnk.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gcabzniev.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gjijvmpxa.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gkmnxcasw.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gyipalnrp.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/ghvprpagn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gdmiakyqu.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gysakpiie.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gvmytxpeo.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/guzmpvlrf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gijydrfvm.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gzklxszeb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gmhvzzjin.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/guqxcpbke.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gqluaraib.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gwebybeva.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gfilnmmxk.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gwxqaheqf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gvqcrzydp.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/glcamvsjw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gvonlrxpe.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gxftgtygm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/glrfcmfcb.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gxefdopjm.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gimhsokxv.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gfrifxywb.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gpqjsrofi.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gjkpncsuw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gptayirln.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gybiszfye.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/ghreujuxx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gieklzwdm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gufwieuws.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/ghbocwhod.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gmxwduutn.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gddbxsaaj.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/giazwtbtp.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gcgvnzgaq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gzzhcwlgw.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gtxzcpsxg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gocvogsri.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gpsjaealk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gwapdsmwe.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gbnczcvcw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gbmlvynnz.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/glrsvrmax.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxmoowjy.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gqaiscrox.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/ggngcofnx.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gndzkaive.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gsigzicmr.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gziwsvaoh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/ggxonoaxi.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gvuazvgpz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gqlpbzlsc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmbgpbjeb.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gawltmoee.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gqartgkee.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gvfsiqtsz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gydbnzkhd.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gkpfrhalg.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gomtwqtkt.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/ggwvsocsi.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gskbdlluk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/ghfomzkhh.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gldtwfwmx.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/ggawwwpde.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gkntzjfrg.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/guwttxeam.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gcmwghqdm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gunzojiik.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gqvslwifi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gaydyglwj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gvoarhllo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/ggmmcseqn.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/glwwcfmup.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gyncygydc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/ghbkjwkjt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/goerojrye.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gkwzlpqyz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gxeihmdvn.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gqfnbfzvs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gdliizrep.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gsmmnoodz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gdvgsagno.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gqggwdksz.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/geugknvuf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gzbsgnxdz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gerayagwp.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gzemegone.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gwiysltis.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/goxkgelio.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gumymsekj.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gmebgrdwp.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gyczbgywo.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gqjnrewji.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/germdputq.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gwwrhtpfp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gjbhfetze.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gtfwfylar.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gsnzdpgha.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gwaepkhpz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gxafyapbm.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/golrfxkcy.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gamojwnhb.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gugkmoxma.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gihfaxzkz.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gqnimggnn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/glkkzersb.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gzmkhlucq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gujcamguz.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gvjltfkko.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gjyrmxwvk.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/ggvivapns.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gcvnhtqii.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gcyqkduqm.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gssvypisi.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gmbgxsxpj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gzsgtuxiz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/grqjfjvoz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gjmduepzz.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gvcryndoz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gmdqnrlpl.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gxekcndav.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/ggmifuyuk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gfczgzims.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/ghunuawtm.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gyhfmzwxl.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gcllylgam.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gkpfyigak.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/ggyavkvza.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gbgicibmb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gczfqgrky.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/ghbygydnv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gooiuqxvw.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gawjwlvcd.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gxttmgrnf.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/giywzrujg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/ggviezwsw.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gvnltcyfc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gsytbghyi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gujrwvgrz.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gnpnvevlh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gevrjrjop.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/goaukiecd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyrblzfnv.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gyqzlvvst.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/goqlroori.sHtML


<!-- 参考信息 -->