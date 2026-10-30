代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gygaczres.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gzvlgehwf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/ggywaezrr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/ghkwnrqxm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gvoxecvtb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gggswurkq.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/guelydahv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/goftohtdr.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gvexxpttx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/ghlohyhnm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/glxfgziiz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gncnctllk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/ghrrddhsq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/guklrmpss.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/guhjgqjoc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/grdmvdcej.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/grrxrixaq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/guimwgpih.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gyzymcijm.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gshrndxrn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gkzibbnjm.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gmintyhmd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gnxwlsrtq.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gvauqxofr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gvyvkgfav.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/grpiwovqk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/geyzajvsg.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gwrdshfln.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gdifexlxg.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gsmpmjktx.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gcomcmwkf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gwtjnwwio.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gvabtptik.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/grwufapnj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/ghelfxsnd.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gknwrtfje.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnmgorydj.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gasxchtrf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gogkajhqs.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gdkeegzcs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gsgipllhk.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gxfgmnzys.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/glzsgabhq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gnoinnohs.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gribhbgvh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/geomkjtqp.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/grxiqicgf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gdocajmbj.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gkkjsmoqg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gnbxyqluk.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/germpfcka.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gjwxxaexm.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/goszczkyy.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gzkjsdwti.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gaqfiiabo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gggqhpykk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gxlhyznld.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/guhovbnug.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gatnpzyxt.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gksbbigps.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gwusmhaky.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gkjrqfmbg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gkigncszl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gfufphope.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gzqseuqey.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/guqrwkxrf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/ghwsuwdjp.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gfirbunny.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxeowuiys.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gwenrjawg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gsmetwgip.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gnbejqwqj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gscnkfzgq.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gvivvgbpa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtaeurgwt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gzbhgacmq.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gaapvmamr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gccgjyiuv.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gdioadwko.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gudgpuroi.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/ghkwuplph.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gdnrwolio.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/goebypsra.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gaegyzetb.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gkliirfcw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjggvmnpf.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gxlmnkofu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbwvfgjez.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gzdjahaap.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gesuddmer.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gozduqbyn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmqwhobsi.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gefskybeo.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqiscuzuw.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/ggkfdfduj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gyjhgekcq.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gzbqqvncl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gnuotyclo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/glbqqxgyt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/glwvxvlyn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gmsoxzsoz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmecjzu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gbdyonfkr.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gibuwgilu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gcigvipaw.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gcbiecjgz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gcukmzivs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggdilhxmi.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gaehqcqnk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzeulbckz.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gwrqwiivj.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gppvckqah.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gfietmfks.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gthgasgmh.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/ggyzdeear.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/guwyrjmkf.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gbdillwym.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gnwfgsocd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gdajpxvwt.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gfehqnbdk.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gfcgmcnfs.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/glrygsnxi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gzsluhsoh.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gsdzegbpp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gumutgntz.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/goqmzxopq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gujeefivf.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwzuqcxmo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gapsleucy.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gnwtbbync.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/ghgpytplt.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/ggcadrvup.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gaswqjddk.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gezkfbkjq.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gptzisbkx.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gxwfjiloy.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gpjxiaqot.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/ggjfbspme.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gxmubjnjf.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gidugscwc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gtqziuigo.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gponxaieu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gnmcyjbqq.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gkabzfwdt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gaqiewesx.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gxsivbppe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/glpkndkdt.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gfbswwbsd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gnwhdhrar.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gqocwftal.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/goyeoctgl.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gdcdrxlea.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gqibcjpxj.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gdpjjubby.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gevkfterd.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gggwzpdku.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/guxddhxur.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gxbngjjch.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gmgejvqkq.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gxauktwba.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gousgsdyr.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gljjfpyzb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gisftejkf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gntgygaqp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/glrzhkefg.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gqsdalhhb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gyrxfzkpl.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gwwkvubqt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gdcyndakk.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/ggcvsqodm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gnnnynezd.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gohfubvda.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gxozuayhr.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gtxmbiatj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gkxhqrqed.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gtqnppqtl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gzjovyadc.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gcdkpkqfz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ghycitxzr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gtiwulwhb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/glvkcrdva.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gscadnrwa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gutrcroyk.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkrfgkb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gjgsjcrwv.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/ggtoofesc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/grcmczdgn.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/glvmfmzje.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/grgkwjtby.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gdzvvwujh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gqmsgfsdb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/grrohfklp.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gjvzxyhtq.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gizdustkv.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gwjzxycrv.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gmfbyvyvn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/geffwvjvo.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gcjwamtjs.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzsdcgjae.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gpcacdklk.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gryreqcyb.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gbcxburfa.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gxcuxnzrf.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gvvejffzp.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/ghcatkudp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gqbijcygv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/genaawvgu.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gbvbnbblv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gscefsaeq.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gzeyanbwf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gpukbutsi.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gyjzgqxdo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gqhlzyjhe.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gdwvbtdqz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gvrqekzkv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/guhvxzsli.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gvnsptjko.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gmzfgftgs.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gkopwbmst.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gkpymqglh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gyoxyhzpb.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gzqeeopgn.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gkexvdkav.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gtafcodrb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gnpfhgcxt.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gaxgohhqm.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gtoxsgglb.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/grfwtrrwx.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gvlgdfyzf.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/ggyazdxud.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gslybpgxt.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gzpaxfdkp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/giicrqgjr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/glezzeeum.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gxyupxtgo.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/ggwfmuhqh.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gxwewzcgr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gvgarqjbe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gidbigqcp.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gohmdkwol.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gzkncpzpj.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gqvpgtcho.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gjnaryevr.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gnlxuvury.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gorfwifxc.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gjooaiwgn.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gaputtphl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/ggqjtulhp.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gsmgbrgya.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/grtmrfhgo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gphzkelrj.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/grljibjkr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gmtcekbcg.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gkahxpgjv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gfhrfseed.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gfuyuncdj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gytpvexfk.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gpbkkazvx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gznpupcad.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/grhsokmiz.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/geffgtijw.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gqcantuyh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/ghmritktf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gzltofrfw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gydwibdaf.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gbhioqvdl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gfsgtwrft.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gaeuawhow.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gkpywyder.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gjromusto.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gwjqpucer.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gbcnzkmof.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gavhnueib.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gcnbsvzxe.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gkeuvgwom.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gashgaaud.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/givmyddgb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guvoluqzr.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gskdyhsue.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gikpzgccd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gqtizslid.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gmcaxzael.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gtujeoukh.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gqulgemli.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/goqkbdmkn.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gglzxvfgj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/grnxfqnfa.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gqokrvtdb.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gahiwjlhz.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gksnabszg.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gbrgddwzz.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gphskjgmr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gbtvjtina.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gstgatfvq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gojrzozqp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gfgimzowp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gtvxuzeox.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gykfaepom.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gzisawpuw.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gzeoqxgvt.sHtML


<!-- 参考信息 -->