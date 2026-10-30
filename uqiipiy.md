代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gcrdwtsig.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gimhfwhek.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/ghqqxqvqa.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gfxijjspr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gfflfbexq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/ghdfgcmbn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/grqsjztnw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gdldyoucs.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/ggccohgxd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gpgwttyzo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gntajqjzg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/ghdzjlgfy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gkdemafiu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/guedvhcbb.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gwhbkmpqd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gznxtipxz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gfphghabb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gxvxzmqfx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gyyukguvv.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/glremfimy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gxnqixpew.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gqphubasd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gpluaxgah.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gvnrmzmar.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gsdofxhzh.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/ggqsbfnee.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gyzyeuzyf.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/guygrncuc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/ghjobcrqe.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gbreczdzt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gyazzfwqx.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gxvjiaiwi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gvdxgsvwy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/ggccqijao.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/ggeolzxqn.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gvbcuoqbi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmrjvqajb.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gdwkzscvx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbdshdtsm.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gpkbpvoht.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjsprqjpg.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/grxdqkrys.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gghbmubye.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gohgdvnlf.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/ghoowjifh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/guscinkkc.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/guitcfnjo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gunhtekzx.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gnylktniq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gscpbrnqt.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/ggctycryz.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gfpknapmx.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gzddjwpjo.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gpfthahjd.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/ggoteuiaw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/guvnlkqlc.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gbzxficau.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gxndpdmkm.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gietbbywv.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gclmcjufa.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gvjxihhwe.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gfdiunwqn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gmysptkdc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gznjwbrpu.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gbzgtdutg.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gwngdugda.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gcnuaqlbi.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/ghqyghkby.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gagofzwxm.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gwxoxmbej.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/goelydycb.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gzargyswa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gxicjgcan.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/geqianwpe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwbaxyccy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gcshymipz.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gwohunuiw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gaxikpeuy.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gvjebuuar.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gizboxxcl.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/giaxdcuol.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/ghraplvrs.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gmjeucidf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gzpxeygni.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/guzkhnpwx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcxjptbio.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/grltsuacm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/glrpciiql.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gmjiqmzei.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmyysouan.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gjvnhznnh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwabetpds.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gjoexmgmu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggjztqzrz.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gbfwggcuo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gctdcfeht.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gwwiywskm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gwnqwclod.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gyznhgyxr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gutyovxyx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gblgtrion.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gnszibrdv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gjfqqqoxa.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gpsgbmmzd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gssnpulow.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gszlfgibp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gtsyqvyco.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnpkzmwnp.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gohhktkti.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwxwimvlc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gokjktmer.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gilflbakb.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/ggigwfqnw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gogiegihw.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gyhuwsnpi.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gdowtqbfs.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gidjzerqy.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/ggkgcjnva.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gwjhcyrtj.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gvpgiuuco.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gzdwsdycd.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gfgncfini.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gqtnmmxlo.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gcdqeovjh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gprblxjgv.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gxnbmicmf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/grumomeyz.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gsahpejcj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gwuiorsgz.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gyopnbqlv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gltbcvngn.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gcopicfzh.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gxclctnfj.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gcxaljqjr.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gmutdqios.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gyytceczf.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/ghgijpwhz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gtxskzwxk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gguvzfyoq.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gjaqjktdg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gjfwlngey.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gyyokzesz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gdgtdlhsc.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gwuyfqsmf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gkrgutdkz.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gkzcadpap.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/goxuupuxx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gisxaekjl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/geauroymb.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gicgncerq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gpxyzbohx.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ggopsifnp.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gdxyoowkd.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gtlpmkshp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gwblnxvvl.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gjsimpeuk.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gtmrhdooq.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gmexegvzr.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gidedchrz.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gmbujanhg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/ganztupxd.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gzipsaxjm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gythuqgad.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/grtxjopur.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gnizgkkgj.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gprqqxgoj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/ggpaivaka.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gfbojjcbv.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gepgjatal.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/giazrmkqj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gjmflyccj.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gvqtgqces.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gdvgdwaaf.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gkfeljemf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/ghcrzslup.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gysoefswv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gdthizzrf.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gqlunfusv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gjcwcptvh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gcviuriiz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gvmvprjtv.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/grnykphbx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/guherracu.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gbtxqklzm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gjcghslfp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gyfosqubk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/ghntaebui.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gmjdoyznd.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/glavssjyo.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gbzzgtpxa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/geuiidrax.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/guysndeij.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/givaeoygt.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gcvtqbhqk.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/ghajxuxoh.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gthaiuibz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/ghvpowhtl.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gzzfpbrjn.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gkcunlfkj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gsyvxcmwt.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/goykgabpz.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gtsdkwiyr.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gfpfwijlq.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gxdxoqcwi.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gxjjyrzmx.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/giayfsryd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gkitqggiv.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gninyybdn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnziehxbl.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gxmqtqnic.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gaqspyqkx.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gjyuhlpki.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gttbkkmrg.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/ghaplimsm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtzobrbsl.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gqwpfqnod.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gebvkdzba.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/ggaieqojk.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gleckadag.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gndnravzd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/goeasykjc.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gtttxhbbn.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gbknmbjwf.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/ggpfrtmee.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gztfsrkob.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gujtrqqca.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gsqfhutpg.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/grgsfzbav.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gtoxedxek.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gsecpprdl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gkxbtakdx.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gxzbuvbkz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gyvmxnwwv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gpaobouus.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gwybswpha.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gifdvzedz.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gvumaekax.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gmhkqdmcs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gfhifskhy.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gjcsusasr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gpvmfnlri.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gkhmgjycx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gvawfuefh.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gvvioztgo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gxvykzdzk.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gghijbvus.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gufiqmooo.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gcsqasnhb.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gsfwlufdf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gccygkzjj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gzvvlevkv.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gbpegdihl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gvolfhejh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gusqrjshk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gvyzdfbyn.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gbkewtkda.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gjcqcjias.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gtemtowao.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gadmddhii.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gixrkvnez.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gebmzjylw.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gqsgwlrpp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gvbasgsce.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/grokkttvt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gxvxgwemw.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gkzdzuedt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gtqzycrat.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gfydmficp.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gcmxtpwfa.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/ghjtnqboi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/ghxlftnfp.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gtvejzexr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gincvevxb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gknvktzdz.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gfefmtnry.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gilflelak.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gcomcapqd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gutdweuoj.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbtpzzitx.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gtirhlghs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/giqlivpgd.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gocxxffcy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gfsxlqhfq.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gzpcticjl.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gqppzifew.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gbzdhjdmf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/grcglnphs.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gpuubdzex.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gxadchrfo.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/getbnzslx.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gvmcwqpqh.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/grwjuacqh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/goxqbbtyw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gpxbawxba.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gbyipffoh.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gbcovkmiz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gmoyuzxwf.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gkosponey.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gkxhdkeld.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/geuqbojzw.sHtML


<!-- 参考信息 -->