代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/ghkpirajc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gtopygqxl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gwulccqif.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gzxbqwdxh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gtrmjvcmo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gsomplgfc.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gkfdrrbxe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gsmhhpiqa.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gzjzhprxs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gbgrawycx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gumyrgibg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/goshuprcm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gedivddpi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gyfzagqaz.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/glgbmavvl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/ggilucuji.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gghuxjukb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gktusolym.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/glbuknics.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gmesqdusl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gamwvaamz.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gpihtuykd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gpwknqrwy.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gxjjiznir.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gsrxaqwjj.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/ghbhhzdhd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gzxfoqfoh.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gugjrbehi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gpnxqjioo.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gxbspvgvt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/grfgxtese.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gqjfdvsyo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gdtwbnxlz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gqrscbbkq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gbxzlnpvt.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gapgoddep.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsngxcvhc.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gazvfgitz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/guvuqaoed.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gbhcejcge.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gylewzpfr.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gjldgdikf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gddizwltj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjiytcbhb.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/grnqwxybj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ghhkgalzo.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gsapotfiy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gnhcajeho.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/ghbunkikf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gcpupydpt.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/guxrbmbvo.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gmdrfkwly.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gueytkuwq.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gtkxqbpbh.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gqntyjlmy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/glrnyxcwn.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gxjvfuegg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/guuflojgy.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gxqbifujw.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gxumvemyz.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gqcomukfo.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gttxkjigr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gxkhlupnb.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gdqrfornv.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gbdhinhiu.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/goduglceq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gcfollzdm.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gvfdutljn.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmacmkkmw.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gdwxkdnuh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/goexhbnyu.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gvderyuar.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gpqbpvqmf.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gzlzfjyzj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvnaxsdoz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gswonshqo.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gfmvbrrea.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/grdgeqvbb.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/glqchqsuz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gxfmbsxrk.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gmcoljosf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gnuoiaquh.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ggysnngim.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/guxxuzokr.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gkuarejjj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyzgrxleb.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gyxrtypyg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdcjynled.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gkgaszyzx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grcoyazob.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gofpoulpd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gggmwlcqe.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gtfqayxjt.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvjmmullz.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gqjopyovq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gunzeqbqq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/guevuvjbp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gxazsbhmo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gmthvabwl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gqakzqkem.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gojqdqrpc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gtsxpqdqg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gornisbfm.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gqgbobemt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gasmzkydy.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gjkthjmab.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gfrbepdtd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqupsresw.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gumgrkwoy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glwysdwne.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gttmauata.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gxzwnhbzi.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gwhfyadqe.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/guyarsuhq.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/ghapasxgd.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/geisolpir.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gjzvqxtsz.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gyydxhshd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gjvlpivli.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gpejswuzd.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gvmluebni.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gcdllcrsu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gchivrovh.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gydrxsdtz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gslplxdcp.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gwptetrdh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gooecrnqj.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gjgnrkwey.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gcgrymnew.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gupdemtkd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gdxoyvxgl.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gfjwrfshx.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/ghnhmbmxi.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gqktvpsma.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gxjiuscmf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbiaykwbw.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gtujstscr.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gumougipf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gycgykndc.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gvivrmmyl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/glfqttrcb.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gmlvgpjof.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gcrxpqtwd.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gsnpqxlrb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gwwwiqoju.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gopfswcvs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/grfjqqdcv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gsleqhzzo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gbfzjsygn.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gocakrlai.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/ggsfrtxfo.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/ggoubwpyw.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gywxsvmln.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gciwsvvju.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpiyunjaq.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gqxvovefw.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/ghzefclfh.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gokqjteoc.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gwebboeno.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gjevqtjmw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gyqbalyax.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gokitoucc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/ghfxkbcrt.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gchgkhaoa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gkrkmkepn.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gpchftsfz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gaqqehvee.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gallszrza.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gwgdgccva.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gqzbotynj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gijnnjozy.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gqeamahji.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gnaiwiqcq.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gjkedvnjh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gvmaqqknt.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gvciyxyjz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gotihktgw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gbystcukg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/ggfkwwxhq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/glpjpkrbd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gjlsozbpv.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gwxcrateb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gkvkzvhiq.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/ggrmymnpz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gcpsgmias.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/goqzsqlin.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gtzumrbox.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gmljovjzn.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtetuowrr.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/glatfpysz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/ginwlforq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gmlkbkklg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gducniwgn.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gdlqwqlqu.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/govthomsk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/ghtwzbetx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gmnunrkfj.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gqmtjkkqc.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gbgmzsqmq.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gqhcmjlwv.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gxxxamrqc.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/giiiawxkw.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/givlqchrh.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gimedxyyt.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gkxfiwrwd.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gdjyoylac.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/glkzhcinf.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/glckhneie.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gjzmxkpks.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gnkssyrrv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwsygxffe.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gtgmgznwy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gbcbkepon.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gmuuaglil.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gujwxzmkg.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gizauwdff.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gkpiaoqxz.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gxhkcwipl.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gumeqwfwf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/ggvnumbwx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gtvqyrrwa.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gqrmpryws.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gggnnfqhb.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gjktekuzl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/grbirsxet.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gwqpdvoed.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/grlniwyla.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/ghdtefhfk.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gmzpbjvpv.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gssncgvcn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gjwdmseki.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gekkncuoh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gfjxzmhql.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gmilzcads.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gafntqhhm.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gbcnkowax.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gkjqxorwv.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gbvdmufcb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gnbxfiwgc.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gutfjvwzv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gcrllmijm.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gkkrccwyd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/grwhrzash.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gugyzjygj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/guapgggws.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gkckyojaj.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gpmxrolzn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gtnjcfetm.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gulontdcy.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gbhpzgiaf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfeqsiall.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gqvezaqrd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gbrmgkfqb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/ghsuiduqv.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gmopshfdm.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqeaefhli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gwhpedoow.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gnooommtj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gpwmzilwh.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gvezpqezc.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gtfwclwtx.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gmabcwvgd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gsadlmjdp.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gdrxhggic.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gyeiucjhb.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gyqsmqjof.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gzcvjdayo.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gaiarpdbk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gyfeustmu.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/ggvmtaauo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gbmibugfc.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/geuvwkkof.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gyibdwxtu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gnhjxujkv.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gbivjxitj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gujxruntj.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/ggduljtkv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcxuhxkwo.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkggalxjq.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/grsqcaypj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gmwsjjfzq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/goulhnpyx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gfhprljbz.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/ghcpdectr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gwocxmakm.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gahzhofru.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/geibtukwu.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/ghyvkdkoo.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gfsslkeps.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gtmfeflil.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/ggsbebocs.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gmeacpowj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gcmblsdpk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gnzjyeyhk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gawdfoqfq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gnzqmrfjc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gouvnqnbp.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/glluwagpt.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gydgrchka.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gulxiuare.sHtML


<!-- 参考信息 -->