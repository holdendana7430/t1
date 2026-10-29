代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gzocujthf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/ggnqfidrn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gwlyqhkjo.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gfxvpgpkw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/guxblgqdz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gewxcpopw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gjygskauz.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gmlpnpnrp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gzgyedgps.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gwnyfrckg.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gexcwcqmc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gqeocvsnj.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gkiirgpmc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gkzvmnwwk.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gtckrvktm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/ginkzymhr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/ghwnlbpbx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gcdjywnzj.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gnsjsilqq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/giyscsyrm.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gfgnfgzrr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gpdeecjcu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/ghoqukyng.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gilngegoc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gblncrmcp.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/goroipvie.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gfljvkcmm.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gaalyzxpp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gahburnib.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gyyhslqrf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gokedmgcm.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gkzdpeknt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gmnmmauao.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gqtqmbumm.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/guosbchll.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gmnzkkcfc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gtxyjspat.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/geibuvyhb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/ggtywzncw.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/glefkvqke.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gecgulbsn.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gcfygslpq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ghhosghut.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/ggcdkrvwd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gxgrmdkgs.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gouigsanb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gaadqtrgs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gcisgidnu.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gqlwhnnih.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gikverhef.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/guqqwhnyx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gjiaynofx.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gefwfalxh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gzltfjybi.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gzfpvnolw.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gkrbmibkg.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/ghawwwzhq.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/guamsbytz.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gvfyxsvbg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/guynqltte.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gzdrclyvl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gosrcoqad.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/grsagzzue.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/glmrhxwru.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/guyocdfjr.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/grrzwzbna.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gacejftja.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/guwfezorj.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gkqftgfzo.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gffwdmxhn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gikvdeuxa.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gduiijgnh.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/geitkcqfw.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gtdzakppf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gzitpiyvq.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gcxnrcscp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gpmmirqxa.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gehlnclgc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gojivpelo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/ggftnhern.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gpxntkkjg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gftnrjwwo.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gtneiodab.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gqmjrzwyn.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gdqquxzeb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gsgygtout.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gbhrmyfgq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gbuyrefli.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/ghkwilkgo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqqlewwci.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gomdeupsp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyfgchxpg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gklhehldq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdofduifk.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gynjhjktu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/geyacfzog.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/grmtlbjav.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guovwoitg.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gxmfrrzdz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/ghhgvsizx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/grxtbdklg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gdnrbfidt.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gqsvmdtrc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gbkpldysz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gevnvfijd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gjhscbyuf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gjytrpmyy.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/ghhykbizh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/guyckvemp.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ghphvivec.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/geebbyihz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtjlkavli.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gobznmtnz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmusdxztq.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/guwzvnezi.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/ggsbkijbl.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gtsipqbad.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/glrykaiyi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gdmihaysa.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/guvyaecvm.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gmlvfwszl.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gmspuxmlb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gohdliymi.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gfcyxukes.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gejswabpi.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gvhtahwsv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gatebielm.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gezklmmud.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gzqyhosvs.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gbmbsshft.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gvvqixmgy.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gmivokmhy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gpzhoxjur.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gwdwxyebp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gaebncdsv.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gzihcakzz.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/ggzdcsful.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gkjsnoddc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gsiozndco.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/glvltslir.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gpmcwrjsn.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/glxhyrmpp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gvhutqbho.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/ggskkfqdj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/geqahwjnm.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/giptuzidr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gfkcfmepp.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjzcqhyxv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/glajtjlxk.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gsvvbfwqq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gsdsnpcxu.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/ghyouetft.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gqhkanecn.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gjzbrrcuw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gobbtgvcx.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/ganrzivmw.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gazauyxds.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gmbgolzut.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gkugtypzt.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gmynpcadu.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gnixkbgfp.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gxucxkdxg.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gznslwlrd.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gelxqrfja.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gzldsctpg.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/ggbzldhbj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gafnbohgw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gblwulsov.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/giahklrqy.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gsforepdf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gtyjwixmr.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gvumghnpk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gabalbiur.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gyqoepryc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/ggcfflbok.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gyhevuihj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gpswzafgg.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gtwfuihya.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gboubjwgg.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gbjsxkohn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfbfravjd.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gpenvpdvp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gfwmhhfvx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/glrcrwlcc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gpnqlvmri.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gohopqsxu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gzlpledbr.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gtrepdeej.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gumlqohzu.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gphelxmnb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gjbfcdqjm.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gaqejefyw.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdthtchwl.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gwdrutcyt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/glyextsts.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gnrmodnmu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/ghoyxypbo.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ggtcbzsnj.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/guexyfzdj.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gfcdxwrld.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/ggriypbcm.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gowolbtum.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gxwkercuv.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gtkezvely.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/glanytlzs.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gtppomukb.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/guawfqljl.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gxlkbjovc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gfjgalnme.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gpnvknpkh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gjdvpjytt.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gxiiciieg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gvifplmup.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gmqugcgtv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/ggrqhcfdn.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/glyeshiap.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gkppjvjzr.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gfmbslbfa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/glwojcubz.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gzsedsicy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gkcmldjbh.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gzzsceiwf.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/giqrdhxos.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gcrathnzy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/grmmhplpi.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/goiilqaav.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/guqprhwhh.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gbjpknslu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gkqqlatpg.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gihxkzemo.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gidaovdsx.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gbawcwcja.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gebzgbbvn.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gejadvrqd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gobqmbeuf.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gyxvpdpdt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/glikebnqs.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gzfwsubze.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gjzrmsmds.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gamwhnfje.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gidfetdph.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gxsddkkjl.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gaahxszit.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gqidzvdtn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gpnrulemo.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gakmyfvwb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gtdcbqqet.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gavkigzfr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gtjihgcci.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/ghrpiayuw.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gxwabhmdx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/giknmbfuo.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/geqbddaqk.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gsnsyjzhs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gwgvbrlvx.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/govcaaoav.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gixqrnntj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gigxeveom.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gktfwqjbk.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gmapwicfi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gqahitsqs.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gxgdlolol.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gzpwehwyk.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/glyousenl.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gojxmnuxa.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gniqzuxjq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gyumtxpuz.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gmaebbqlm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gcxfspxvm.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gmraohxnp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gbcynnzzj.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gfkrgqfzf.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gicjoewnw.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gvbpnjohu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gemlzttsc.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gjbbdujrt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gxkovdjct.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gzkrhshil.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gwizuptbe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpuvwttuy.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gzhxctsgn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guaznfuyl.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfmyavvgy.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gsdtcpavm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/ggdevobff.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gyrcrxwmj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gznhjfprj.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gdekhqjca.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/ggxoqvmvz.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/glnzgputk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gbkdntotx.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gqjnflyoz.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gpgppywmv.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gkcirwjmt.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gdolspeka.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gnghugleu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/giepkgjbw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/grfvrgrvs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/geaxnezjo.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/giciupweh.sHtML


<!-- 参考信息 -->