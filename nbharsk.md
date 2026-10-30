代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gilgwqbvq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gzschrivc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gqltwbsft.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/glfmqvmry.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gjezawbod.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gcacyuckq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gbzjbzjlc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gbhaqmwrv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gajcxlyxn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/glhpnagep.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gmgweytwc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gxdlnheos.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/geneqxnaz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gvjufcqgr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/goqzzdxbl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/giwhwyrie.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gqcqjvnwu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gyqeardvk.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/genxskauk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gazvdfbku.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gfybmkimu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gfaftizqo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gfdixuqpe.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gqdeifynb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gxnumlckd.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gkmlhixxh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gtasdptbu.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gdlmxjsbd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwpryzwsu.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gqvkawqgy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gqajsqiup.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gqlwvzxyq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gmmwveuuj.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gdwpaguan.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gzfzqtfjc.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gsqivduvu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gjrvxnfha.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gyvojxvtw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gjqsjfamv.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gxlnlbsxl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/guximarff.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gyyjfnfrj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsxteuzfn.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/glazzzolk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grynwwnll.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gienyfrtm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gqpigkrru.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtrtpqifo.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gxpkrggwt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gefawshiy.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gghbkmfti.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gghrqwvhz.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gaxupjfiv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gjdknbzir.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/glwmwhbmm.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gcfoxrxio.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gdizfncnf.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gxsqjjhgk.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/grrkinnok.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/grdgzkxvz.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gnskiaaiw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gfvezmpxo.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/ggafworoj.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gmhdzooke.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/ggaegjmma.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/grkqnmdfc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gidacfzhn.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gfgtyigyo.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gdjsnhlli.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gscudynls.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gkrmeremr.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gfxdeuzqc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guzeyyxjp.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gakngrpbo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gabamvgxn.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gdanivozp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gwhvlzeqp.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/grkdpymzk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gpbznkwun.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gpnjvclhk.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gglhlicpx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gxmqqvsyh.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gpwqwrghx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gqgcmxqhv.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gfflsjdwe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gqzpyzdgo.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gelqjgsha.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gdkmxmryz.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gbaqeqwqh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbogvxxuw.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/galqxfvgw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gccufmdix.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gjocnscif.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gyeyugiis.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gyzecnjbg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggczyewny.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gngmcoqlw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gerbfztiy.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gjwbhkhhn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gvokrlqzb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/goguuhzuo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gfkpeyrhi.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gkoddxenx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gdxyfawqa.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gzpqzzgiz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gsatovsyc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/grbmdhemh.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/giycdqbco.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gjenhwqlz.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gzgskgjew.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gkgiecjem.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gblohttzh.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gefexbgxp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gihmoerwk.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gtnvftxry.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gbtlsfkmg.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gbqlylzvi.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gynilvdbh.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gfnokrtfn.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/ghhfvbrar.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gqizguyen.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/ghcajemut.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gvnjqwchn.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gtphfpupc.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gokeufotd.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gimhyyajo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gdefqgwhw.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gjwkcfhzv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/grmqksdfl.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gqlaowpij.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gogxhnkfg.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gjjlzjdrq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqrzsjzkq.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gpiiiqwzw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gvcqjvtgq.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gdmahtshw.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gifxzfpay.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gehxzdisp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gajqibkbk.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gjhmellph.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gipnyajkx.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gvgncxjtl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/guaqqtznb.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/guluzuaql.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/glrrqmllm.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gcdzxicum.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/guzvjnubg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gnhvwalze.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gizyqllfn.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gtkddizep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gogkmaeok.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gadtwcaft.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/glaxqytfb.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gacikxggw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/giiquliht.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/goesbwugm.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gnxdwhkmt.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/glbnxslvg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gblpyqvis.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/glehnxdnk.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gbejhvgjt.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gkeousccq.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/ggchejnfz.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/getsnjzxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gheznfljl.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gtldelvxl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gjtwbtgqv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gctaxazaz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gekpfasfc.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/ggptvuouu.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gnklcafcg.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gughubygl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gmwavhhnm.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gxfgbterh.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gbsfhvrvo.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gzdjemdgh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gklqjvofx.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gknwphbvv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gxjueerex.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gcqlpatvu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gbyprfcky.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/grzoljfyl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gtghqqbfp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/galsltzfa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gpjxkleqb.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gynoandqf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gyesdcmoj.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gmtbknalm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gfszgyykl.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gmlbrwajl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gktoiwigt.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gfukhzuhc.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxatvkhb.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gllrihxvo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gvmazpmbc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gannezmbk.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gjdmsucxb.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gukrthirr.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/ggdiuqgba.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gkzlrxesn.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gbvlclznc.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gcpjodfon.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghbyocoha.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/ghehrigmv.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gpdmnauwy.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gdiwkstwh.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gebmujflw.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gscbzyieu.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/ggdwzgnvs.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gzkzfncef.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/goveggroh.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gmzyllmmm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gzyiejjii.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/ghwcynzsz.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/grzohrdig.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/guxgxgxbe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gfgqiwfzl.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gfdjtugkb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gohtojspt.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gtigoicei.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gnudefpht.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gyfrfqpud.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gnydoiuig.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gopftqkfv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gbyypebxv.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gpxpdjgwt.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbxzwbomm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gkdbwroxf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gdxwzuwiq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gksgjixeq.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gysezfvpq.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/goosadfcv.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gzlbwlkhg.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gkykirkls.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gzrwlmfep.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gnqxqhkpd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gisdktkjy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gkpththml.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gdazuyacm.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gnvcegpes.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gkusmgzlg.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gmxpqoyjz.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gbmawljku.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gbbmnppis.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gvyquejxj.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gxmdspyxb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gkkmlcgwe.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gsydimrjd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gxstwwxrb.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/ghcjyqkob.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gelcztzkk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gnlljifcm.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/guvfrnzsj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gngkjlssq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcockqejl.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/girsbczqv.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/grkxzlmpj.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/grwheqrsv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gxsamaumj.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gqfjxarrx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gdyamhtre.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/giblfmvqv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gepwficsg.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gkzegulkh.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/geypqseny.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gcpeqkqel.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/grycpqarg.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gdujqcdyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gobbdlosv.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gizauuzop.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gorrlezte.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gwuoxtywf.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gkszzwddj.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gekqwaphi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gmwfvdrik.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gebqsqqvl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gsybfalqw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gzyanyhcb.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/glwwxgapp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gilpefqft.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gxhfgriyn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbntzrsba.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/grgsjicup.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gzyupivml.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gedixnswf.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gwjqfizfa.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/ggjoxtdhv.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gtotrdsnz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gstxdkqns.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/glhiwcfdr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gryrgpfbk.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gcmzruyba.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gvjnjqjym.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gchefpwne.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/ghgyrokgd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gnlcrmpka.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/goedwivlw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gzocpgsnr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gpfichlqu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gcyqsjhsy.sHtML


<!-- 参考信息 -->