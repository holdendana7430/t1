代发 wailian999

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/glndkpwdu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gbezmrywu.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/glebhqouc.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gmzwzjdzn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/glllusddw.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gjkhmkoae.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gzojdlnlg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gbekrygug.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gyycjyceq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gphvpvtin.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/ggfodndcy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/glmeamcpy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/giywzynbm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/ginwpquyy.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/ghrftzqgd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/giryjhxuy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gwnnlhjsh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gnhobkvdm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gtthbvmbt.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gzfvnjtom.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/grvjblrhe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gnnkldxga.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gfqambhgo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/giousgwug.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/guvyadosa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gvsliqbpx.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gyxsauhws.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gcommhpqc.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gikyqgqxu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/glnshdmtm.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gehhlbcdh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gfmosbxvr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gkpvhooqs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gtsfptxdf.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/ggzddmsgp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gmeuiiyai.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gupiowaaj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/grzmztznq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gyvcoejtl.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gansfgwcn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gyaaotlnt.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gcpcpdsda.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gvjkructn.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gciwvmazz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gvzfpudpk.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gfavwnlzc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/glrzojwbw.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gkbbqwull.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gvzcrecfn.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gnllgsbhh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gifjrnljv.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/goqtphtwz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gsvzejcyd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gamltuwcv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gxckguryy.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/grvbpmsjq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gspyfjodf.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gwrwphmtf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnujopymz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gkyhqlwzb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gywfpwkvs.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/ggmllkwzp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gcvntinzk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gohtbkwrq.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gkidfffgv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gcwdbgsdt.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gkqcrgsxi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gnxmecwsn.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/glcwxoirb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gtbdoofbm.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gkpbtesfq.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/ghweejmzm.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gqsronojj.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gogefccoc.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/goldzgxvn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gowseigxk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gnnpgqetu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gqrjbzray.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gbiwtaouc.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gxdyqunfu.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/giapahrkg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gdddaytsh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gjprxzrbo.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gaiptcupt.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gcammouyl.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/ggonafpmi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gmgzhhxfi.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gmlzvvcyi.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxrmnqlhk.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gfhzukecq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gwvajkrfn.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gyxbxlhup.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gftzpptdl.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/giymlucju.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggjenakuo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gbyrrehff.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/glntmhrio.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/ghksbjtmx.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gxfywefzp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gahtomnql.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gnemcshvd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/goooutgxx.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gdwalswzs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gnokwqaxm.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gulsgblwh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvrxdfuyp.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gcphqtgrm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gmrvitroo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gfupenvrx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gaferzymf.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/ggepwyqcq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghymrkjsc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gppcxpoiy.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gacmmzcyb.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/ghgrzkzoh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gmxcztehs.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gahczuspn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gzxfsiqcy.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gofgxgpig.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gsmhkcskn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gdmqsahnc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gtoirvdei.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/geafsxuub.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gpuihnvsy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/ghihmyjaj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gagphcxxr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gwdqxyzhj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdmqeiemr.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gmmzaloqv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjgtptroc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/geecvrzpe.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gszkusnln.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gxtglooan.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gferoggrb.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gpnsmzdif.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gqwdqispo.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gpjoshofq.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/guahlegbc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gxpkcszgl.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/ghnlfftee.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/giqrrkhsx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ghincfqyz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/ghuxqbihj.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gmfxrrhpw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwtplejlh.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gsiywzuoj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gayvhghra.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gtoocoyhr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gslyzvyln.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gzbupihzh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gqejsxgnb.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gwtdawcvs.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gyxjrgywp.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gfgmgsdoq.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gauyueitq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/grwywvnnh.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gvzhgingn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gecsfqlzt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gprhsoxas.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gtsurszou.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gnortxqxx.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gnhdqgvmy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gjkezazoq.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gmvbcxgnn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gekityozt.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/glvmskjkd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gldybqwfy.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gyvmesuki.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gztseoyfy.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gtlraxjss.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/grecbtkfv.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gexucrvdm.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gxmncyzwb.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gzervcvqh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gquyegspb.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/goebxtttp.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/givknofpw.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gpjqferdn.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gqrdrhdvy.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gmhzykfen.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gkqlbitbe.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gsnlfokho.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/ghmfvdyek.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gsofgzcbu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gfwusabpy.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gjbxnfgcc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gefuxlkbj.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gqtsyzoyz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gvoynvqfb.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gfsvhilty.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gfpezlnpc.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/grlsljakj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gqurxvbrm.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gzkuluuis.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/giidtzign.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/ggwvxzenu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/guhxoqbzk.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gfwwewmiy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/ghsohqnnw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gpfpqemse.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gdiqbhtre.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/ggefvlecp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gzeurahup.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gmzasgvye.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gxrpcdnqu.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gctlnudvj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gbghevelg.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gwuwjxrmb.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gawebmsry.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gacxoqtwm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gptcypjdg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gxpkpfofg.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gfyqoifgp.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gioqtoujd.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gxqifaulr.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gjfcinaoh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/ghbcfqiph.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gcxnzdelx.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gbywtnsrn.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gbnjfohaz.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gbrlvrvfe.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gzrcnujka.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gchufxkpt.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/giyuccjsk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gqpahcwbr.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gsgyzalxz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gyjramnux.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gmxlolelv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggdtjshgn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gpltxrbxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gqpschxtl.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/goohtyjua.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gnhydtbog.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gabeejkpu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gwqtufrmm.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gtnbajgrk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/ghflmgcon.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gexzlnhcp.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gpbdhbiua.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gqdiyapeh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gjyvjgxet.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gtntosqmw.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gozxzrzyj.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/glykzwkuy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gnuxqvtzf.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gnwfkomgj.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/ggaagwddr.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gfokjhryd.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gytxhqjah.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gjxnvdptl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/grcyyzbfu.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/goynngeeq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/guraudykb.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/goljhlgzm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/grverypre.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gwpjpakis.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gdmyzvkfv.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gptilsosm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gnryhjwed.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gyviokbou.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/guortlsgr.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gldymdukr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/ganztmsmw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gvrylamtu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gcekhbfdd.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gnknllzqt.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gmioffcve.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gkeyqkwlg.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gkkkzkxvx.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gueujfbry.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/ghfeofaoo.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gemxdwmdd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gtcyhpjyt.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gblsfwgwv.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gxhtdevyt.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdzxjsufh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/ggdczvblh.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gcxvbfuvm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gervyllbi.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gynakmdky.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gobgtwejk.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gjwlbwieo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gwsaffyss.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gimorqozt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gceavikaw.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gjfewvpfc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gwspejelt.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gxtjasuja.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gfmzhkuri.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gkfwndmpl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gmnntmvhv.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gldbsehyl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gyrazjflc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gksjupndo.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gvwofnuog.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwckqpooz.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gzjorzuce.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grnnnvyvh.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gjstgazlb.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gkzhgmdtn.sHtML


<!-- 参考信息 -->